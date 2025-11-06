# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![IMG-20251106-WA0008](https://github.com/user-attachments/assets/2db664d7-adbc-44d0-bea2-673c3940f8fc)

![IMG-20251106-WA0003](https://github.com/user-attachments/assets/7f68634d-c42f-4e1f-a112-05a1d6c83004)

![IMG-20251106-WA0005](https://github.com/user-attachments/assets/61838916-b344-47d0-82d5-d3cab38eef7a)

![IMG-20251106-WA0010](https://github.com/user-attachments/assets/2baaa87e-d31c-4173-bef4-bc266a425d25)



## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
    num = [1];
    den = [1 15 50 0];
    sys = tf(num,den);
    rlocus (sys);
    [k poles] = rlocfind(sys);

## Output:
<img width="701" height="875" alt="Screenshot_2025-11-05_090038 1" src="https://github.com/user-attachments/assets/6505fc9f-cc47-405d-8ce4-2154bf55fd9e" />


## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 0 < k < 794.6398
