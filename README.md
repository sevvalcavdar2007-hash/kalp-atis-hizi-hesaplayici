# kalp-atis-hizi-hesaplayici
Python ile geliştirilmiş basit kalp atış hızı hesaplayıcı.
print("*" * 40)
print("❤️  KALP ATIŞ HIZI DEĞERLENDİRME ❤️")
print("*" * 40)

name = input("isim giriniz: ")
print(f"Merhaba {name} hoş geldin!")

age = int(input("Yaş: "))
nabiz = int(input("Nabiz: "))

# Matematiksel hesaplama
maksimum = 220 - age
alt = maksimum * 0.50
ust = maksimum * 0.85

print(f"Maksimum kalp atış hızı: {maksimum}")
print(f"Hedef egzersiz aralığı: {alt:.0f}-{ust:.0f}")

# Yaşa göre dinlenme nabzı kontrolü
if 7 <= age <= 9:
    if 80 <= nabiz <= 120:
        print("Normal")
    else:
        print(" nabız 80-120 arasında olmalı.")

elif 10 <= age <= 14:
    if 70 <= nabiz <= 110:
        print("Normal")
    else:
        print(" nabız 70-110 arasında olmalı.")

elif age >= 15:
    if 60 <= nabiz <= 100:
        print("Normal")
    else:
        print(" nabız 60-100 arasında olmalı.")     
else:
    print("Bu yaş grubu için değerlendirme yapılamıyor.")    
