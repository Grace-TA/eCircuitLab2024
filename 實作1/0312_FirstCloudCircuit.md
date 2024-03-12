# 第一個雲端電路實作!

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/b718cc25-ef84-4d64-b6e5-55073df51817)

## 實作1: 麵包板 + 電錶量測電阻 (麵包板 vs. 分壓器); 請試著分析與說明結果

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/90666364-9f42-40a7-88fb-06a181798609)

> 這個結果可以通過歐姆定律（Ohm's Law）和串聯電路的特性來解釋。在串聯電路中，流經每個元件的電流是相同的。因此，我們首先計算整個電路的總電阻（R1 + R2 = 15K歐姆），然後使用歐姆定律（V = IR）計算出電路中的電流。有了電流值後，我們就能利用歐姆定律計算出在R2上的電壓（V = IR2）。


## 實作2: 麵包板 + 電源供應器 (5V) + 錶量測電壓, 為什麼會是3.33V? 請試著分析與說明結果

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/2d1d7497-e2f8-413c-9d0f-e64b696b785e)

> 在這個案例中，由於R2的電阻值是R1的兩倍，根據電壓分配原則，R2上的電壓將是整體電壓的較大一部分。計算結果顯示，R2上的電壓大約是3.33伏特，這代表了整體電壓5伏特中的大部分。這個結果說明了串聯電路中電壓分配的性質，即電壓會按照各元件電阻值的比例分配。

## 實作3: 麵包板 + Function Generator (Function: SINE, Frequency: 500Hz, Amplitdue: 5V, Offset: 0V) + 示波器 (Time Per Division: 1ms) , 請問#1與#2示波器量測到的Peak Voltage各是多少? 請試著分析與說明結果

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/c35eb40f-09dd-4c06-8463-b487a6ae1a1a)

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/701b9cbb-f5b5-4d9e-b69e-4097bb0b8742)

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/da76dba6-261f-4a65-b3eb-dd1f8ce6e2bf)


> #1示波器量測Funcion Gen的輸出; 因此, V.peak = ?; 而#2示波器量測點為R2的跨壓; 因此量測電壓應該會是原來的2/3.

## 實作4 - 麵包板 + LED X 3+ Resistor X 3 (i.e., Current Limit; R分別是900, 9K, 90K ohm), 使用電錶量測電流. 請試著分析與說明結果

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/37323de7-f90b-4991-96aa-5f85de786820)

> Current Limit越大, 電流越小; LED高度也越暗; 電錶的量測結果, 也再次確認接線是正確的.

## 實作5: 麵包板 + LED X 2 + Capacitor (10uF, 0.1uF) X 2, Switch X2, 使用示波器量測 (分離時間: 1s). 請試著分析與說明結果

![image](https://github.com/Grace-TA/eCircuitLab2024/assets/89304181/2198c2bd-0966-4558-a713-57ae36d6cf48)

> 典型的RC放電特性量測.電容和電池一樣, 越大越可以供應越久的操作. 
