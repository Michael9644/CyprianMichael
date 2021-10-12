Name: Cyprian-Michael Nwankwo

Activity File: Exploring Kibana
You are a DevOps professional and have set up monitoring for one of your web servers. You are collecting all sorts of web log data and it is your job to review the data regularly to make sure everything is running smoothly.
Today, you notice something strange in the logs and you want to take a closer look.
Your task: Explore the web server logs to see if there's anything unusual. Specifically, you will:
:warning: Heads Up: These sample logs are specific to the time you view them. As such, your answers will be different from the answers provided in the solution file.
Instructions
Add the sample web log data to Kibana.
Answer the following questions:
In the last 7 days, how many unique visitors were located in India? There are 223
In the last 24 hours, of the visitors from China, how many were using Mac OSX? They were 9 visitors
In the last 2 days, what percentage of visitors received 404 errors? How about 503 errors? 6.383% for 404 and 2.128% for 503
In the last 7 days, what country produced the majority of the traffic on the website? China, with 314 traffics on the website.
Of the traffic that's coming from that country, what time of day had the highest amount of activity? The 12th hour of the day has the highest amount.

List all the types of downloaded files that have been identified for the last 7 days, along with a short description of each file type (use Google if you aren't sure about a particular file type).
Gz:A GZ file is basically an archive compressed using the gzip compression technology. Like other file archives, this archive type helps you combine your files and reduce the size of your files by compressing them.
Css:CSS (Cascading Style Sheets) are files that describe how HTML elements are displayed on the screen, paper, etc. With HTML, you can have either embedded styles or styles can be defined in an external stylesheet. 
Zip:a computer file whose contents of one or more files are compressed for storage or transmission. A ZIP file may contain one or more files or directories that may have been compressed.
Deb: A DEB file is a standard Unix archive that contains two bzipped or gzipped archives, one for the installer control information and another for the actual installable data. DEB files are often used for software installation packages by multiple versions of Linux including Ubuntu, Kubuntu , Edubuntu, and PCLinuxOS.
Rpm: An RPM file is an installation package originally developed for the Red Hat Linux operating system, but now used by many other Linux distributions as well.

Now that you have a feel for the data, Let's dive a bit deeper. Look at the chart that shows Unique Visitors Vs. Average Bytes. 1 unique Visitor with Avg. Bytes of 9,367

In your own words, is there anything that seems potentially strange about this activity?
Filter the data by this event.
What is the timestamp for this event?10/26/2020 	10:55
What kind of file was downloaded? India
From what country did this activity originate?
What HTTP response codes were encountered by this visitor?100 % HTTP
Switch to the Kibana Discover page to see more details about this activity.
What is the source IP address of this activity? 35.143.166.159
What are the geo coordinates of this activity? Lat : 
{
  "lat": 43.34121,
  "lon": -73.6103075
}


What OS was the source machine running? Windows 8
What is the full URL that was accessed? In the screenshoot
From what website did the visitor's traffic originate? http://facebook.com
Finish your investigation with a short overview of your insights.
What do you think the user was doing? It seems they are on Facebook and from their click on the elastic file that lead them to the metric beat.
Was the file they downloaded malicious? If not, what is the file used for? The file was not malicious, but can definitely be used for malicious purposes.
Is there anything that seems suspicious about this activity? Yes, why it came from Facebook looks suspicious.
Is any of the traffic you inspected potentially outside of compliance guidlines?yes, why a companies metric beat should coming from a Facebook link seems suspicious.