Felix Buchholz
Parsons School of Design, Data Visualization
Machine Learning, Spring 2019
Instructor Aaron Hill
Assignment 3

#### [See the result here](https://felixbuchholz.github.io/ml-cluster-uncertainty/)

# Clustering artworks by visual qualities of uncertainty


With the open-ended character of this assignment ([see instructions here](https://github.com/visualizedata/ml/tree/master/ML_assignment_3/option_2)), I decided to try and cluster the artworks by the visual qualities of uncertainty they express, because the dataset was created with that intention and is most unique in that way. I didn’t want to cluster the works by medium, genre or date, since these seemed the more obvious criteria. Early exploration was rewarding so I mainly experimented with the selection of variables and number of clusters.

In regards to the number of clusters I settled between my own minimum and maximum with 20 clusters some visual similarities were exhaustive in some clusters but others felt too broad. At the upper 

Choosing variables I excluded the boolean indicators ([ – see the original description of the variables here](https://github.com/visualizedata/ml/blob/master/ML_assignment_3/option_2/contents-of-cluster_images.csv)). For example whether an artwork was a map or representative, so the clustering would be restricted to the visual expressions only. 


### Here’s an overview of the variables I used
| variable | explanation                                                                                                                                                                                  |
|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| pl       | given location on the planar dimensions                                                                                                                                                      |
| si       | variations in height, width, area                                                                                                                                                            |
| va       | the various degrees between white and black                                                                                                                                                  |
| te       | variation in the fineness or coarseness of an area having a given value; includes blur                                                                                                       |
| co       | hue, using the repertoire of colored sensations which can be produced at equal value                                                                                                         |
| or       | various orientations, ranging from the vertical to the horizontal in a distinct direction                                                                                                    |
| po       | A POINT represents a location on the plane that has no theoretical length or area. This signification is independent of the size and character of the mark which renders it visible.         |
| li       | A LINE signifies a phenomenon on the plane which has measurable length but no area. This signification is independent of the width and characteristics of the mark which renders it visible. |
| ar       | An AREA signifies something on the plane that has a measurable size. This signification applies to the entire area covered by the visible mark.                                              |

### Implementation

For the implementation I built on the starter code and what we discussed in class. I consulted the silhouette graphs – but also had the feeling that looking at the clusters would be the most helpful so I tried to organize them on a website to allow for quick quality control and also making my own comments on clusters.
[See the final code here](https://github.com/felixbuchholz/ml-cluster-uncertainty/blob/master/cluster.ipynb)
[– and again the website with the clusters](https://felixbuchholz.github.io/ml-cluster-uncertainty/)
