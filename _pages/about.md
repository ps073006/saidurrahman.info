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
};


</script>
<body>
I am Saidur Rahman, a elebele <script>getAge();</script> PhD student (joined Fall-2017) in computer science at Montana State University, Bozeman, Montana. My advisor is Dr. Mike Wittie. I am interested in the design and analysis of Content Delivery Networks and measuring internet performance.

I am from Dhaka, Bangladesh which has full of natural beauties located in South Asia. I have done my B. Sc final examination (CGPA: 3.55) in Department of Computer Science & Engineering, University of Dhaka. I worked a as a Research Assistant at the Green Networking Research Group in the same department. Then I joined Samsung R&D Institute Bangladesh (September 2016- December, 2016). I worked as a lecturer in State University of Bangladesh (CSE department) (December,2016 to May 2017).
</body>
</html>
