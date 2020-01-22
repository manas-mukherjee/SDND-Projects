## 1st review 

Good job so far👏
It looks like you spent a lot of time learning the concepts and implementing them.
Your write up file is concise and well written.

Kudos 🙌 for identifying the issues you are facing and showing willingness to learn. Good attitude. Keep it up.

You are almost there. There are few minor changes or tweaks that are needed to finish this project as noted in the previous section.

The following changes that might help you in certain conditions like curved lanes, shadows etc.
1) Increasing min_line_len and max_line_gap for Hough Transform close to 100 will make your lines longer
2) You took kernel-size of the Gaussian Filter as 7, decreasing this will remove the noise making the image less blurry
3) Take a look at how you are classifying the lanes based on slope (Should it be >0 for right lanes? or should it be >0.5? Think about what your slope condition should be so as to remove horizontal lines as shown in the first image below
4) Region of interest : Look at your vertices in the last image below. Check your 2nd and 3rd points first dimension (530 and 440 ) Should it not be the other way around? Also try fine tuning your region of interest so your left and right lanes down overlap as seen in the second image

Reflection describes the current pipeline, identifies its potential shortcomings and suggests possible improvements. There is no minimum length. Writing in English is preferred but you may use any language.

Good work describing your current pipeline and figuring out some of its potential shortcomings and possible improvements.
Whereas more possible improvements are:
• Image from infrared camera.
• Adding a outlier reduction approach like RANSAC on the hough lines.
• Using curve fitting to plot the curve instead of straight lines
