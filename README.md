# LICENSE
Calculates simple interest using formula: (P × R × T) / 100  Interactive terminal prompts for principal, rate, and time  No dependencies – runs on any Linux/macOS system
#!/bin/bash

# Simple Interest Calculator
echo "Oddiy Foiz Kalkulyatori"
echo "------------------------"

read -p "Asosiy summani kiriting (P): " principal
read -p "Foiz stavkasini kiriting (% yillik, R): " rate
read -p "Muddatni kiriting (yil, T): " time

interest=$(( (principal * rate * time) / 100 ))
total=$(( principal + interest ))

echo "------------------------"
echo "Foiz miqdori: $interest"
echo "Jami to'lov summati: $total"
