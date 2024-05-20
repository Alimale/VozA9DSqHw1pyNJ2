# NLP project


# Data Description:

The data comes from our sourcing efforts. We removed any field that could directly reveal personal details and gave a unique identifier for each candidate.

Attributes: id : unique identifier for candidate (numeric) job_title : job title for candidate (text) location : geographical location for candidate (text) connections: number of connections candidate has, 500+ means over 500 (text) Output (desired target): fit - how fit the candidate is for the role?
(numeric, probability between 0-1) Keywords: “Aspiring human resources” or “seeking human resources”

# Project description:

Assuming that we were able to list and rank fitting candidates, we then employ a review procedure, as each candidate needs to be reviewed and then determined how good a fit they are through manual inspection. This procedure is done manually 
and at the end of this manual review, we might choose not the first fitting candidate in the list but maybe the 7th candidate in the list. If that happens, we are interested in being able to re-rank the previous list based on this information. This supervisory signal is going to be supplied by starring the 7th candidate in the list. Starring one candidate actually sets this candidate as an ideal candidate for the given role. Then, we expect the list to be re-ranked each time a candidate is starred.
