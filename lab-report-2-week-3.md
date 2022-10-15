# Lab Report 2
## Part 1
Code for my Simplest Search Engine
```
import java.io.IOException;
import java.net.URI;
import java.util.ArrayList;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    int num = 0;
    ArrayList<String> str = new ArrayList<>();

    public String handleRequest(URI url) {

        if (url.getPath().equals("/")) {
            return String.format("Number: %d", num);
        } else if (url.getPath().equals("/increment")) {
            num += 1;
            return String.format("Number incremented!");
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("count")) {
                    num += Integer.parseInt(parameters[1]);
                    return String.format("Number increased by %s! It's now %d", parameters[1], num);
                } else if(parameters[0].equals("s")) {
                    str.add(parameters[1]);
                    return String.format("Word added.");
                }
            } else if (url.getPath().contains("/search")) {
                String[] parameters = url.getQuery().split("=");
                ArrayList<String> output = new ArrayList<>();
                for(String word : str) {
                    if(word.contains(parameters[1])) {
                        output.add(word);
                    }
                }
                
                if(output.size() == 0) {
                    return String.format("No Match");
                } else {
                    return output.toString();
                }
            }
            return "404 Not Found!";
        }
    }
}

class SearchEngine {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```

![Add words](./searchEngine1.png)
To add the word apple, the main method is called. Then handleRequest is called. The url is passed into the handleRequest method. An arraylist of string named *str* is created with empty value. With *"/add"* and *"s"* present in the url, the word *"apple"* after *"="* is added to the *str*. Now *str* stores one element. *str* still holds one element after the request is done. 

![Add words](./searchEngine2.png)
I added another word. The process is most the same as described above. *str* now will hold two elements and will not change after the request is done.

![Search](./searchEngine3.png)
I added a few other words and then did a search for the words contain *"app"*. Since the url now contains the key word *"/search"*, it passes the if statement for search. A new arraylist of string named *"output"* is created to temporarily hold value that matches requirement. All the words in the variable *"str"* will go through the loop. The ones that contains *"app"* will be added to the *"output"*. The output is printed on the webpage at the end. After the request is done. *"str"* will not change, but *"output"* will be cleared. 


