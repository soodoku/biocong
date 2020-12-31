# Congressional Biographies

We scrape congressional biographies from the [Congressional Directory](https://www.govinfo.gov/app/collection/cdir/) from the 105th to the 115th Congress.

We iterate over the text biographical files, e.g.,  https://www.govinfo.gov/content/pkg/CDIR-2018-10-29/html/CDIR-2018-10-29-STATISTICALINFORMATION-2.htm and download the html files.  

We then parse the content of each file extracting the following information:

1. Name, e.g. RICHARD SHELBY
2. Party, e.g., Republican
3. location, e.g., Tuscaloosa, AL
4. born_in, e.g, Birmingham, AL 
5. birthdate, e.g., May 6, 1934
6. education, e.g., "attended the public schools;  B.A., University of Alabama, 1957; LL.B., University of Alabama School of Law, 1963;"
7. professional, e.g., "attorney; admitted to the Alabama Bar in 1961 and commenced practice in  Tuscaloosa; member, Alabama State Senate, 1970-78; law clerk, Supreme Court of Alabama, 1961-62; city prosecutor, Tuscaloosa, 1963-71; U.S. Magistrate, Northern District of Alabama, 1966-70; Special Assistant  Attorney General, State of Alabama, 1969-71; chairman, Legislative 
Council of the Alabama Legislature, 1977-78; former president, 
Tuscaloosa County Mental Health Association; member, Alabama Code 
Revision Committee, 1971-75; member, Phi Alpha Delta legal fraternity, 
Tuscaloosa County; Alabama and American Bar Associations; First 
Presbyterian Church of Tuscaloosa; Exchange Club; American Judicature 
Society; Alabama Law Institute;"
8. married, e.g., "the former Annette Nevin in 1960" 
9. children, e.g., "Richard C., Jr., and Claude Nevin" 
10. committees, e.g., "chair, Appropriations; Banking, Housing, and Urban Affairs; Environment and  Public Works; Joint Committee on the Library; Rules and Administration;  elected to the 96th Congress on November 7, 1978; reelected to the three  succeeding Congresses; elected to the U.S. Senate on November 4, 1986; reelected to each succeeding Senate term."


