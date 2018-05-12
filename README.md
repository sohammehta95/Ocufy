![Head](img/head-2.png)


Ocufy - a mobile eye testing interface with which any user can check their eye acuity in just under five minutes!

Check out the webpage for the project on : www.ocufy.xyz

# Abstract
Eye-testing is one of the most important health check-up required by all individuals. However, it turns out that it is also one of the most neglected check-ups of all time. Most people do not anticipate the need for checking their eyes until their vision is affected. Due to these reasons, we created Ocufy - a mobile eye testing interface with which any user can check their eye acuity in just under five minutes. Not only is it free to use for everyone, but it also provides one of the most accurate results of a mobile eye test. This accuracy is achieved with the help of an algorithm which finds the user’s screen-to-face distance and starts the test only after a minimum threshold is achieved thus providing the most authentic results. We performed the evaluation with 10 people and found out that the application provided accurate results 85% of the time. Moreover, the application received an average rating of 4.5/5 with over 80% respondents recommending it to use it next time to check their eyes.

# Intorduction
Today, with advances in technology, the human eye is getting more and more hitched to the digital screen making it prone to blurred vision. A study published in the journal Ophthalmology found that on current trends, 50 percent of people on the planet would need glasses or contact lenses with 10 percent suffering from severe myopia [1]. Our application relieves the pain of the user who has no access to an eye clinic. Also, it is for the user who does not anticipate the need for checking their eye until their vision is affected.


# Motivation
With each author diagnosed with myopia, one of the major motivation for this research project was to make people realize the importance of an eye test before there is a need for it. It is recommended for each person to get an eye test at least every two years. In one of the research study conducted, 80% of respondents believed that sight is the most important sense, however, a third hadn’t gotten an eye test in four years or more, with a worrying 6% have never had an eye exam [2]. 

According to WHO, an estimated 253 million people live with vision impairment where 36 million are blind and 217 million have moderate to severe vision impairment. 81% of people who are blind or have moderate or severe vision impairment are aged 50 years and above [3]. The other affected people are especially children and people from low and middle-income countries. Lastly, women are most affected by this as at least 2/3rd of blind people are women [4]. But the most important factor for motivation was that 80 percent of all vision impairment can be prevented or cured.

# Problems in Existing Systems
The systems discussed in the previous section has various limitations that make the vision testing and screening extremely difficult for the user. The reasons are:

## 1) Too Expensive for the average user

Most of the professional and accurate eye testing solutions are developed for oculists who can afford to buy these expensive software for their clinics. The average user cannot purchase these software as they are too expensive and are complicated to set up initially without the help of an expert user. For instance, the Canela 20/20 Vision offers their software for $49 or $69 monthly pricing plans while the Precision vision software is priced as high as $1125.

## 2)	Incorrect Results provided by most solutions:

To overcome the issue of expensive software and due to the increased availability of smartphones, many software developers hopped on the idea of making an eye testing application for smartphones. While this is a novel idea with which user can easily check their eye vision instantly, it seldom provides any accurate results. The main reason being that the same test is provided for every screen size and every person irrespective of the distance at which they are holding their phones.

<p align="center">
  <img src="img/incor.png"/>
</p>


# METHOD

To make the eye test mobile, we first need to understand how the traditional eye testing system works. We also need to understand how the results are evaluated for this test. Moreover, it has to be learned how can this method be converted so as to be viable to implement in a small phone screen.


## 1) Understanding the Snellen Chart
A Snellen chart is an eye chart that can be used to measure visual acuity. Snellen charts are named after the Dutch ophthalmologist Herman Snellen, who developed the chart in 1862. The normal Snellen chart is printed with eleven lines of block letters. The first line consists of one very large letter, which may be one of several letters, for example, E, H, or N. Subsequent rows have increasing numbers of letters that decrease in size. A person taking the test covers one eye from 6 meters or 20 feet away, and reads aloud the letters of each row, beginning at the top. The smallest row that can be read accurately indicates the visual acuity in that specific eye. The symbols on an acuity chart are formally known as "optotypes"

<p align="center">
  <img src="img/snellen.png"/>
</p>

## 2) Optotypes and their Characteristics
In the case of the traditional Snellen chart, the optotypes have the appearance of block letters and are intended to be seen and read as letters. They are not, however, letters from any ordinary typographer's font. They have a particular, simple geometry with some unique characteristics. The following are the features of the optotypes:
•	Snellen developed optotypes using symbols based in a 5×5-unit grid so that the size of the critical detail (each gap width) subtends 1/5th of the overall height
•	The thickness of the lines equals the thickness of the white spaces between line
•	The height and width of the optotype (letter) is five times the thickness of the line.

<p align="center">
  <img src="img/opto.png"/>
</p>

## 3) Constructing Visual Acuity Chart

Before constructing a Visual Acuity Chart, one needs to know and decide what kind of chart one wants to construct. There are actually different kinds of charts for visual acuity measurement with Snellen chart being the most common. Based on construction they generally fall into two categories, Snellen and logMAR [11]. Visual Acuity Chart can be constructed based on 2 criteria: 

1.	Measurement of minimum separable acuity
2.	Measurement of minimum recognizable acuity

Two distinct points can only be recognized as separate when they subtend an angle of one minute arc at nodal point of eye.


## 4) Defining Standard Vision
Snellen defined “standard vision” as the ability to recognize one of the optotypes when it subtends an angle of 5 minutes of arc. It is a representation of visual acuity in the form of a fraction (e.g. 6/6, 20/20) in which the numerator is the testing distance, and the denominator is the distance at which smallest Snellen letter read by the eye has an angular size of 5 minutes.

<p align="center">
  <img src="img/eq.png"/>
</p>

For example, 6/60 means the ability to see an object only at 6 meters which should be normally seen at 60 meters. At 6-meter (20 ft.), the letters on the 6/60 (or 20/20) line should subtend 5 minutes of arc (each limb of the letters subtend 1 minute of arc)
