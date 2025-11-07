# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:

<img width="638" height="951" alt="image" src="https://github.com/user-attachments/assets/a8de91a1-9364-44f3-adde-ea761ce76976" />

<img width="433" height="947" alt="image" src="https://github.com/user-attachments/assets/2628b790-ffef-4b38-9e9f-0f997e287a4f" />

<img width="342" height="936" alt="image" src="https://github.com/user-attachments/assets/7eff2bb7-2480-49f7-a666-9dd9c5e97f09" />


## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num=[1];
den=[1 15 50 0];
sys=tf(num,den);
rlocus(sys);
[k,poles]=rlocfind(sys)
```

## Output:
<img width="692" height="587" alt="image" src="https://github.com/user-attachments/assets/848495d1-21d2-4456-814c-62bded8b799c" />

<img width="236" height="290" alt="image" src="https://github.com/user-attachments/assets/81999bd6-9bd5-4bb6-877a-484c343e65a5" />

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 0 < k < 753.1393
