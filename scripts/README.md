# Note on threshold value

During the model validation stage, it was shown that the model performs best when the threshold value is set to 9. Recall that this value is a rating, where ratings range from 1 to 10. This means that the vast majority of wine recommendations for each user will be filtered out. Setting the threshold value this high means that the system may not actually be able to recommend 3 wines from each of 3 varietals. 

In order for each user to be given more recommendations, the threshold value needs to be lowered to 8 or 7. This shouldn't affect the performance of the current system too much; wines are still choosen from the most recommendated varietals. 

The systems will attempt to provide 3 wine recommendations for each of the 3 most recommended varietals, making a total of 9 recommendations for each user. If it can't do that, then it will provide the 5 top rated red wines and the 5 top rated white wines. However, having set the threshold to 7, the system will be able to provdie wines by varietals.

Lastly, by setting the threshold value to 7, it should also be able to recommend more than 3 wines from each of the top 3 or 4 or 5 varietals. However, please note that this will require experimentation. 
