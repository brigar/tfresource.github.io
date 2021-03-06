---
title: "Model Validation and Reasonableness Checking/Amount Of Travel"
categories:
  - Needs Review
---

### Amount of Travel or Activity

\_\_TOC\_\_

The first step in the conventional four-step travel demand forecasting process is the generation of the travel activity for the modeled time period (e.g., daily, peak hour, etc.). Average weekday (referred to hereafter as “daily”) travel is normally generated although there are models that have focused on shorter time periods. In four-step models, the generation of daily travel is referred to as trip generation. In activity-based models, model components related to the generation of daily travel include the generation of daily activity patterns for households, tour and subtour generation, and intermediate stop generation. All of these types are referred to in this chapter as “trip generation models.”

In four-step models, trip generation is the step where the purposes and amount of travel are calculated. Home-based trips are forecast from the home locations to activities outside the home including work, school, shopping, recreation, social, or other activities. The nonwork related trips are often aggregated into one or more nonwork trip purposes. Four-step models forecast trip productions and attractions, with each trip having one production end and one attraction end. Productions are related to the home end of the trip while attractions are related to the nonhome end. For example, on a daily basis, a single worker may generate two home-based work trip productions at home – a trip from home to work and a trip from work to home. At the work location, the same worker would generate two attractions for the same two trips. Trip productions and attractions focus on the locations generating the travel, not the directionality of travel.

Four-step models must also account for nonhome-based trips which do not start or end at the traveler’s home. While the definition of which end of a nonhome-based trip is the production end and which is the attraction end is not critical, by convention the origin is usually designated as the production end. Some regions have subdivided nonhome-based trips into work-based other and other-based other trips. In some cases, the work location has been designated the production end of work-based other trips and the nonwork location the attraction end. Models have used different methods for account for nonhome-based trip making. Since nonhome-based trip-making is performed by persons living in households, a common method for accounting for the trips is to generate them at a household level and then allocate the trips to origins and destinations outside the home.

