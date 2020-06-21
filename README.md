A person named ram .He used to go to a different temples daily therefore today he visited a temple which consist a puzzle .The puzzle was there are three temples with a pond in front of each temple .the person who want to get inside the temple should bring “n” flowers as input.
The condition is ram need to take bath in the pond in front of temple at that time flowers get doubled (eg if it is 5 means it changed to 10).ram needs to put the same “m” (m >= (input*2)) flowers from “n” flowers to the god for all the three temple (n-m) now n becomes the remaining of n=(n-m) for the second temple same to the next temple.
Ram should visit all the three temples and also take bath in all three ponds .Hence, at last ram consists zero flowers in his hand.(puzzle completed) else puzzle not completed.

Constraints:
1<=n<=100000

Formula :
n = (n*2)-m

Sample testcase1:
595  explanation((((((7*2)-8)*2)-8)*2)-8)==0

Output:
Completed

Sample 2:
5 explanation((((((5*2)-6)*2)-6)*2)-6)==-2 ,therefore m value can be taken from 1 to 10

Output:
Incompleted

Sample 3:
7

Output:
Completed

Sample 4:
59

Output:
Incompleted

Sample 5:
280

Output:
Completed

Code:
n=int(input())
flag=False
for m in range(1,(n*2)+1):
    c=((((((n*2)-m)*2)-m)*2)-m)
    if c==0:
        flag=True
        break
    else:
        continue
if flag:
    print('Completed')
else:
    print('Incompleted')






