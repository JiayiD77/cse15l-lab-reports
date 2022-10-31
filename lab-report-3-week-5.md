# Lab Report 3
## Use command *grep*

*grep -n*
Example 1 (I am using '...' to represent the remaining output so that I don't have to copy all the output here which is way to much lines)
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -n "chapter" ./technical/*/*.txt
./technical/911report/chapter-1.txt:560:    Others in the agency were aware of it, as we explained earlier in this chapter.
./technical/911report/chapter-10.txt:162:                chapter 3). Ashcroft told us he was determined to take every conceivable action,       
./technical/911report/chapter-10.txt:420:                Iraqi intelligence officer (discussed in chapter 7) and a Polish report that
./technical/911report/chapter-11.txt:226:                (reprinted in chapter 4), brought the focus back to more traditional hostage taking;   
./technical/911report/chapter-11.txt:299:                the main focus (war in Korea), and as too unrealistic. As we pointed out in chapter    
./technical/911report/chapter-11.txt:403:                the embassy bombings of August 1998. We described those decisions in chapter 4. It     
./technical/911report/chapter-11.txt:472:            Earlier chapters describe in detail the actions decided on by the Clinton and Bush
./technical/911report/chapter-11.txt:538:                capabilities were in the domestic arena. In chapter 3 we discussed these
./technical/911report/chapter-11.txt:588:                Kuala Lumpur, detailed in chapter 6. In late 1999, the National Security Agency        
./technical/911report/chapter-12.txt:51:            As we mentioned in chapter 2, Usama Bin Ladin and other Islamist terrorist leaders
./technical/911report/chapter-12.txt:196:            Many details in chapters 2, 5, and 7 illustrate the direct and indirect value of the       
./technical/911report/chapter-12.txt:783:                dangerous weapons. As we note in chapter 2, al Qaeda has tried to acquire or make      
./technical/911report/chapter-12.txt:784:                nuclear weapons for at least ten years. In chapter 4, we mentioned officials
...
```

 Example 3
 ```
 ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -n "gene" ./technical/government/*/*.txt
./technical/government/Media/Annual_Fee.txt:76:years. The additional revenue generated by the fee hike will allow
./technical/government/Media/Anthem_Payout.txt:55:people by surprise. And while it was generally a nice surprise, it
./technical/government/Media/Anthem_Payout.txt:87:an expert abou their particular situation, there are some general
./technical/government/Media/Anthem_Payout.txt:93:In general, you must receive fair-market value for whatever you
./technical/government/Media/Attorney_gives_his_time.txt:7:Attorney gives of his time generously
./technical/government/Media/balance_scales_of_justice.txt:49:economic means will generally do better in the judicial system than
./technical/government/Media/balance_scales_of_justice.txt:61:A large portion comes from the interest generated by the state's
./technical/government/Media/Barr_sharpening_ax.txt:28:political activities. Edwin Meese, attorney general under President
./technical/government/Media/Campaign_Pays.txt:34:Last year's campaign generated enough money and resources to
./technical/government/Media/City_Council_Budget.txt:51:McMahon, the general counsel of the City Council, said that in view
./technical/government/Media/CommercialAppealMemphis2.txt:47:court-generated fees from two other programs.
./technical/government/Media/CommercialAppealMemphis2.txt:71:people too well, except in fee-generat-ing type cases," Brewer
./technical/government/Media/Coup_Reshapes_Legal_Aid.txt:224:generally want to give to programs that do quality work because
./technical/government/Media/Court_Keeps_Judge_From.txt:22:attorney general contends that the money belongs in the state's
./technical/government/Media/defend_yourself.txt:44:are so rare that statistics about the practice generally are not
./technical/government/Media/Entities_Merge.txt:51:TRLA generated controversy in 1996, when its attorneys
./technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:19:in the general population.
./technical/government/Media/Firm_to_the_Poor_Needs_Help.txt:44:Historically, LSEO letter-writing campaigns generated from
./technical/government/Media/Funds_Shortage.txt:33:generated on client assets held in trust by lawyers in
./technical/government/Media/Good_guys_reward.txt:131:''My part in the firm is not to generate income,'' he said. ''A
./technical/government/Media/Good_guys_reward.txt:137:He's confident that they, like he, will always give generously
./technical/government/Media/grants_fail_to_come.txt:82:"Anything in between, you"re screwed. Basically the general
./technical/government/Media/Greedy_Generous.txt:12:antithetically named site generousassociates.com. What, if
./technical/government/Media/Greedy_Generous.txt:44:and generosity, these two sites and the underlying issues they
...
 ```

 The command *grep -n* opion takes a pattern in "" and a file option after it and return all the lines that in file that contains the pattern with the prefix of line number added before the actual content of the line. This can be used if we the actual content of the file is really large. With the line number provided, we can easily locate where the content is.


*grep -n*

Example 1
 ```
 ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -r "this is" ./technical
./technical/911report/chapter-1.txt:    FAA: No, this is not an exercise, not a test. 
./technical/911report/chapter-1.txt:    The failure to find a primary radar return for American 77 led us to investigate this issue further. Radar reconstructions performed after 9/11 reveal that FAA radar 
equipment tracked the flight from the moment its transponder was turned off at 8:56. But for 8 minutes and 13 seconds, between 8:56 and 9:05, this primary radar information on American 77 was not displayed 
to controllers at Indianapolis Center.
./technical/911report/chapter-1.txt:    Then, at 9:39, a fourth radio transmission was heard from United 93: Ziad Jarrah: Uh, this is the captain. Would like you all to remain seated. There is a bomb on board and are going back to the airport, and to have our demands [unintelligible]. Please remain quiet.
./technical/911report/chapter-1.txt:    The Secret Service logged Mrs. Cheney's arrival at the White House at 9:52, and she joined her husband in the tunnel. According to contemporaneous notes, at 9:55 the 
Vice President was still on the phone with the President advising that three planes were missing and one had hit the Pentagon. We believe this is the same call in which the Vice President urged the President not to return to Washington. After the call ended, Mrs. Cheney and the Vice President moved from the tunnel to the shelter conference room.
./technical/911report/chapter-11.txt:                them and then develop a fully informed joint plan. Accomplishing all this is
./technical/911report/chapter-12.txt:                protect the interests of their home states or districts. But this issue is too
./technical/911report/chapter-13.1.txt:            We recognize that this is a new and difficult idea precisely because the authorities
./technical/911report/chapter-13.1.txt:                administration) told us that this is perhaps the single largest obstacle impeding
./technical/911report/chapter-13.1.txt:                over its national security mission. Part of the reason for this is the demand around
./technical/911report/chapter-13.4.txt:                industry, devoted enormous resources to investigating this issue, including securing
./technical/911report/chapter-13.4.txt:                Mihdhar to the community, this is belied by the hijackers' apparent decision to     
./technical/911report/chapter-13.5.txt:                don't believe anybody said this is likely al Qaeda. I don't think so." White House  
./technical/911report/chapter-2.txt:                without assaulting them, even if this involved the killing of Muslims, this is
./technical/911report/chapter-8.txt:                this is incorrect. Both Hazmi and Mihdhar could have been held for immigration
./technical/911report/chapter-9.txt:                lobby, "One of the most critical things in a major operation like this is to have      
./technical/biomed/1468-6708-3-1.txt:          persons, but we think this is unlikely given the absence
...
 ```

Example 2
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -r "this is" ./technical/biomed/
./technical/biomed/1468-6708-3-1.txt:          persons, but we think this is unlikely given the absence
./technical/biomed/1468-6708-3-4.txt:        simple algebra can show that this is always so. We can see
./technical/biomed/1468-6708-3-7.txt:        disease. If this is the mechanism responsible for
./technical/biomed/1471-2091-3-14.txt:          analysis. We suspect this is because many genes that are
./technical/biomed/1471-2091-3-16.txt:        If this is the case, then a small alteration in position of
./technical/biomed/1471-2091-3-16.txt:        residues line up as shown in our model. While this is not
./technical/biomed/1471-2091-3-4.txt:        metal binding (Table 2), and we postulate this is due to
./technical/biomed/1471-2091-3-8.txt:        intracellular ThDP is about 30 μM, much of this is found in
./technical/biomed/1471-2091-3-8.txt:        However, this is not the case as
./technical/biomed/1471-2091-4-1.txt:        To our knowledge, this is the first report on the
./technical/biomed/1471-2091-4-5.txt:          (~50 kDa, Fig. 1B). We assumed that this is due to a
...
```

