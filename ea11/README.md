# Decision Trees Exercise

Do the exercise at the and of the LE. You can do the second part also in R if you want.
But somehow the results of the second part should be printable.
Again best you upload a PDF or the ref to Github or a Jupyter Notebook where everything can be seen with a minimum of clicks!

## Excercises DET

1. Find some data [here](https://drive.google.com/open?id=1E3bFrHnMGGmBgyAk9vAVnHGpQ8Z_asOP) on people. The goal is to decide if someone buys a computer or not. Derive the best decision tree by calculating a little by hand (Shannon). At least the first split.

2. Check your tree against the tree derived from SciKit Learn as given in the Python example before! Print the tree with Graphviz (can be easily done with [WebGraphViz](http://www.webgraphviz.com/))

## Result DET

### 1. Calculating

| Rec | Age   | Income | Student | Credit_ratin | Buys_computer |
|-----|-------|--------|---------|--------------|---------------|
| r1  | <=30  | High   | No      | Fair         | No            |
| r2  | <=30  | High   | No      | Excellent    | No            |
| r3  | 31-40 | High   | No      | Fair         | Yes           |
| r4  | >40   | Medium | No      | Fair         | Yes           |
| r5  | >40   | Low    | Yes     | Fair         | Yes           |
| r6  | >40   | Low    | Yes     | Excellent    | No            |
| r7  | 31-40 | Low    | Yes     | Excellent    | Yes           |
| r8  | <=30  | Medium | No      | Fair         | No            |
| r9  | <=30  | Low    | Yes     | Fair         | Yes           |
| r10 | >40   | Medium | Yes     | Fair         | Yes           |
| r11 | <=30  | Medium | Yes     | Excellent    | Yes           |
| r12 | 31-40 | Medium | No      | Excellent    | Yes           |
| r13 | 31-40 | High   | Yes     | Fair         | Yes           |
| r14 | >40   | Medium | No      | Excellent    | No            |
| r15 | <=30  | Medium | No      | Excellent    | No            |
| r16 | <=30  | Low    | No      | Fair         | No            |
| r17 | <=30  | Low    | No      | Excellent    | No            |
| r18 | 31-40 | Low    | Yes     | Fair         | Yes           |
| r19 | >40   | Medium | Yes     | Excellent    | Yes           |
| r20 | 31-40 | High   | No      | Excellent    | Yes           |

#### Formula
Information entropy
Also called Shannon entropy (after the father of intromation theory)

Usually information entropy is denoted as $H$

$H$ is defined as the weighted average of the self-information of all possible outcomes


$H(X) = \sum\limits_{i=1}^N p_i \cdot I(p_i) = -\sum\limits_{i=1}^N p_i\cdot\log(p_i)$


Lets consider two case scenario with $P = (p, 1 - p)$, so entropy is given by $H = -p \log(p) - (1 - p) \log(1 - p)$
1. E(D)    = -(p<sub>t</sub>)*log<sub>2</sub>*p<sub>t</sub>%20-%20p<sub>f</sub>*log<sub>2</sub>*p<sub>f</sub>
<img src="http://www.sciweavers.org/tex2img.php?eq=H%28X%29%20%3D%20%5Csum%5Climits_%7Bi%3D1%7D%5EN%20p_i%20%5Ccdot%20I%28p_i%29%20%3D%20-%5Csum%5Climits_%7Bi%3D1%7D%5EN%20p_i%5Ccdot%5Clog%28p_i%29&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="H(X) = \sum\limits_{i=1}^N p_i \cdot I(p_i) = -\sum\limits_{i=1}^N p_i\cdot\log(p_i)" width="297" height="53" />

2. G(D, A) =

#### Result Table

|               | buying | not buying | total  | E(D)      | G(D,A) |
|---------------|--------|------------|--------|-----------|--------|
| **Age**       |        |            |        |           |        |
| <=30          | 2      | 6          | 8      | 0,811278  |        |
| 31-40         | 6      | 0          | 6      | 0         |        |
| >40           | 4      | 2          | 6      | 0,918295  |        |
| **Income**    |        |            |        |           |        |
| high          | 3      | 2          | 5      | 0,97095   |        |
| medium        | 5      | 3          | 8      | 0,954434  |        |
| low           | 4      | 3          | 7      | 0,985228  |        |
| **Student**   |        |            |        |           |        |
| yes           | 8      | 1          | 9      | 0,5032583 |        |
| no            | 4      | 7          | 11     | 0,9456603 |        |
| **Credit-r.** |        |            |        |           |        |
| excellent     | 5      | 5          | 10     | 1         |        |
| fair          | 7      | 3          | 10     | 0,8812908 |        |
