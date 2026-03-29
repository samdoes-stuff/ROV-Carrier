
# 23/03/2026

After working for sometimes, I realized I need to journal everything or else I will forget. 

Massive change for now. Fully switched to RADXA CM4 for more options and feature around the same price. 
As I saw Jeff Geerling's youtube video previously, he mentioned that the Software support is bad. 

Also, I don't have a lot of experience in software. I mean no experience with embedded software. 

After inspecting through the schematic, I found a lot of good things. 

1. The connectors and even the connections of two parts of the CM4 are as same as Raspberry pi CM4. So 
I don't have to change the connections of those two. 
That means my Sensors and Connectors are going to be totally fine. 

2.  I was looking for active cooling. But I realized that I cannot afford pin in RP CM4. But RADXA solves this issue. 

3. Also, RADXA has amazing storage options. Onboard emmc, ssd, sata, sd card and even UFS. If you are wondering
what UFS are? Please check UFS out. I also got to know about UFS yesterday while navigationg RADXA. 

UFS are faster than emmc and can pack a lot of storage in small price. Hard thing is to source them. 

4. Also off mood, I will use this as my travel partner using my main ssd so It also provides the option. 

Danger:  It is too good true be true. I am doubting that Radxa CM4 can do lot of things at once. I have to do some research and update the journal. 

Time to fix my SSD portion and check the 40 pin gpio

decision changed again rooting for CM5. Better at eveything.


# 28/03/2026 

Plan changed again. I found out that Radxa is copy catting a chinese company and selling their module in a higher price. 
I found some more great option than RADXA CM5 which is SOM RK3399V2 from "Friendly Elec"  

It is much cheaper (87$) and meets most of my needs. I will use this hopefully I don't bring in any big change. 


Ahh may be I won't because I need the 40 pin gpio support for my carrier. eDP is supported in Radxa Cm5 but not used. I will definitely use the eDP let's see. 

what should I do? When I am focusing more on expandibility, I am losing some functions. Main purpose is to make a carrier board but when I am making something why don't I make this for my cyberdeck. Same thing but needs more time from me.  

Should I move on or I restart everything. Ohh boy!!!!

# 29/03/2026 

Pin config for my understanding 

First What is already equipped 

## PCIE-E key  
1. GPIO4_A1
2. GPIO4_A0
3. GPIO4_A2
4. GPIO3_A6
5. GPIO1_A3
6. GPIO1_A2
7. GPIO4_C3
8. GPIO1_A0
9. GPIO1_A1
10. GPIO2_C3
11. GPIO2_C0
12. GPIO0_C5
13. GPIO2_B7
14. GPIO0_C4
15. GPIO2_A6
16. GPIO2_A7
17. GPIO2_B0
18. GPIO2_B1
19. GPIO2_B2
20. GPIO0_B2
21. GPIO2_B3

## Type-C 
1. I2C6_SDA_M0
2. I2C6_SCL_M0
3. GPIO0_D3
4. GPIO1_D2

## Type-C 2
1. GPIO3_B4
2. GPIO0_D5
3. I2C7_SDA_M0
4. I2C7_SCL_M0

## PCIE3.0 M key 
1. GPIO4_B4
2. GPIO4_B5
3. GPIO4_B6

## eDP
1. GPIO3_A7
2. GPIO3_B7

## SD Card 
1. GPIO0_A4

## Ext_USB2.0 
1. GPIO1_B0

## Audio (Probably Need to change(I2S) the interface but GPIO remains)
1. GPIO1_A7
2. GPIO1_C4
3. I2C6_SDA_M0
4. I2C6_SCL_M0

## For navigator I need 4 pairs of RX & TX signal. 
1. TX1_RPI - GPIO1_B6 
2. RX1_RPI - GPIO1_B7
3. TX3_RPI - GPIO3_B5 
4. RX3_RPI - GPIO3_B6 
5. TX4_RPI - GPIO3_C0
6. RX4_RPI - GPIO3_C1
7. TX5_RPI - GPIO1_B5
8. RX5_RPI - GPIO1_B4

## I need 4 pairs of SDA & SCL
1. SDA0
2. SCL0
3. SCL1
4. SDA1
5. SDA4
6. SCL4
7. SCL6
8. SDA6

## I need 5 SPI
1. SPI_CS1 - 
2. SPI_CS2 - 
3. SPI1_SCLK -  
4. SPI1_MISO -  
5. SPI1_MOSI - 