In conventional four-step models, the most common forms of trip production and attraction models are cross-classification and linear regression, ([13](#fn13)) with cross-classification more common for trip production models and regression more commonly used for trip attraction models. In a cross-classification model, the number of trips is estimated for each combination of the values of two or more independent variables. Typically, these are household characteristics such as the number of persons (household size), number of workers, number of vehicles, and income level. Categories nearly always include aggregations of levels (for example, five or more persons). In a regression model, the number of trips is estimated as a linear combination of variables. For trip attraction models, these are usually zone-level variables representing levels of activity in the zone. They generally include the number of households or persons and the number of employees classified by type (for example, retail, service, etc.).

In activity-based modeling, the focus is the generation of daily activities performed by residents and the travel required to perform those activities. Daily activities that take place outside the home are grouped together to form tours. Each home-based tour begins and ends at home and includes one or more stops along the tour, with common practice designating a particular activity as the primary activity of the tour. Thus, a worker making trips to and from work would be represented by one home-based work tour. Tours may be generated from homes with the tour type being determined by the primary activity performed at the location outside the travelers’ homes. Subtours may be generated from nonhome locations, typically work locations. Work-based subtours begin and end at the work location.

Each tour may have intermediate stops, beyond the primary activity location, to perform additional activities. For example, a worker might have to drop off a child at day care on the way to work and pick the child up on the way from work to home. In a four-step model, such a pattern would result in two home-based nonwork trip productions (at the home), two home-based nonwork attractions at the day-care, and two nonhome-based trips, one with an origin at the day care and a destination at the work location and one with an origin at the work location and a destination at the day-care. In an activity-based model, such an activity pattern would result in one tour that includes two intermediate stops.

Activity-based models do not compute trip attractions as used in four-step models. The activity locations that would correspond to the attraction ends of trips are estimated during the destination choice (primary activity and intermediate stop) models, which are described in [Distribution](Model_Validation_and_Reasonableness_Checking_Distribution). This means that any checks of trip attractions described in this chapter cannot be performed until after the destination choice models have been estimated. It is still good practice, however, to perform these checks.

Multinomial logit is the most common form of models of tour and activity generation within activity-based models. These may range from relatively simple models of the exact number of tours or subtours to complex models indicating which combinations of activities are undertaken by a person throughout the day. Variables usually include a variety of characteristics of the traveler and his/her household, area or zone characteristics such as residential or employment density, and accessibility variables computed from “logsums” from subsequently applied destination and mode choice models, as well as a variety of constant terms related to individual alternatives (which may represent complex combinations of activities). It is important to recognize that an activity-based model will have several model components related to trip generation, and each of them must be validated individually, as well as the aggregate results of the activity generation process.

Additional components of travel are typically included in the trip generation step including commercial vehicle trips, internal-external trips, and external-external trips. Most current models use conventional approaches such as cross-classification and linear regression to generate travel for these trip purposes.

The common concept for both four-step and activity-based models is that they both generate measurable amounts of activity or travel. In validating trip generation models, past practice has focused on aggregated statistics related to the numbers of trips generated. With activity-based modeling techniques, the need for disaggregate validation testing has become more pronounced. Both aggregate and disaggregate validation checks may be performed for activity-based models. While it may be more difficult or require more innovation, some disaggregate validation tests may also be performed for four-step models. Evaluation and validation of trip- and tour- generation models are important since the information resulting from this step (i.e., trips or tours) provides the basis for all of the subsequent steps. Errors in this step will propagate through the model chain.

### Residential Person Travel

Residential person travel is defined as travel made by residents of the modeled region, within the modeled region. Not included in this definition are trips made with one or both ends outside the modeled region, truck and commercial vehicle trips, and trips made to and from “special generators” even though they are made by residents of the modeled region. These other types of travel are discussed in subsequent sections of this chapter.

In four-step models, trips made for residential person travel are often referred to as “internal-internal” trips to denote both trip ends being located within the modeled region. The outputs of internal-internal trip generation are productions and attractions by trip purpose at the zone level. In activity-based models, this type of travel is often referred to simply as residential or resident travel. Activity-based models generate outputs at a disaggregate level (i.e., for each modeled person). There are different outputs depending on model structure, but usually produce the following:

-   Number of activities by purpose;
-   Number of tours by purpose;
-   Number of stops on each tour; and
-   Number of work-based subtours.

Some models may also estimate joint activity or travel participation among household members, and so additional outputs related to this joint participation may be produced.

#### Sources of Data (Trip Generation)

Whenever a recent local household travel/activity survey is available, it is the source for the estimation of resident person travel models, whether in a four-step or activity-based modeling context. In some areas, establishment surveys are performed to assist in the development of trip attraction models.

When recent survey data that could be used for model estimation are not available, model parameters such as trip rates may be transferred from another model or borrowed from other data sources. A common source is the National Household Travel Survey (NHTS), a national survey of personal travel last conducted in 2008. Some other national data sources include the NCHRP Report 365, Travel Estimation Techniques for Urban Planning, which is being updated (the update is expected to be available in 2010), and other documents (e.g., TCRP Report 73, Characteristics of Urban Travel Demand). These reports summarize information from the NHTS and from travel models for various types of urban areas and planning contexts.

Models are estimated, of course, using the best available data, whether it is locally collected, transferred, or from national sources. The truly independent sources of trip generation data needed for model validation generally do not exist for the local area, except in the rare instance when a household survey data set is so large that it can be split into estimation and validation data sets. The validation checks described below therefore rely on the use of the estimation data sources themselves. The national sources can be used as reasonableness checks for various aggregate checks. Household survey data sets collected for two different points in time for a region might be used for sensitivity testing.

#### Aggregate Checks (Trip Generation)

##### Four-Step Models

##### Trip Productions

The main aggregate checks of trip generation models are comparisons of aggregate model results, usually trips per household by purpose by various other market segments, to observed data from the local household survey. Market segments may be defined by demographic or geographic characteristics, or any other variables by which model results and the comparison data sources are reported.

If a model has been estimated using local household survey data, the model results can be compared to the results from the expanded household survey data. This is particularly useful if the comparisons are made using different stratifications of the data. For example, if the trip generation model is based on household size and income group, comparing the results of an application using the base year socioeconomic data to the expanded survey results by area type could produce important insights regarding the validity of the model. Such a comparison can help identify errors in the model estimation and errors in the survey expansion (or differences to be checked between the household characteristics during the survey period compared to the model base year). However, problems with the survey data set itself, outside the expansion, might not be identified since they would exist in both the survey data and the models estimated from the data.

[Table 5.1](#Table-t5-1) shows an example home-based nonwork trip production model for a region. Suppose the model was applied to the base year socioeconomic data and the resulting modeled trips by area type were compared to trips from the expanded household survey used to estimate the model. Further, suppose that the modeled productions to the productions from the expanded survey data were as follows:

|               |                                        |
|---------------|----------------------------------------|
| <center>      
 **Area Type**  
                
 </center>      | <center>                               
                 **Ratio Modeled/Expanded Productions**  
                                                         
                 </center>                               |
| CBD           | 1.10                                   |
| Fringe        | 1.05                                   |
| Urban         | 1.03                                   |
| Suburban      | .98                                    |
| Rural         | .95                                    |
| Overall       | .99                                    |

Such results would suggest an area type or density bias that might be corrected to produce an improved trip generation model.

Since, quite frequently, the same data set must be used for estimation and validation, it is a good idea to check the model results against other data sources, such as the national sources. Differences between the trip generation model results and the national data sources should be explainable by distinguishing local characteristics. Such checks are discussed in [Reasonableness and Sensitivity Testing (Trip Generation)](#Reasonableness_and_Sensitivity_Testing_(Trip_Generation)).

<div id="Table-t5-1">
<center>
Table 5.1 Example Home-Based Nonwork Trip Production Model

</center>
</div>
| <center>                   
 **Income Group**            
                             
 </center>                   | <center>           
                              **Household Size**  
                                                  
                              </center>           |
|----------------------------|--------------------|
| <span></span>              | <center>           
                              **1**               
                                                  
                              </center>           |
| Low (Less than \$15,000)   | 1.27               |
| Middle (\$15,000–\$74,999) | 1.38               |
| High (\$75,000 or more)    | 1.59               |

##### Trip Attractions

The types of checks described above are relevant for trip productions since data sources such as the NHTS and local household activity/travel surveys use households as the sampling unit. There are few sources for checks of trip attractions. One check that can be easily done is to compare the number of home-based work attractions to the total employment by zone. Since home-based work attractions include trips both to and from work, summarized at the workplace, one might expect that an upper bound on the ratio of home-based work attractions to employees would be 2.0. ([14](#fn14)) However, there are many reasons for every worker not making two home-based work trips on an average weekday, including the following:

-   Some workers are not scheduled to work on every weekday, because their regular schedules include weekends, flex-time, or part-time work.
-   A percentage of workers are absent on any given weekday, due to vacations, personal days, sick leave, telecommuting, or work-related travel.
-   Any journeys to or from work that include stops on the way are usually considered as combinations of home-based nonwork and nonhome-based trips in most four-step models. (This would not be the case when checking work tour destinations in activity-based models.)

These factors result in the number of home-based work trips per employee being much lower than 2.0. One source ([15](#fn15)) suggests that a reasonable range is between 1.20 and 1.55 home-based work attractions per employee.

**Balancing Trip Productions and Attractions**

In theory, the estimated total trip productions must be equal to the total trip attractions for each trip purpose, since each trip has two ends, a production and an attraction. In model application, however, the estimation of trip productions and attractions will not be exactly equal. This can cause issues with the application of trip distribution models since a doubly constrained model will attempt to match both productions and attractions. While the different trip production and attraction models contribute to the imbalance, much of the difference may be explained by the estimates of the socioeconomic data used in model application.

Before checking the balance between productions and attractions, the effects of nonresidential person travel must be considered. If significantly more people from outside the modeled region work, shop, and perform other activities within the region than residents perform these activities outside, there should be more internal-internal attractions than productions, offset by a corresponding surplus of external trip productions over attractions. This imbalance must be carefully computed since many models use vehicle trips for external travel and person trips for residential travel. (External travel is discussed in [External/Nonresident Travel](#External/Nonresident_Travel).) Another area of imbalance that must be considered is special generators (discussed in [Special Generators](#Special_Generators)). Special generator trips are often dominated by or are exclusively trip attractions – for example, airports generate no home-based productions – and so the effects of these “extra attractions” must be considered before balancing productions and attractions regionally.

Once these effects have been considered, the balance between productions and attractions can be checked for each trip purpose. Assuming that the production and attraction models have been developed from the same data source, the ratio of regionwide productions to attractions by purpose should fall in the range of 0.90 to 1.10 prior to balancing. For the base year, the balance between productions and attractions is, in effect, a validation measure. If there is not a close match, the reasons for the lack of match should be investigated.

##### Activity-Based Models

While the aggregate checks of trip rates described above are directly applicable to the results of four-step models, they can also be performed for activity-based models. For activity-based models, it may be necessary to compile and report results that are not directly generated. Specifically, it should be possible to summarize the tour and intermediate stop information to estimate trips comparable to those used in traditional trip-based models. While this might seem to be a step backward, most regions developing activity-based models have a long history of using trip-based models. If overall regional results in terms of trips per household, trips per person, or the shares of trips by traditional trip purposes are substantially different from those estimated using traditional trip-based models, an investigation of the difference might be warranted.

It is necessary to perform additional checks of activity-based model components. As discussed at the beginning of this section, such models will produce, for each person modeled:

-   Number of activities by purpose;
-   Number of tours by purpose;
-   Number of stops on each tour;
-   Number of work-based subtours; and
-   Joint activity or travel participation (possibly).

These measures can be summarized by market segment (e.g., area type) in a similar manner to the trip rate summaries discussed earlier and compared to local survey data.

Since trip attractions are not directly estimated in activity-based models, there are no checks of “activity attractions” corresponding to trip attraction checks or checks of balancing of productions and attractions at this stage of the modeling process. However, after destination choice modeling and intermediate stop modeling are performed, some tests analogous to trip attraction model checks may be performed. For example, after the application of all tour destination and intermediate stop location choice models, trip tables analogous to trip-based trip tables should be available for processing. It may be possible to aggregate the various tables by purposes similar to those used for trip-based models to summarize “attractions” by purpose. The resulting summaries could be used to estimate implied “trip attraction rates” for some purposes to check the reasonableness of the resulting travel. For example, it might be possible to summarize home-based work half-tours (i.e., those without an intermediate stop on the journey to or from the work location, depending on the direction of the half-tour) by the work zone. The tours could be divided by the total number of employees to estimate the implied trip attractions per employee. For the base year, the implied trip rate should be reasonably close to the trip attraction rate used for trip-based models.

#### Disaggregate Checks (Trip Generation)

The trip generation model forms associated with four-step models, such as cross-classification and linear regression models, are applied aggregately, and so there are no applicable disaggregate checks.

Logit models are disaggregately estimated (one record per person/activity/stop), and therefore disaggregate validation is needed for the logit choice models associated with activity-based models, along with the aggregate checks described above.

Ideally, disaggregate validation of a model should be performed using a data set that is independent of the data set used for model estimation. As discussed above, household activity/travel surveys typically have such small sample sizes that the entire data set is needed for model estimation. In most cases, therefore, there is no independent model estimation data set available for validation.

Limited disaggregate validation can be performed using the same data set used for model estimation, but reporting the results by market segment. Logit model estimation software has the capability to apply the estimated model to a data set in the same form as the estimation data set. For example, a logit model could be applied to the data set used for estimation but the results may be reported by vehicle availability level. It might be found, for example, that certain activity patterns are not being chosen often enough in the model for households with zero vehicles.

#### Criteria Guidelines (Trip Generation)

There are no specific criteria guidelines associated with the trip generation checks described above. While no specific guidelines are associated with trip generation, trip generation is the first basic step in the modeling process; errors and inaccuracies in this step may propagate throughout the modeling process.

#### Reasonableness and Sensitivity Testing (Trip Generation)

The primary reasonableness checks for trip generation models are comparisons of aggregate trip rates to those estimated for other regions. [Table 5.2](#Table-t5-2) shows total person trips per household by trip purpose for different metropolitan area sizes based on the 2001 NHTS. This table is segmented by household size (number of persons in the household). [Table 5.2](#Table-t5-2) provides the opportunity for comparisons of several types of trip production model results, including:

-   Total trips per household;
-   Total trips per household by purpose;
-   Percentage of trips by purpose; and
-   Trips by purpose for household size categories (1, 2, 3, etc.), if the trip generation model is segmented by household size.

Tables 5.3 through 5.5 show the same type of summaries of the 2001 NHTS data, segmented by number of workers, number of vehicles, and income level, respectively.

It should be noted that the data shown in Tables 5.2 through 5.5 are for all person trips, including both motorized (auto, transit) and nonmotorized (walk, bicycle) trips. It is recognized that many models include only motorized trips. To allow for better trip comparisons for these models, [Table 5.6](#Table-t5-6) presents the share of trips that are motorized, by urban area size and trip purpose, from the 2001 NHTS. These percentages can be used to adjust the values in Tables 5.2 through 5.5.

An additional reasonableness check for cross-classification models is to ensure that the rates for individual cells are consistent with one another. This includes checking the following:

-   The direction (increase/decrease) between trip rates in adjacent cells along both dimensions is correct. For example, for home-based work trips, the trip rate should be higher for a greater number of workers, holding the other variable constant. However, caution should be exercised since it may not always be correct that a higher value for a variable will result in an increase in the trip rate. As an example, a two person, one worker household might make more nonwork trips than a two person two worker household.

<div id="Table-t5-2">
<center>
Table 5.2 Trip Rates by Purpose Stratified by Number of Persons by MSA Population

</center>
</div>
|                                                     |                       |                    |
|-----------------------------------------------------|-----------------------|--------------------|
|                                                     | <center>              
                                                       **Number of Persons**  
                                                                              
                                                       </center>              | <center>           
                                                                               **All Households**  
                                                                                                   
                                                                               </center>           |
| &nbsp;                                              | <center>              
                                                       **1**                  
                                                                              
                                                       </center>              | <center>           
                                                                               **2**               
                                                                                                   
                                                                               </center>           |
| <center>                                            
 **Home-Based Work**                                  
                                                      
 </center>                                            |                       |
| <center>                                            
 '''MSA population greater than 3 million '''         
                                                      
 </center>                                            | 0.54                  | 1.45               |
| <center>                                            
 '''MSA population between 1 and 3 million '''        
                                                      
 </center>                                            | 0.56                  | 1.58               |
| <center>                                            
 '''MSA population between 500,000 and 1 million '''  
                                                      
 </center>                                            | 0.51                  | 1.48               |
| <center>                                            
 '''MSA population between 250,000 and 500,000 '''    
                                                      
 </center>                                            | 0.47                  | 1.44               |
| <center>                                            
 '''MSA population less than 250,000 '''              
                                                      
 </center>                                            | 0.51                  | 1.42               |
| <center>                                            
 '''Not in MSA '''                                    
                                                      
 </center>                                            | 0.39                  | 1.35               |
| <center>                                            
 **Home-Based Nonwork**                               
                                                      
 </center>                                            |                       |
| <center>                                            
 '''MSA population greater than 3 million '''         
                                                      
 </center>                                            | 1.58                  | 4.20               |
| <center>                                            
 '''MSA population between 1 and 3 million '''        
                                                      
 </center>                                            | 1.66                  | 4.21               |
| <center>                                            
 '''MSA population between 500,000 and 1 million '''  
                                                      
 </center>                                            | 1.65                  | 4.58               |
| <center>                                            
 '''MSA population between 250,000 and 500,000 '''    
                                                      
 </center>                                            | 1.71                  | 4.39               |
| <center>                                            
 '''MSA population less than 250,000 '''              
                                                      
 </center>                                            | 1.84                  | 4.38               |
| <center>                                            
 '''Not in MSA '''                                    
                                                      
 </center>                                            | 1.59                  | 4.20               |
| <center>                                            
 **Nonhome-Based**                                    
                                                      
 </center>                                            |                       |
| <center>                                            
 '''MSA population greater than 3 million '''         
                                                      
 </center>                                            | 1.24                  | 2.98               |
| <center>                                            
 '''MSA population between 1 and 3 million '''        
                                                      
 </center>                                            | 1.19                  | 3.09               |
| <center>                                            
 '''MSA population between 500,000 and 1 million '''  
                                                      
 </center>                                            | 1.18                  | 2.97               |
| <center>                                            
 '''MSA population between 250,000 and 500,000 '''    
                                                      
 </center>                                            | 1.24                  | 2.99               |
| <center>                                            
 '''MSA population less than 250,000 '''              
                                                      
 </center>                                            | 1.37                  | 3.09               |
| <center>                                            
 '''Not in MSA '''                                    
                                                      
 </center>                                            | 1.18                  | 2.93               |
| <center>                                            
 **All Trip Purposes**                                
                                                      
 </center>                                            |                       |
| <center>                                            
 '''MSA population greater than 3 million '''         
                                                      
 </center>                                            | 3.36                  | 8.63               |
| <center>                                            
 '''MSA population between 1 and 3 million '''        
                                                      
 </center>                                            | 3.41                  | 8.88               |
| <center>                                            
 '''MSA population between 500,000 and 1 million '''  
                                                      
 </center>                                            | 3.34                  | 9.03               |
| <center>                                            
 '''MSA population between 250,000 and 500,000 '''    
                                                      
 </center>                                            | 3.42                  | 8.82               |
| <center>                                            
 '''MSA population less than 250,000 '''              
                                                      
 </center>                                            | 3.76                  | 8.89               |
| <center>                                            
 '''Not in MSA '''                                    
                                                      
 </center>                                            | 3.16                  | 8.48               |

Source: 2001 NHTS.

<div id="Table-t5-3">
<center>
Table 5.3 Trip Rates by Purpose Stratified by Number of Workers by MSA Population

</center>
</div>
|                                                  |                       |
|--------------------------------------------------|-----------------------|
|                                                  | <center>              
                                                    **Number of Workers**  
                                                                           
                                                    </center>              |
| &nbsp;                                           | <center>              
                                                    **0**                  
                                                                           
                                                    </center>              |
| <center>                                         
 **Home-Based Work**                               
                                                   
 </center>                                         |                       |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 0.02                  |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 0.02                  |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 0.01                  |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 0.01                  |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 0.02                  |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 0.02                  |
| <center>                                         
 **Home-Based Nonwork**                            
                                                   
 </center>                                         |                       |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 3.57                  |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 3.62                  |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 3.62                  |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 3.94                  |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 3.86                  |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 3.52                  |
| <center>                                         
 **Nonhome-Based**                                 
                                                   
 </center>                                         |                       |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 1.46                  |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 1.62                  |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 1.38                  |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 1.61                  |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 1.74                  |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 1.64                  |
| <center>                                         
 **All Trip Purposes**                             
                                                   
 </center>                                         |                       |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         |                       |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 5.05                  |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 5.26                  |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 5.01                  |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 5.56                  |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 5.62                  |

Source: 2001 NHTS.

<div id="Table-t5-4">
<center>
Table 5.4 Trip Rates by Purpose Stratified by Number of Autos by MSA Population

</center>
</div>
|                                                  |                     |
|--------------------------------------------------|---------------------|
|                                                  | <center>            
                                                    **Number of Autos**  
                                                                         
                                                    </center>            |
| &nbsp;                                           | <center>            
                                                    **0**                
                                                                         
                                                    </center>            |
| <center>                                         
 **Home-Based Work**                               
                                                   
 </center>                                         |                     |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 0.82                |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 0.47                |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 0.41                |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 0.35                |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 0.58                |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 0.23                |
| <center>                                         
 **Home-Based Nonwork**                            
                                                   
 </center>                                         |                     |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 3.15                |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 2.47                |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 2.53                |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 2.11                |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 1.78                |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 2.29                |
| <center>                                         
 **Nonhome-Based**                                 
                                                   
 </center>                                         |                     |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 1.63                |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 1.19                |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 0.93                |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 0.94                |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 0.85                |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 0.96                |
| <center>                                         
 **All Trip Purposes**                             
                                                   
 </center>                                         |                     |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 5.60                |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 4.13                |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 3.87                |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 3.40                |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 3.21                |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 3.48                |

Source: 2001 NHTS.

<div id="Table-t5-5">
<center>
Table 5.5 Trip Rates by Purpose Stratified by Income Level by MSA Population

</center>
</div>
|                                                  |                                    |
|--------------------------------------------------|------------------------------------|
|                                                  | <center>                           
                                                    **Income Level (in 2000 Dollars)**  
                                                                                        
                                                    </center>                           |
| &nbsp;                                           | <center>                           
                                                    **Missing**                         
                                                                                        
                                                    </center>                           |
| <center>                                         
 **Home-Based Work**                               
                                                   
 </center>                                         |                                    |
| <center>                                         
 '''MSA population greater than 3 million '''      
                                                   
 </center>                                         | 1.11                               |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 0.93                               |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 0.89                               |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 0.94                               |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 0.78                               |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 0.75                               |
| <center>                                         
 **Home-Based Nonwork**                            
                                                   
 </center>                                         |                                    |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 4.38                               |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 3.97                               |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 3.33                               |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 3.88                               |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 3.78                               |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 3.63                               |
| <center>                                         
 **Nonhome-Based**                                 
                                                   
 </center>                                         |                                    |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 2.00                               |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 2.36                               |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 1.81                               |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 2.10                               |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 1.90                               |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 2.18                               |
| <center>                                         
 **All Trip Purposes**                             
                                                   
 </center>                                         |                                    |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 7.49                               |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 7.26                               |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 6.03                               |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 6.92                               |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 6.46                               |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 6.56                               |

Source: 2001 NHTS.

<div id="Table-t5-6">
<center>
Table 5.6 Motorized Trip Percentages by Urban Area Population

</center>
</div>
|                                                  |                     |                        |                   |               |
|--------------------------------------------------|---------------------|------------------------|-------------------|---------------|
|                                                  | <center>            
                                                    **Home-Based Work**  
                                                                         
                                                    </center>            | <center>               
                                                                          **Home-Based Nonwork**  
                                                                                                  
                                                                          </center>               | <center>          
                                                                                                   **Nonhome-Based**  
                                                                                                                      
                                                                                                   </center>          | <center>      
                                                                                                                       **All Trips**  
                                                                                                                                      
                                                                                                                       </center>      |
| <center>                                         
 **MSA population greater than 3 million**         
                                                   
 </center>                                         | 96.3%               | 83.7%                  | 87.8%             | 86.8%         |
| <center>                                         
 **MSA population between 1 and 3 million**        
                                                   
 </center>                                         | 97.4%               | 87.9%                  | 93.5%             | 91.1%         |
| <center>                                         
 **MSA population between 500,000 and 1 million**  
                                                   
 </center>                                         | 97.6%               | 89.6%                  | 95.2%             | 92.5%         |
| <center>                                         
 **MSA population between 250,000 and 500,000**    
                                                   
 </center>                                         | 97.8%               | 89.3%                  | 94.1%             | 92.1%         |
| <center>                                         
 **MSA population less than 250,000**              
                                                   
 </center>                                         | 97.2%               | 89.5%                  | 94.5%             | 92.2%         |
| <center>                                         
 **Not in MSA**                                    
                                                   
 </center>                                         | 97.2%               | 91.1%                  | 94.2%             | 93.0%         |
| <center>                                         
 **All Areas**                                     
                                                   
 </center>                                         | **97.0%**           | **87.3%**              | **92.0%**         | **90.2%**     |

Source: 2001 NHTS.

-   The incremental differences between trip rates in adjacent cells make sense. For example, if household size is one of the variables, the increments between one and two person households, two and three person households, etc., should be reasonable in terms of the additional trips adding a household member would produce.

Sensitivity testing for aggregate trip generation models is not considered to be very useful. Cross-classification models already use separate trip production rates for different levels of the input variables. For example, if one of the input variables is household size, the check of the aggregate trip rates by number of persons in the household (the model results that are compared to the numbers in [Table 5.2](#Table-t5-2)) already show how the model results vary by number of persons. For regression models, the coefficients themselves indicate the sensitivity of trip generation with respect to the input variables.

The logit models used for trip generation in activity-based models are sensitive variables other than socioeconomic characteristics, through the use of logsum terms that represent accessibility. It is therefore possible to conduct tests of the sensitivity of these models to transportation level of service. For example, highway travel times could be increased or decreased by a fixed percentage, and the resulting changes in the number of activities, tours, and stops can be examined.

Generally, speaking, however, trip generation has not been found to be very sensitive to changes in transportation accessibility, beyond the effects of changes in land use and development. Destination, time-of-day, and route choices are much more sensitive to changes in transportation level of service. So a reasonable result might be that changes in trip generation resulting from changes in level of service are small.

#### Troubleshooting Strategies (Trip Generation)

In the past, while checks of trip generation results were relatively uncommon, calibration adjustments to trip rates were often made in response to other system-level validation checks. For example, it was sometimes found that vehicle miles traveled (VMT) from the model were too low compared to observed data from traffic counts. A common response would be to increase trip rates for nonwork travel, on the assumption that nonwork trips were more likely to be underreported in the surveys from which the models were estimated. There seems to be some merit to this claim as survey methods have improved over the years, and fewer trips go unreported. However, there was no direct connection between the underreporting of trips and the shortfall in modeled VMT.

Since there is no independent local data source with which to validate trip generation models, the possible model problems that could be indicated by the checks described in this chapter have to do with discrepancies within the survey data set, between the survey data and the socioeconomic data used to apply the model, and between local data and national sources. [Table 5.7](#Table-t5-7) shows some of the typical issues that might be found from these tests.

<div id="Table-t5-7">
<center>
Table 5.7 Troubleshooting Strategies for Issues with Trip Generation Model Results

</center>
</div>
|                                                                                     |                                                                                              |
|-------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| <center>                                                                            
 **Issue**                                                                            
                                                                                      
 </center>                                                                            | <center>                                                                                     
                                                                                       **Potential Troubleshooting Strategies**                                                      
                                                                                                                                                                                     
                                                                                       </center>                                                                                     |
| 1\. Total trips from base year model results inconsistent with expanded survey data | -   Check survey expansion factors for consistency with model application data               
                                                                                       -   Check for differences in socioeconomic data between survey and base years                 
                                                                                       -   Recheck estimated model parameters                                                        |
| 2\. Trip rates inconsistent across variables in cross-classification model          | -   Recheck inconsistent rates                                                               
                                                                                       -   Check error levels for estimated rates                                                    
                                                                                       -   “Smooth” trip rates by combining cells in cross-classification                            |
| 3\. Model results inconsistent with national sources                                | -   Recheck estimated model parameters                                                       
                                                                                       -   Check for ways in which local travel characteristics differ than national                 
                                                                                       -   Adjust parameters if they seem erroneous                                                  |
| 4\. Imbalance between modeled productions and attractions by trip purpose           | -   Check consistency of survey data with model application data                             
                                                                                       -   Check to ensure that external and special generator trips have been correctly considered  |

#### Forecast Checks (Trip Generation)

Trip generation forecasts should be compared to base year estimates for reasonableness. Specifically, trip or activity generation rates per household or per person for the forecast year should be compared to the base year. For trip-based models, past trends in many areas, as documented in the 1997 FHWA Model Validation and Reasonableness Checking Manual, have shown total trips per person to be increasing over time, albeit at a decreasing rate. The changes in per capita trip rates are probably caused by a number of factors that may or may not be included in the trip generation models, including:

-   Decreasing household sizes since smaller households tend to generate more trips per capita than larger households;
-   Increasing mobility through increasing income or auto ownership; and
-   Increasing activity participation (i.e., less time spent “at home”).

In addition to checking implied per capita trip and activity generation rates, the distributions of trips or activities by purpose should be compared to base year conditions. Again, typical trends in the U.S. have shown an increase in the proportion of nonhome-based travel with commensurate decreases in home-based travel.

For trip-based models, production-attraction balancing factors should also be checked for reasonableness. Large changes from base year factors might suggest an imbalance in socioeconomic forecasts. For example, if home-based work trip attractions had to be substantially scaled downward to match home-based work productions, the forecast employment or workers per household should be reviewed for reasonableness.

Large changes in per capita trip rates or large changes in the proportions of trips by purpose should be carefully reviewed. All changes in per capita trip rates and proportions of trips per purpose should have plausible explanations.

### External/Nonresident Travel

This section deals with personal travel in the modeled region not made by the region’s residents or which enters or leaves the modeled region. Components of this segment of travel include:

-   '''Trips made by the modeled region’s residents which leave/return to the modeled region – '''These trips may be modeled, based on household survey data, as part of the resident trip modeling process, either with a separate “internal-external” trip purpose (or purposes) or combined with other resident internal-internal trips, in which case the external zones are valid choices during trip distribution. Alternately, these trips may be combined with trips made by nonresidents that enter the region and modeled as a separate trip purpose or purposes, based on external cordon survey data. In this case, it is necessary to remove internal-external trips from the household survey data prior to use for the development and validation of the internal-internal models. This travel segment is hereafter referred to as resident internal-external (I‑X).
-   **Trips made by nonresidents entering/leaving the modeled region –** Since information on travel by nonresidents is not included in household surveys, data for estimating and validating models must be obtained elsewhere, often from external cordon surveys. A separate trip purpose (or purposes) is defined, representing the specific trips where these nonresidents enter or leave the modeled region. This travel segment is hereafter referred to as nonresident external-internal (X-I).\
    In most regions, the percentage of trips entering or leaving the modeled region by a mode other than private auto is miniscule. In many models, therefore, most or all external travel is modeled as vehicle trips, rather than person trips. Trip productions and attractions represent vehicle trip ends, and there is no mode choice component applied for these trips. It is necessary in these cases to consider vehicle occupancy when dealing with person trip components (for example, resident I‑X trips from the household survey).\
    It should be noted that trips made to and from the airport by visitors who arrive in the modeled region by air are usually considered to be generated at the airport rather than outside the modeled region, and are not considered external trips. These trips are usually handled by airport modeling procedures (see [Special Generators](#Special_Generators)).\
    Nonresident X-I productions and attractions must be generated for both ends of the trip, the “internal” end of the trip (produced by or attracted to an internal zone within the modeled region) and the external end (produced by or attracted to an external zone). The total number of vehicle trips (resident I‑X, nonresident X-I, and X-X) generated at an external station in the base year is equal to the traffic count at the external station. Generally, this count acts as a control total for the (vehicle) trips generated at the external zone, with the trips categorized by type based on the results of the external cordon survey. When external transit trips are included, the control total (in person trips) is the transit passenger count plus the traffic count multiplied by the vehicle occupancy (from the external cordon survey, or other source).\
    Trip productions and attractions for external trips at internal zones may be generated by separate model components that consider the location of the zone relative to the regional boundary. It is important to ensure that such trips are not “double counted” by internal-internal trip generation models.
-   '''Trips made by nonresidents that have both ends within the modeled region – '''This segment consists of travel made by nonresidents excluding the trip to enter or leave the modeled region. These generally include trips made within the modeled region while the traveler is visiting. These trips are excluded from both household surveys (since the travelers are nonresidents) and external cordon surveys (since the trips do not enter or leave the modeled region). This travel segment is hereafter referred to as nonresident internal-internal (I‑I).\
    Many models do not explicitly model nonresident I‑I trips, simply including them within the resident nonhome-based trips (even though the survey data on which models of these trips are based does not include nonresident trips). Visitor surveys are not commonly conducted except in areas with large numbers of visitors. In some areas, nonresident I‑I trips are modeled as a percentage of nonresident external-internal (X-I) trips. The percentage might be derived from the percentage of nonhome-based trips for residents of the modeled region, based on the household survey data.
-   '''Trips with both ends outside the modeled region that pass through the region – '''These are made by travelers that are not performing any activities within the modeled region but whose travel paths use roadways within the modeled region. This travel segment is hereafter referred to as external-external (X-X).\
    External-external trips are usually modeled using fixed trip tables. Base year trip tables are developed by expanding the X-X trips from external cordon surveys while forecast year trip tables are usually factored from the base year tables.\
    With the exception of resident I‑X trips, activity-based models do not have the data needed to model full activity patterns and tours associated with external trips. It is therefore usual practice to model external travel using a trip-based approach, similar to the approaches used in four-step models. The model validation checks described in this section are therefore relevant to external travel models for both four-step and activity-based models.

#### Sources of Data

There are four major data sources that may be relevant to the modeling and validation of external/nonresident travel:

1.  '''Household activity/travel survey – '''The household survey used for the estimation and validation of the resident person travel models includes all trips made by residents that leave the modeled region.
2.  '''External cordon survey – '''An external cordon survey is conducted either by intercepting and interviewing travelers as they enter or leave the modeled region or by recording license plate information and mailing a survey form. It includes all travelers that pass through the survey location regardless of resident status or the origin and destination of the trip and is usually conducted for each major external station. Only information about the trip that is intercepted or recorded is collected, but information about traveler and trip characteristics is collected (though these surveys often collect less information than household or visitor surveys). In many cases, some external stations, especially those with low volumes, are not surveyed, and information on origins/destinations, external trip types, traveler characteristics, and vehicle occupancy obtained from survey results at other locations.
3.  '''Visitor travel survey – '''This survey is usually conducted where visitors to a region stay overnight (such as hotels) and asks about all travel made by the respondent (and perhaps his/her travel party) within a set period, say the previous 24 hours. A complete set of traveler/trip characteristics is obtained, but the sample is limited to people who are staying at hotels. Trips made by visitors who stay somewhere outside the sampling frame or who do not stay overnight are not included.
4.  **Traffic/passenger counts at the modeled region’s boundary –** Traffic counts at external stations can provide control totals for the number of vehicle trips entering and leaving the modeled region. If a significant number of travelers enter and leave the modeled region via transit, passenger counts at the regional boundary may also be useful in providing control totals for external travel.

[Table 5.8](#Table-t5-8) summarizes how these data sources relate to the four categories of external/nonresident travel.

<div id="Table-t5-8">
<center>
Table 5.8 External/Nonresident Travel Data Sources

</center>
</div>
|                                       |                            |
|---------------------------------------|----------------------------|
|                                       | <center>                   
                                         **Data Source**             
                                                                     
                                         </center>                   |
| <center>                              
 **Household Activity/ Travel Survey**  
                                        
 </center>                              | <center>                   
                                         **External Cordon Survey**  
                                                                     
                                         </center>                   |
| <center>                              
 **Resident I-X**                       
                                        
 </center>                              | Included                   |
| <center>                              
 '''Nonresident X-I '''                 
                                        
 </center>                              |                            |
| <center>                              
 **Nonresident I-I**                    
                                        
 </center>                              |                            |
| <center>                              
 **External-external**                  
                                        
 </center>                              |                            |

<div id="t5-8_a">
a&nbsp;Traffic/passenger counts include these trips, but do not separate them into their component categories and include no information on traveler or trip characteristics.

</div>
\

#### Aggregate Checks (External Models)

Because both traffic (and perhaps transit passenger) count data and external cordon survey data (where available) are used in the estimation of external travel models, there are likely no independent data sources with which to validate these models. The main checks include ensuring consistency with the model estimation data. These checks include the following:

-   Comparing total modeled base year vehicle trips (including resident I-X, nonresident X-I, and X-X) trips to the base year traffic count for each external station. Caution should be exercised in considering that traffic counts may include trucks, which are modeled separately (see [Commercial Vehicle and Freight Travel](#Commercial_Vehicle_and_Freight_Travel)). The best approach is to compare the vehicle trips associated with external/nonresident passenger travel to the traffic count excluding trucks, and to compare separately the truck model results with the truck count.
-   Comparing total implied trip rates, including all internal and external passenger travel, across zones. The implied trip rates are the total person trip productions (internal and external) per household and total person trip attractions per employee. Particular attention should be paid to comparing implied trip rates for zones located near the modeled region boundary and interior zones. Because models should generate more external travel for outlying zones, this check will ensure that these additional external trips were not “double counted” along with resident internal-internal trips. A corresponding check is the percentage of total generated person trips that are external, which should be higher for outlying zones.

#### Disaggregate Checks (External Models)

There are no applicable disaggregate checks of external travel models.

#### Criteria Guidelines (External Models)

There are no applicable criteria guidelines for checks of external travel models.

#### Reasonableness and Sensitivity Testing (External Models)

The reasonableness checks for external travel models are mainly the aggregate checks presented in [Aggregate Checks (External Models)](#Aggregate_Checks_(External_Models)).

#### Troubleshooting Strategies (External Models)

[Table 5.9](#Table-t5-9) shows some typical issues with external travel model results and suggested strategies for dealing with them.

#### Forecasting Checks (External Models)

Forecast internal-external and external-external travel should be compared to base year for reasonableness. Growth rates in travel can be compared to growth rates for internal person trips, and significant differences should be explainable using demographic forecast data.

<div id="Table-t5-9">
<center>
Table 5.9 Troubleshooting Strategies for Issues with External Travel Model Results

</center>
</div>
|                                                                                                                                               |                                                                                                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|
| <center>                                                                                                                                      
 **Issue**                                                                                                                                      
                                                                                                                                                
 </center>                                                                                                                                      | <center>                                                                                                       
                                                                                                                                                 **Potential Troubleshooting Strategies**                                                                        
                                                                                                                                                                                                                                                                 
                                                                                                                                                 </center>                                                                                                       |
| 1\. Total vehicle trips for each external station for base year model inconsistent with the corresponding traffic count                       | -   Check traffic count data for errors, seasonal adjustment, and adjustment between the count and model years 
                                                                                                                                                 -   Check to ensure that truck trips are excluded from counts when comparing to passenger trips from the model  
                                                                                                                                                 -   Make sure X-X trips are not double counted                                                                  
                                                                                                                                                 -   Recheck control totals estimated from the original counts                                                   |
| 2\. Total implied trip rates including both internal and external travel significantly higher or lower for zones near modeled region boundary | -   Check to ensure that trips are not double counted – trips are modeled as external or internal, not both    |
| 3\. Zones near modeled region boundary have lower percentage of external trips than interior zones                                            | -   Check sensitivity of trip generation model to distance from the modeled region boundary                    |

### Commercial Vehicle and Freight Travel

There are a variety of ways in which freight, trucks, and other commercial vehicles are considered in travel models. These include:

-   Commodity flow models, where freight movements are estimated by commodity type and converted to truck vehicle trips (and perhaps trips by other freight modes);
-   Truck vehicle trip models, usually consisting of truck trip generation and distribution models;
-   Factoring of nonhome-based trips; and
-   Not explicitly considering truck travel separately.

The latter two methods, of course, are not based on actual data on truck or freight movements and are not recommended. They may be found in many older models or where no local data are available.

Commodity flow models are often found in connection with models of larger regions such as statewide models. Freight flows often cover long distances, and modeling freight for an urban area would mean that a large percentage of the freight modeled is external to the region.

In commodity flow models, the tonnage of freight (either by all modes or only by truck) is estimated using input variables of employment by type and households. The employment types for these models are often more disaggregate than those used in person trip attraction models. These models are often linear regression models, similar in form to person trip attraction models. Normally, one set of regression equations for the production end and one set of regression equations for consumption end are estimated. These regression equations are either developed for each commodity group or type. The outputs of this tonnage generation process are tons of each commodity produced and consumed for each zone.

Following tonnage generation, a tonnage distribution model is run, often a gravity model similar to those used for person trip distribution (see [Distribution](Model_Validation_and_Reasonableness_Checking_Distribution)). If multimodal freight tonnage has been generated, a mode choice step follows, where the tonnage tables of freight that are the outputs of tonnage distribution are split into tons by mode (truck, rail, water, air, etc.). Finally, a process to convert tons of truck freight to truck vehicle trips is applied, resulting in truck vehicle trip tables that may be used in the highway assignment process. Truck trips are often modeled by vehicle size category. An example categorization is:

-   Light trucks (four-tire);
-   Medium trucks (single unit/6+ tire); and
-   Heavy trucks (combinations).

It should be noted that there are many trucks that are not carrying freight, and it may be necessary to add these to the freight-carrying truck trips generated by a commodity flow model.

Truck vehicle trip models use truck trip generation equations, which are also usually linear regression models with employment by type and number of households as the independent variables. Truck trip distribution models usually use the gravity model formulation. Truck vehicle trip models are also often segmented by vehicle size category.

There are several other types of commercial vehicles that may be present in modeled regions. These types of commercial vehicles are seldom modeled explicitly although a few models, mainly in large urban areas, do specifically consider taxi trips. A good source for information on commercial vehicle travel is Cambridge Systematics et al, 2004. ([16](#fn16))

#### Sources of Data (Truck Models)

The main sources of data for truck/freight model validation include the following:

-   **Local truck/commercial vehicle survey –** If such a survey is available, it is likely to have been the data source for truck/freight model estimation. It is the best source for information on local origin-destination travel data for truck trips. However, such surveys are relatively uncommon.
-   **Public/commercial freight data sources –** These include such data sources as the Commodity Flow Survey (CFS), the Freight Analysis Framework (FAF), and TRANSEARCH.
-   **Commodity Flow Survey –** The CFS is undertaken as part of the Economic Census through a partnership between the U.S. Census Bureau, U.S. Department of Commerce, and the Bureau of Transportation Statistics (BTS), U.S. Department of Transportation. The survey is undertaken approximately every five years, most recently in 2002 and produces data on the movement of goods in the United States. It provides information on commodities shipped, their value, weight, and mode of transportation, as well as the origin and destination of shipments of manufacturing, mining, wholesale, and select retail establishments. The CFS is available on a CD from BTS.
-   '''Freight Analysis Framework – '''The FAF, available from the FHWA, integrates data from a variety of sources to estimate commodity flows and related freight transportation activity among states, regions, and major international gateways. The original version, FAF1, provides estimates for 1998 and forecasts for 2010 and 2020. The more recent version, FAF2, provides estimates for 2002 and the most recent year plus forecasts through 2035.
    -   TRANSEARCH is a freight database that is available commercially from Global Insight. The databases had previously been available from Reebie Associates before they were acquired by Global Insight, and the database is often referred to as “Reebie” data. TRANSEARCH uses a multitude of mode-specific data sources to create a picture of the nation’s freight traffic flows on a market-to-market commodity basis. The national database uses counties as the primary flow unit although TRANSEARCH can also use proprietary data to provide a more disaggregate level of geography. Each record in the TRANSEARCH database records the flow from an origin zone to a destination zone.
-   **Other national sources –** National data sources include the *Quick Response Freight Manual II* ([17](#fn17)) and its predecessor report the *Quick Response Freight Manual*. ([18](#fn18)) These reports provide parameter values from other truck/freight models as well as information on other data sources.
-   **Vehicle classification counts –** Vehicle classification counts that specify the numbers of trucks by vehicle size category used in the model are critical data needed for validation of truck travel models.

#### Aggregate Checks (Truck Models)

If commercial vehicle or freight models have been developed from local survey data, aggregate checks analogous to those specified for trip generation models might be possible. For example, estimated total truck trips from the model could be compared to truck trips from the expanded truck survey.

Because of the relative lack of local data on truck and freight movements, the main check of truck/freight models cannot really occur until the highway assignment stage, when modeled truck volumes can be compared to vehicle classification traffic counts. If modeled truck volumes are too high (or low) compared to observations, this likely means that the trip/tonnage generation rates are too high (or low), or the truck trip lengths are too long (or short). Vehicle classification counts cannot distinguish full versus empty trucks, freight versus nonfreight related commercial vehicle movements, or intraregional versus interregional truck movements. Thus, the vagaries associated with vehicle classification traffic counts make validation of truck trip generation models after traffic assignment very coarse.

Truck and freight movements can vary significantly depending on geographic, economic, and land use characteristics of an area. It is therefore difficult to determine typical truck travel parameters for areas based on national data sources. The average values provided in these sources may differ significantly from those found in individual areas.

#### Disaggregate Checks (Truck Models)

There are no applicable disaggregate checks of truck/freight models.

#### Criteria Guidelines (Truck Models)

There are no applicable criteria guidelines for checks of truck/freight models.

#### Reasonableness and Sensitivity Testing (Truck Models)

If truck/freight models have been developed using locally collected survey data, the resulting models can be compared to national sources identified in [Sources of Data (Truck Models)](#Sources_of_Data_(Truck_Models)). Otherwise, the primary reasonableness checks for truck/freight models are the comparisons to vehicle classification traffic counts, as discussed in [Aggregate Checks (Truck Models)](#Aggregate_Checks_(Truck_Models)).

#### Troubleshooting Strategies (Truck Models)

As implied in [Aggregate Checks (Truck Models)](#Aggregate_Checks_(Truck_Models)), the calibration strategies for truck/freight models are adjustments to truck model parameters to address significant differences between modeled truck volumes and vehicle classification traffic counts.

#### Forecasting Checks (Truck Models)

Forecast truck/freight travel should be compared to base year for reasonableness. For example, overall numbers of truck trips per employee in the modeled region might be compared for forecast and based years. Also, after the traffic assignment step, the regional truck VMT to total VMT for the modeled region should be compared for reasonableness.

### Special Generators

The term “special generators” refers to specific locations where the trip generation models used for resident internal-internal travel do not accurately estimate the amount of travel generated. These are typically locations that generate high travel demand where typical measures of trip attraction, such as employment and households, are low compared to the demand generated. Typical special generators may include:

-   Airports;
-   Universities and colleges;
-   Recreational attractions;
-   Casinos;
-   Military bases and establishments;
-   Hospitals; and
-   Regional shopping centers/malls (usually in smaller modeled regions with few of these locations).

Typically, the estimated demand for each special generator is asserted outside the trip generation process. The demand estimates may be developed from separate person or vehicle counts or from surveys or from data from similar locations within or outside the modeled region. Once the trip ends are estimated, the trips generated by special generators are considered trip productions and attractions for the zones in which the special generators are located, and the productions and attractions are balanced (in four-step models). These trips are then considered through the remainder of the modeling process.

Many special generators are atypical not only in the amount of travel demand generated relative to variables typically used in trip generation models, but also in their trip distribution, mode choice, and time-of-day characteristics. In such cases, it is preferable to conduct surveys of travelers to the special generators to develop separate models for these components. In effect, the special generators are treated as separate trip purposes. For example, many models have reduced the need for special generators by modeling home-based university and airport trips as separate trip purposes. However, it is often infeasible to collect such survey data, due to the expense or the difficulty in obtaining permission to survey at privately owned facilities.

#### Sources of Data (Special Generators)

The main sources of data for special generator model estimation and validation include:

-   Special generator traveler survey, as described above; and
-   **Traffic or person trip counts** at or near the special generator location.

#### Aggregate Checks (Special Generators)

If counts of trips to/from the special generator are available, the trips generated by the model can be compared to these counts. If such counts are unavailable, it may be possible to conduct traffic counts on nearby roadways leading or adjacent to the special generator, and highway assignment results on these roadways can be compared to the counts.

#### Disaggregate Checks (Special Generators)

There are no applicable disaggregate checks of special generator models.

#### Criteria Guidelines (Special Generators)

There are no applicable criteria guidelines for checks of special generator models.

#### Reasonableness and Sensitivity Testing (Special Generators)

The reasonableness checks for special generator travel models are the comparisons to traffic or person trip counts, as discussed in [Aggregate Checks (Special Generators)](#Aggregate_Checks_(Special_Generators)).

#### Troubleshooting Strategies (Special Generators)

Since the demand levels for special generators are asserted, it is a relatively simple matter to adjust these demand levels to address any significant discrepancies between the modeled trips/volumes and the count data described in [Sources of Data](#Sources_of_Data_(Special_Generators)) and [Aggregate Checks (Special Generators)](#Aggregate_Checks_(Special_Generators)).

#### Forecasting Checks (Special Generators)

Forecast special generator trips should be compared to base year special generator trips for reasonableness. It is important to stratify special generator trips into those expected to increase over time versus those that are expected to remain relatively static. For example, special generator trips for universities and colleges, military establishments, and hospitals might be expected to remain relatively static unless enrollment, troop levels, or numbers of beds are forecasted to change. Conversely, special generator trips to recreational attractions such as parks or open space or to regional shopping centers might be expected to grow with the population of the region even if the basis for the special generator remains unchanged.

------------------------------------------------------------------------

<div id="fn13">
13&nbsp;Cross-classification is actually a specific form of linear regression where the effects of independent variables (vehicle availability, household size, etc.) are allowed to have a general nonlinear effect. An equivalent linear regression formulation would have appropriately defined dummy variables to represent the effect of each combination value of the independent variables.

</div>
<div id="fn14">
14&nbsp;Cases of workers making more than one round trip between home and work on the same day do occur but are relatively rare. There are far fewer cases than those of the workers not making home-based work trips described later in the paragraph.

</div>
<div id="fn15">
15&nbsp;Cambridge Systematics, Inc., *FSUTMS-Cube Framework Phase II – Model Calibration and Validation Standards: Model Validation Guidelines and Standards*, prepared for Florida Department of Transportation Systems Planning Office, 2008.

</div>
<div id="fn16">
16&nbsp;Cambridge Systematics, Inc., A. Chatterjee, and H. Cohenm, *Accounting for Commercial Vehicles in Urban Transportation Models*, prepared for the Federal Highway Administration, Washington, D.C., 2004.

</div>
<div id="fn17">
17&nbsp;Beagan, D., M. Fischer, and A. Kuppam, *Quick Response Freight Manual II*, Publication No. FHWA-HOP-08-010, prepared by Cambridge Systematics, Inc., for the Federal Highway Administration, September 2007.

</div>
<div id="fn18">
18&nbsp;*Quick Response Freight Manual*, prepared by Cambridge Systematics, Inc., Comsis Corporation, and the University of Wisconsin-Milwaukee, for the Federal Highway Administration, September 1996.

</div>

------------------------------------------------------------------------

