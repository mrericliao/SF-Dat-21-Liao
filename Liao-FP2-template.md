# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) SF-DAT-21 | Final Project, Part 2: Project Design Writeup and Approval Template

Follow this as a guide to completing the project design writeup. The questions for each section are merely there to suggest what the baseline should cover; be sure to use detail as it will make the project much easier to approach as the class moves on.

### Project Problem and Hypothesis

- What's the project about? What problem are you solving?
    
    *I will be looking at 2 third-party datasets for IP address geolocation (1 is considered the true set), and seeing what discrepancies lie within certain non-metropolitan regions.  For example, most of Spain's IP addresses show as being geolocated to Barcelona; I will look into big towns within Spain, and see which dataset is better in terms of accuracy, or exactly how much better the truth set is from the other third-party data.*
    
- Where does this seem to reside as a machine learning problem? Are you predicting some continuous number, or predicting a binary value?

    *I will use machine learning to determine how much more accurate one third-party dataset is at geolocation thant the other (truth set).  I will probably set dummy variables for the zip codes and see which set predicts certain zip codes better.*
    
- What kind of impact do you think it could have?

    *Having a granular IP address geolocation database is pivotal for most IT companies, or companies with a web presence.  Companies like Neustar actually pride themselves on having the most granular data, and this is a project that would be carried out by actual data sciences.*
    
- What do you think will have the most impact in predicting the value you are interested in solving for?

    *Accuracy in correctly predicting geolocation/zip codes will have the most important impact.  A lot of companies data stuff, where they'll guess a safe area to drop an IP address' geolocation, if they don't know the actual geolocation.  This causes certain datasets to appear more accurate than they really are.*  

### Datasets

- Description of data set available, at the field level.  (see table)
- If from an API, include a sample return.  (this is usually included in API documentation!) (if doing this in markdown, use the JavaScript code tag)

    *Both datasets will contain fields related to IP address geolocation (lat, long, city, zip code, etc.)*
    
    Dataset 1:
    | IP address | zip code | latitude | longitude | City |
    
    Dataset 2:
    | IP address | zip code | latitude | longitude | City |

### Domain knowledge

- What experience do you already have around this area?
    
    *I currently sell IP address databases, and am familiar with Neustar's data, as well as some competitors.*
    
- Does it relate or help inform the project in any way?

    *Yes, it helps because I'm already familiar with one of the data glosaries, but I'll have to figure out the other dataset, as it does not come with one.*
    
- What other research efforts exist?
    - Use a quick Google search to see what approaches others have made, or talk with your colleagues if it is work related about previous attempts at similar problems.
    - This could even just be something like "the marketing team put together a forecast in excel that doesn't do well."
    - Include a benchmark, how other models have performed, even if you are unsure what the metric means.

    *There are a lot of high-level information that various companies put out on IP addresses and geolocation.  I will be reading into said materials, but will be using one dataset in particular as the truth set (and benchmark).   
  

### Project Concerns

- What questions do you have about your project?  What are you not sure you quite yet understand?  (The more honest you are about this, the easier your instructors can help)

    *I'm not sure excaclty how I will do my analyzation of my datasets.  One dataset is also 7.2GB (.out.gz) file, and I can't figure out how to download it, as I keep getting a network timeout error.*
    
- What are the assumptions and caveats to the problem?
    - What data do you not have access to but wish you had?
    - What is already implied about the observations in your data set?  For example, if your primary data set is twitter data, it may not be representative of the whole sample.  (say, predicting who would win an election)
    
    *My assumption is that one dataset is more accurate than the other (an am using said datast as the truth set).  My datasets should both represent the entire population.*
    
- What are the risks to the project?
    - What's the cost of your model being wrong?  (What's the benefit of your model being right?)
    - Is any of the data incorrect? Could it be incorrect?
    
    *One risk of my project is that I can predict accuracy incorrectly, and the person I am sourcing my data from will spend money on a "bad" dataset.  It is quite possible that one dataset will be incorrect due to data stuffing.*

### Outcomes

- What do you expect the output to look like?
    
    *I expect one dataset to be a certain percent more accurate in non-metropolitan areas.  I will be looking into multiple regions, so just because one dataset is more accurate in one region, it doesn't mean that it is the most accurate overall.*
    
- What does your target audience expect the output to look like?

    *My target audience expects one third-party data, in particular, to be more accurate than the other in certain non-metropolitan areas.*
    
- What gain do you expect from your most important feature on its own?

    *I expect a gain of geolocation accuracy between the two datasets.  I will be able to determine which dataset is truly better (in certain regions & overall).*
    
- How complicated does your model have to be?

    *My model has to be able to accurately determine to certain percentages, standard deviations, etc. which dataset is truly better.*
    
- How successful does your project have to be in order to be considered a "success"?

    *My model, as an independent study, has to simply uncover the pros, cons, & accuracy between the 2 datasets.
    
- What will you do if the project is a bust (this happens! but it shouldn't here)?

    *I will cry first =P , then I will go back and see what mistakes I did (coding or regression model error), and redo my analysis.*

