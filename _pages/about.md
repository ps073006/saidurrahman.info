---
permalink: /
title: "Saidur Rahman"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<html>
<script>
function getAge() {

    function isLeap(year) {
        return year % 4 == 0 && (year % 100 != 0 || year % 400 == 0);
    }
    var birthDate = new Date(2017, 8, 27);
    var now = new Date(),
        age = now.getFullYear() - birthDate.getFullYear(),
        doyNow = now.getDoY(),
        doyBirth = birthDate.getDoY();

    // normalize day-of-year in leap years
    if (isLeap(now.getFullYear()) && doyNow > 58 && doyBirth > 59)
        doyNow--;

    if (isLeap(birthDate.getFullYear()) && doyNow > 58 && doyBirth > 59)
        doyBirth--;

    if (doyNow <= doyBirth)
        age--;  // birthday not yet passed this year, so -1
    if(age>2)
    {
      document.write(age+"rd");
    }
    else
    {
      document.write(age+"nd");      
    }
}


</script>
<body>
<p align="justify">I am Saidur Rahman, a Ph.D. student (joined Fall-2017) in Computer Science at Montana State University, Bozeman, Montana. My advisor is <a href="https://www.cs.montana.edu/mwittie/">Dr. Mike Wittie</a>. Currently, I am interested in applications of Augmented Reality in the intersection of edge, serverless computing paradigms. I am focusing my research activities towards this goal and tailoring my courses to increase knowledge in this area. Previously, I worked on DNS resolutions and Web performance.</p>

<p align="justify">I am from Dhaka, Bangladesh which has full of natural beauties located in South Asia. I have done my B. Sc in Department of Computer Science & Engineering, University of Dhaka. My CV is available for download <a href="https://drive.google.com/open?id=1yhvZXnDe3dt9yrIVhurmf93FMw0WWdYI">here</a> (Last updated 05/04/2020).</p>
</body>
</html>
