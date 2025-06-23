# Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule
Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule

update @ 2025/06/23

1. initial RH850 EVB - RH850/F1KM-S1 (BLDC) Starter Kit , to test below function 

- UART : RX:P10_9 , TX:P10_10

- CAN1 : RX:P10_7 (polling , no RX rule , accept all ID) , TX:P10_6 (polling)

2. Below is EVB switch

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/EVB_CAN_cfg.jpg)

3. Below is PCAN config setting 

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/PCAN_cfg.jpg)

4. Below is power on message

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/log_MCU_power_on.jpg)

5. when use UART terminal , which send CAN TX message from RH850 EVB , and rececive with PCAN


digit 1 , 
![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/log_tx1.jpg)


digit 2 , 
![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/log_tx2.jpg)


digit 3 , 
![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/log_tx3.jpg)


6. Below is different ID test condition , which send by PCAN , and rececive with RH850 RX


- ID : 100 , Extend ID , Data Frame , DLC 64 , CAN FD Frame , w/o BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_100.jpg)


- ID : 103 , Extend ID , Data Frame , DLC 8 , CAN FD Frame , w/ BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_103.jpg)


- ID : 103 , Standard ID , Remote Frame , DLC 8 , CAN Frame , w/o BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_103_RTR.jpg)


- ID : 123 , Standard ID , Data Frame , DLC 8 , CAN Frame , w/o BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_123.jpg)


- ID : 55 , Extend ID , Data Frame , DLC 16 , CAN FD Frame , w/o BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_055.jpg)


- ID : 66 , Standard ID , Data Frame , DLC 24 , CAN FD Frame , w/o BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_066.jpg)


- ID : 77 , Standard ID , Data Frame , DLC 48 , CAN FD Frame , w/ BRS

![image](https://github.com/released/Sample_Project_RH850_S1_CAN_FD_RX_Polling_No_Rule/blob/main/rx_pollig_ID_077.jpg)