Example 3
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -r "this is" ./technical/government/
./technical/government/About_LSC/diversity_priorities.txt:lawyer should have one, and that this is critical to moving people
./technical/government/About_LSC/reporting_system.txt:client-eligible population. In the first instance, this is done by
./technical/government/About_LSC/State_Planning_Report.txt:passed, this is expected to generate about $150,000 annually, all
./technical/government/Alcohol_Problems/DraftRecom-PDF.txt:not using a uniform screening method. He agreed that this issue
./technical/government/Alcohol_Problems/DraftRecom-PDF.txt:specifically for this topic. He said the way to accomplish this is
./technical/government/Alcohol_Problems/DraftRecom-PDF.txt:other conferences, which indicates that this issue is high on the
./technical/government/Alcohol_Problems/Session2-PDF.txt:screens may address this issue by allowing patients to spend more
./technical/government/Alcohol_Problems/Session3-PDF.txt:alcohol use. It is thought that this is particularly true if the
./technical/government/Alcohol_Problems/Session3-PDF.txt:outcome. She thought more research is needed on this issue.
./technical/government/Alcohol_Problems/Session3-PDF.txt:Barry reinforced the importance of looking at this issue by age
./technical/government/Alcohol_Problems/Session3-PDF.txt:predictors. More data on this issue could help us plan better
./technical/government/Alcohol_Problems/Session4-PDF.txt:As we already know, this is a complex problem that probably does
...
```

The command option *grep -r* will recursively look through all the subdirecories and files under the given directory with out the needed to give the file path. This can be really useful if the directory has many subdirectories but we want to look through all the files in it. There is no need to write file path like *./technical/*/*/*/*/*/*/*.txt* but simply *./technical*.

*grep -v*

Example 1
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -i "chapter" ./technical/*/*.txt
./technical/911report/chapter-1.txt:    Others in the agency were aware of it, as we explained earlier in this chapter.
./technical/911report/chapter-10.txt:                chapter 3). Ashcroft told us he was determined to take every conceivable action,
./technical/911report/chapter-10.txt:                Iraqi intelligence officer (discussed in chapter 7) and a Polish report that
./technical/911report/chapter-11.txt:                (reprinted in chapter 4), brought the focus back to more traditional hostage taking;
./technical/911report/chapter-11.txt:                the main focus (war in Korea), and as too unrealistic. As we pointed out in chapter
./technical/911report/chapter-11.txt:                the embassy bombings of August 1998. We described those decisions in chapter 4. It
./technical/911report/chapter-11.txt:            Earlier chapters describe in detail the actions decided on by the Clinton and Bush
./technical/911report/chapter-11.txt:                capabilities were in the domestic arena. In chapter 3 we discussed these
./technical/911report/chapter-11.txt:                Kuala Lumpur, detailed in chapter 6. In late 1999, the National Security Agency
./technical/911report/chapter-12.txt:            As we mentioned in chapter 2, Usama Bin Ladin and other Islamist terrorist leaders
./technical/911report/chapter-12.txt:            Many details in chapters 2, 5, and 7 illustrate the direct and indirect value of the
./technical/911report/chapter-12.txt:                dangerous weapons. As we note in chapter 2, al Qaeda has tried to acquire or make
./technical/911report/chapter-12.txt:                nuclear weapons for at least ten years. In chapter 4, we mentioned officials
./technical/911report/chapter-12.txt:            First, as we will discuss in chapter 13, to open up the sharing of information across
./technical/911report/chapter-13.1.txt:                opportunities,"some of which we reviewed in chapter 11. These are often
./technical/911report/chapter-13.1.txt:                "connecting the dots." In chapter 11 we explained that these labels are too narrow.
./technical/911report/chapter-13.1.txt:                    described in chapter 12.
./technical/911report/chapter-13.1.txt:                still not sized or funded to be an executive agency. In chapter 3 we described some
./technical/911report/chapter-13.1.txt:                regions, countries, and issues that we discuss in chapter 12. Much of the job of
./technical/911report/chapter-13.1.txt:            We summarized the resulting organization of the intelligence community in chapter 3.
./technical/911report/chapter-13.1.txt:                    civil-military misunderstandings we described in chapter 4. It is a problem to
./technical/911report/chapter-13.1.txt:                describe in chapter 8, the information is distributed, but in a compartmented
./technical/911report/chapter-13.1.txt:            In chapter 6, we described the transition of 2000-2001. Beyond the policy issues we
...
```

