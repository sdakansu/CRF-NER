# CRF-NER
Conditional Random Fields

## Labelling
Label format is an important step to do. There are several different labellings.
IO (Inside-Outside) tagging is easy, if the word is a named entity, it is tagged as I-xxx, ortherwise O.
IOB (Inside-Outside-Beggining) tagging is extended version of IO tagging. The beggining word of the named entity is
tagged as B-xxx and following words of the entity are tagged as I-xxx. Other words are tagged as O (O for out).

Example: 
Türkiye       --> B-ORG                                                             
Cumhuriyeti   --> I-ORG                                                                
1923          --> O                                                                                     
yılında       --> O                                                                       
kurulmuştur.  --> O                                                                             
İlk           --> O                                                                   
cumhurbaşkanı --> O                                                                                   
Mustafa       --> B-PER                                                                       
Kemal         --> I-PER                                                                                                           
Atatürk'tür.  --> I-PER                                                                                   
Başkenti      --> O                                                                      
Ankara'dır.   --> B-LOC                                                                                                                           


**CRF features:**     
* Root (Stem)                                                                                                                                                           
* Part-of-Speech (POS)                                                                                                                                                           
* Proper Noun (PROP)                                                                                                
* Noun Case (NCS)                                                                                               
* Orthographic Case (OCS)                                                                                                                      
* All Inflectional Features (INF)                                                                                                                  
* Start of the Sentence (SS)                                                                        


## Result 
**F1 Scores**                                                                                                                 
CRF1 --> 0.8485571904592357                                                                                                                                               
CRF2 --> 0.8402884363601334                                                                                           
CRF3 --> 0.8467095943830918                                                                                                               
CRF4 --> 0.8105135631724366                                                                                                       
CRF5 --> 0.845174444670488                                                                                        
Average --> 0.8382486458090771                                                                                    

