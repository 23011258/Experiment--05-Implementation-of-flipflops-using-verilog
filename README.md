### NAME : CHANDANA YENDLURI
### REG NO : 23011258
### Experiment 05:Implementation of flipflops using verilog
## AIM:
To implement all the flipflops using verilog and validating their functionality using their functional tables

## Equipments Required:
 HARDWARE REQUIRED:– PC, Cyclone II , USB flasher
 SOFTWARE REQUIRED: Quartus prime
## THEORY
## SR Flip-Flop
SR flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, SR latch operates with enable signal. The circuit diagram of SR flip-flop is shown in the following figure.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/1e8ec93a-a7d3-46e3-aa6a-6a092f8b4b98)


This circuit has two inputs S & R and two outputs Qtt & Qtt’. The operation of SR flipflop is similar to SR Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of SR flip-flop.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/d2145754-fbaa-446e-9751-7da28835a09f)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, SR flip-flop can be used for one of these three functions such as Hold, Reset & Set based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of SR flip-flop. Present Inputs Present State Next State

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/cf1229b1-dc37-4671-9f0a-b678ab451fe5)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. The three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/87fa0a9d-21f1-4233-8c29-2b3e94a45d18)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=S+R′Q(t)Q(t+1)=S+R′Q(t)

## D Flip-Flop
D flip-flop operates with only positive clock transitions or negative clock transitions. Whereas, D latch operates with enable signal. That means, the output of D flip-flop is insensitive to the changes in the input, D except for active transition of the clock signal. The circuit diagram of D flip-flop is shown in the following figure.

This circuit has single input D and two outputs Qtt & Qtt’. The operation of D flip-flop is similar to D Latch. But, this flip-flop affects the outputs only when positive transition of the clock signal is applied instead of active enable. The following table shows the state table of D flip-flop. image

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/add5e124-f9c2-444d-8a3d-bb382fb2d0fb)

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/9e4f413d-a6cf-47c0-93fb-9d9f5b6fe5e5)

Therefore, D flip-flop always Hold the information, which is available on data input, D of earlier positive transition of clock signal. From the above state table, we can directly write the next state equation as Qt+1t+1 = D

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/1eb72437-d384-4a98-aad1-ffe48e4c206c)


Next state of D flip-flop is always equal to data input, D for every positive transition of the clock signal. Hence, D flip-flops can be used in registers, shift registers and some of the counters.

## JK Flip-Flop
JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/db7610bb-53c6-4845-8cf9-fb347f980858)

This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/ac8ecb76-b658-4b3d-b5b6-807396dcff4e)


Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/7dddb4ef-8ba8-4b69-954e-428f6471f094)


By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/f01e93d8-79c6-4b2b-abf5-d32be25cdf1b)


The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

## T Flip-Flop
T flip-flop is the simplified version of JK flip-flop. It is obtained by connecting the same input ‘T’ to both inputs of JK flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of T flip-flop is shown in the following figure.

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/b2c4cd2f-e56f-48f8-af5e-dfdb41e0b702)


This circuit has single input T and two outputs Qtt & Qtt’. The operation of T flip-flop is same as that of JK flip-flop. Here, we considered the inputs of JK flip-flop as J = T and K = T in order to utilize the modified JK flip-flop for 2 combinations of inputs. So, we eliminated the other two combinations of J & K, for which those two values are complement to each other in T flip-flop. The following table shows the state table of T flip-flop.

Here, Qtt & Qt+1t+1 are present state & next state respectively. So, T flip-flop can be used for one of these two functions such as Hold, & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of T flip-flop. Inputs Present State Next State

![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/481a48c7-57fa-42c8-8f4b-1ee96ce9fcd0)


From the above characteristic table, we can directly write the next state equation as Q(t+1)=T′Q(t)+TQ(t)′ ⇒Q(t+1)=T⊕Q(t)

### Procedure
1.Using nand gates and wires construct SR flip flop.

2.Repeat same steps to construct JK,D,T flipflops.

3.Find RTL logic and timing diagram for all flipflops

### PROGRAM
## SR Flip-Flop:
 module sr(S,R,clk,Q,Qbar);
 input S,R,clk;
 output reg Q;
 output reg Qbar;
 initial Q=0;
 initial Qbar=1;
 always @(posedge clk)
 begin
 Q=S|((~R)&Q);
 Qbar=R|((~S)&(Qbar));
 end
 endmodule
## JK Flip-Flop:
 module jk(J,K,clk,Q,Qbar);
 input J,K,clk;
 output reg Q;
 output reg Qbar;
 initial Q=0;
 initial Qbar=1;
 always @(posedge clk)
 begin
 Q=(J&(~Q))|((~K)&Q);
 Qbar=((~J)&(Qbar))|K&(~Qbar);
 end
 endmodule
## D Flip-Flop:
module d(d,clk,q,qbar);
input d,clk;
output q,qbar;
reg q,qbar;
always @(posedge clk)
begin
q=d;
qbar=~q;
end
endmodule
## T Flip-Flop:
module t(clk,T,q,qbar);
input clk,T;
output q,qbar;
reg q,qbar;
always @(posedge clk)
begin
q=(T&~q)|(~T&q);
qbar=~q;
end
endmodule
RTL LOGIC FOR FLIPFLOPS
## SR Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/ee810a8b-144a-45e0-bc35-e8f6a0826de4)


## JK Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/f019a981-b6fd-478c-b1df-93abca91860e)


## D Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/3511efff-3d2f-4018-bb94-db007e0fc285)


## T Flip-Flop:


### TIMING DIGRAMS FOR FLIP FLOPS
## SR Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/89788ae3-c800-45f5-b3ce-34fa50b31b23)


## JK Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/f16caafb-1bcc-4d92-a163-54730418dd2c)


## D Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/0a9fa447-641e-4b69-a4f2-3001744ffe23)


## T Flip-Flop:
![image](https://github.com/23011258/Experiment--05-Implementation-of-flipflops-using-verilog/assets/139842204/3d926412-eb1a-4feb-acd6-c39ad44cb6f8)


## RESULTS
Thus, the implementation of SR,JK,D and T flipflops using nand gates are done sucessfully.