Example 2
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -i "CHAPTER" ./technical/*/*.txt
./technical/911report/chapter-1.txt:    Others in the agency were aware of it, as we explained earlier in this chapter.
./technical/911report/chapter-10.txt:                chapter 3). Ashcroft told us he was determined to take every conceivable action,      
./technical/911report/chapter-10.txt:                Iraqi intelligence officer (discussed in chapter 7) and a Polish report that
./technical/911report/chapter-11.txt:                (reprinted in chapter 4), brought the focus back to more traditional hostage taking;  
./technical/911report/chapter-11.txt:                the main focus (war in Korea), and as too unrealistic. As we pointed out in chapter   
./technical/911report/chapter-11.txt:                the embassy bombings of August 1998. We described those decisions in chapter 4. It    
./technical/911report/chapter-11.txt:            Earlier chapters describe in detail the actions decided on by the Clinton and Bush        
./technical/911report/chapter-11.txt:                capabilities were in the domestic arena. In chapter 3 we discussed these
./technical/911report/chapter-11.txt:                Kuala Lumpur, detailed in chapter 6. In late 1999, the National Security Agency       
./technical/911report/chapter-12.txt:            As we mentioned in chapter 2, Usama Bin Ladin and other Islamist terrorist leaders        
./technical/911report/chapter-12.txt:            Many details in chapters 2, 5, and 7 illustrate the direct and indirect value of the      
./technical/911report/chapter-12.txt:                dangerous weapons. As we note in chapter 2, al Qaeda has tried to acquire or make     
./technical/911report/chapter-12.txt:                nuclear weapons for at least ten years. In chapter 4, we mentioned officials
./technical/911report/chapter-12.txt:            First, as we will discuss in chapter 13, to open up the sharing of information across     
./technical/911report/chapter-13.1.txt:                opportunities,"some of which we reviewed in chapter 11. These are often
./technical/911report/chapter-13.1.txt:                "connecting the dots." In chapter 11 we explained that these labels are too narrow. 
./technical/911report/chapter-13.1.txt:                    described in chapter 12.
```

Example 3
```
ucsd@DESKTOP-TN1IVAS MINGW64 /d/cse15l/docsearch (main)
$ grep -i "GENE EXPRESSION A" ./TECHNICAL/BIOMED/*.txt
./TECHNICAL/BIOMED/1471-2091-2-13.txt:          concentration of 1 mM to induce gene expression and the
./TECHNICAL/BIOMED/1471-2091-3-14.txt:          Gene expression analysis was performed using
./TECHNICAL/BIOMED/1471-2091-3-23.txt:        important role in the regulation of gene expression and in
./TECHNICAL/BIOMED/1471-2105-3-17.txt:        has permitted global measurement of gene expression at the
./TECHNICAL/BIOMED/1471-2105-3-17.txt:          inclusion in the gene expression analysis experiment.
./TECHNICAL/BIOMED/1471-2105-3-17.txt:          Gene expression analysis using the murine 11k
./TECHNICAL/BIOMED/1471-2105-3-22.txt:        provide an overall idea of gene expression and contribute
./TECHNICAL/BIOMED/1471-2105-3-23.txt:        study differences in gene expression associated with
./TECHNICAL/BIOMED/1471-2105-3-23.txt:        in gene expression are to be detected. A further reduction
./TECHNICAL/BIOMED/1471-2105-3-3.txt:        hope in recent years, gene expression array technology has
./TECHNICAL/BIOMED/1471-2121-3-30.txt:        the light-responsive gene expression and photomorphogenic
./TECHNICAL/BIOMED/1471-2121-3-6.txt:        changes in gene expression and cellular proliferation. In
./TECHNICAL/BIOMED/1471-2121-4-6.txt:        step in gene expression as inhibition of mRNA targeting can
./TECHNICAL/BIOMED/1471-213X-1-13.txt:        Delta gene expression appears to
./TECHNICAL/BIOMED/1471-213X-1-15.txt:          gene expression and transrepresses NF-κB [ 47 ] . To
./TECHNICAL/BIOMED/1471-213X-1-9.txt:        3, 4, 5] that rhythms of gene expression are of central
```

The command option *grep -i* will ignore the case distinction in both the pattern and file provided. It is pretty useful because the words at the beginning of a sentence have a captical letter. Using -i can help us avoid doing work such as *grep "this"* and *grep "This"*.