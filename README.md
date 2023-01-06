# Simple-Voting-Scheme
#### Simple Voting Scheme

Write a Python program that reads a file containing votes indicated by name of candidate, one per line, and counts and declares the winner (candidate with most number of votes). If there is a tie for first place, all candidates are declared the winner. Here are the contents of a possible input file and a sample run of the program:
<pre>
mirage:02-vote raj$ more vote1.dat 
Red
Blue
Green
Blue
Blue
Red
mirage:02-vote raj$ python3 Vote1.py vote1.dat 
Votes:  ['Red', 'Blue', 'Green', 'Blue', 'Blue', 'Red']
Winner:  Blue
</pre>

Here is an example with a tie for first place:
<pre>
mirage:02-vote raj$ more vote1.dat 
Red
Blue
Green
Blue
Blue
Red
Red
mirage:02-vote raj$ python3 Vote1.py vote1.dat 
Votes:  ['Red', 'Blue', 'Green', 'Blue', 'Blue', 'Red', 'Red']
Winner:  Blue
Winner:  Red
</pre>

Build your solution by implementing the following functions:
<pre>
# This function takes as input a list of ballots and 
# returns a list of candidates mentioned in the ballots
# e.g. candidates(["Red","Blue","Red","Green","Red"]) should return ["Red","Blue","Green"]
def candidates(ballots):
  pass

# This function takes as input a candidate and a list of ballots and
# returns the number of votes candidate received in ballots
# e.g. voteCount("Red",["Red","Blue","Red","Green","Red"]) should return 3
def voteCount(candidate,ballots):
  pass

# This function takes as input a list of candidates and a lits of ballots and
# returns a list of vote counts for each candidate as shown in example below:
# e.g. voteCounts(["Red","Blue","Green"],["Red","Blue","Red","Green","Red"]) 
# should return [(3,"Red"),(1,"Blue"),(1,"Green")]
def voteCounts(candidates,ballots):
  pass

# This function takes the vote counts as generated as in previous function as input and
# returns list of winners.
# e.g. winners([(3,"Red"),(1,"Blue"),(1,"Green")]) should return ["Red"]
def winners(voteCounts):
  pass

# Main function that reads input from file and uses the above functions to determine
# winners and print them
def main():
  pass
  </pre>
