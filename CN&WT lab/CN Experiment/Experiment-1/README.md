# Experiment 1

## Aim of the Experiment
  To implement data link layer framing method character count. 
  i. character count ii. character stuffing and iii. Bit stuffing
  
### Step by step procedure of Experiment
1. First scan the number of frames required.
2. Scan the frames.
3. Find the string length of each frames.
4. Print the frames at Sender.
5. Print the Data Transmitted.
6. Print the frames at Receiver.


### Bit stuffing 

1.Bit stuffing is the insertion of non information bits into data. 
2.The stuffed bits should not be confused with overhead bits.
3.Use the two-character sequence 01111110  to signal the beginning of a frame, and the sequence 01111110 to flag the frame's end.
4.Use character stuffing within the frame. 
5.Replace every occurrence of 11111 with the 0

### character stuffing
1.Use the two-character sequence DLE STX (Data Link Escape, Start of TeXt) to signal the beginning of a frame, and the sequence DLE ETX (End of TeXt) to flag the frame's end.
2.Use character stuffing within the frame.
3.Replace every occurrence of DLE with the two-character sequence DLE DLE.
4.The receiver reverses the processes, replacing every occurrence of DLE DLE with a single DLE.

### Output

#### character count:

![output](Charactercount.png)

#### Bit stuffing:

![output](bitstuffing.png)

#### character stuffing:

![output](Character_stuffing.png)

