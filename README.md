# UFO Data Report by Cameron Bannick
For the last 100 years or so, we have been plagued by the so called 'UFO Phenomenae'. It was quickly discredited due to the rising fear of the Soviet Union and written off as you would Ghosts or Bigfoot. However, as time went on and technology improved, a small minority of sightings could not be debunked or explained. This means, according to witnesses in the Naval Pilot Program eye witness testimony, there is a technology that defies our understanding of Physics and propulsion. A lot of our fighter jets sensors also fail to detect any heat signature from these aircrafts. Now, I want to clear, where these things come from are superfluous to the problem. There are highly advanced aircraft with an unknown propulsion system we cannot explain regularly flying in US air space.
# Issue Adressed
Our goal is to understand the relationship between Longitude, Lattitude, and DateTime features to better understand the relationship between them and a crafts shape.
# Data Provided
Our data was provided by kaggle and gave us a certain amount of sightings over the last 30 years in the US and Cananada. Our features include Date, Time, Shape, Longitude, Latitude, as well as a bunch of info regarding their comments on the sight. The biggest challenge facing this data set was the wide range of answers for our duration feature. There were answers ranging from actual numbers, to ranges of times, to the actual written 'cellphone'. After inspecting this feature in our data, I determined that these were unusable, due to a lot of the answers not indicating a time frame in the slightest. It should also be noted, these signts were from civilians, meaning their was no investigation into most events to verify how accurate the account was. 
# Data Visuals
![image](https://github.com/CameronBannick/Ufo_Report/blob/main/Data%20visuals/Number%20of%20sightings%20by%20shape.jpg)
 The most common UFO shape seems to come as a blinding light follwed by a circle. However, there are a few values that could possibly overlap (Light/Fireball and Circle/Sphere). 
![image](https://github.com/CameronBannick/Ufo_Report/blob/main/Data%20visuals/Number%20of%20sightings%20by%20month.jpg)
The trend for UFO sightings by month seems to be slow in the winter months while thy start increasing as it gets warmer. However, it could be possible there are other factors such as clearer skies, more people outside looking to the sky, ect. 
![image]([https://github.com/CameronBannick/Ufo_Report/blob/main/Data%20visuals/Number%20of%20sightings%20by%20month.jpg](https://github.com/CameronBannick/Ufo_Report/blob/main/Data%20visuals/Map%20of%20sigthings.png))
Assuming all of these shapes and sightings has been verified, the above visual is interesting because of the lack of structure. There are different types of crafts, assumingly for different purposes. But, what we see is no order or pattern, shapes are just randomnly spread out. Meaning, it is possible there a two or more culprits behind these phenomena of crafts. However, I will also say when sifting through this data, there didn't seem to be any standardization in the data collection.

# The Models
We created 2 versions of 3 different models in order to see how well we could predict the shape of the ufo given the Day, Month, Longitude, Lattitude, Year, and State. As stated earlier, the loss of the Duration feature will be a big loss to out overall predictions. In addition, we didn't have an equal amount of shapes to train our models with as the overwhelming majority of sights were descrived mearly as 'light'
Model 1 was only able to predict 21 percent of our sightings accurately and after some tweaking we got it to 22%. 
Model 2 came back at only 13 percent and after some adjustments we got it to 15 percent
Model 3 was stuck at 21 percent despite making some adjustments

The adjuststed Model 1 would seem to be the best performing.

# Conclusion
After sifting through all the data, it is very clear there needs to be a higher standar of data collection when it comes to UFOs. A lot of features originally provided could have been useful if all the entries weren't muddied with irrelevant ones (for example "Duration" had an entry "cell phone"). While we did make some good insights such as there being no pattern in shapes and the most common, even those could be misleading because certain entires in feature "shape" included values such as fireball and light which may or may not be considered the same thing. 
