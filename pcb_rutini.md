# Aylık PCB Tasarım Rutini

Her ay bu listeden bir proje seçilerek tasarlanacak. Projeler zorluk seviyesine göre 4 kademeye ayrılmıştır. Başlangıçta kolay seviyeden başlamak workflow oturtmak için tavsiye edilir, ancak sıra zorunlu değildir — istenilen seviyeden istenilen proje seçilebilir.

---

## 🟢 Seviye 1 — Başlangıç (THT ağırlıklı, tek katman yeterli)

Temel KiCad / EasyEDA workflow'unu öğrenmek, gerber üretmek, ilk lehimleme deneyimleri için uygundur.

- [ ] 555 Timer LED Blinker
- [ ] Elektronik zar (CD4017 + 7 LED)
- [ ] LM3914 VU metre
- [ ] Logic probe
- [ ] Continuity tester (süreklilik testi)
- [ ] Lineer voltaj regülatörü (LM7805 / AMS1117)
- [ ] USB-C breakout (basit, sadece güç)
- [ ] 7-segment display sürücü
- [ ] Servo tester
- [ ] IR remote receiver breakout
- [ ] Solenoid sürücü
- [ ] EL wire inverter (küçük)

---

## 🟡 Seviye 2 — Orta-Kolay (SMD'ye giriş, çok bileşenli)

SMD lehimleme, decoupling, basit güç yönetimi konularına giriş.

- [ ] Buck converter breakout (MP1584 / LM2596)
- [ ] Boost converter breakout
- [ ] TP4056 + DW01 Li-ion şarj & koruma kartı
- [ ] Op-amp ses amplifikatörü (LM386)
- [ ] Aktif filtre kartı (low-pass / band-pass)
- [ ] Mikrofon preamp
- [ ] Wien bridge osilatör
- [ ] Sample & hold devresi
- [ ] Shift register LED bar (74HC595)
- [ ] Binary counter göstergesi
- [ ] Rotary encoder breakout
- [ ] Capacitive touch slider
- [ ] Logic level converter
- [ ] USB-UART köprüsü (CH340 / CP2102)
- [ ] H-bridge motor sürücü (DRV8833)
- [ ] Step motor sürücü (A4988 klonu)
- [ ] WS2812B LED matrix
- [ ] OLED breakout
- [ ] Rotary encoder volume kontrol
- [ ] FM radyo alıcısı (TEA5767)
- [ ] PD trigger USB-C breakout

---

## 🟠 Seviye 3 — Orta-İleri (mikrodenetleyici, switching, sensör entegrasyonu)

Tam bir mikrodenetleyici kartı tasarlamak, switching regülatör layout kuralları, çok sensörlü sistemler.

- [ ] ATtiny85 dev board (ISP header, decoupling)
- [ ] ATmega328 Arduino klonu
- [ ] ESP8266 / ESP32 dev board (anten clearance dahil)
- [ ] RP2040 minimum sistem
- [ ] STM32 "blue pill" klonu
- [ ] CH32V003 (RISC-V) dev board
- [ ] Raspberry Pi HAT (GPIO + EEPROM)
- [ ] I2C sensör hub (BME280 + MPU6050 + OLED)
- [ ] Ultrasonik mesafe modülü
- [ ] HX711 + load cell breakout
- [ ] Geiger sayacı (HV üreteç dahil)
- [ ] Nixie tube sürücü (HV switching)
- [ ] Negatif voltaj üreteci (charge pump)
- [ ] Solar harvester (panel + supercap + MPPT)
- [ ] Theremin
- [ ] VCO/VCA synth modülü
- [ ] POV (persistence of vision) display
- [ ] nRF24L01 breakout (RF layout)
- [ ] Bluetooth audio receiver
- [ ] IR transceiver modülü
- [ ] E-paper interface kartı
- [ ] Dijital kasa kilidi (D flip-flop tabanlı)
- [ ] ESR meter
- [ ] Bench power supply ön panel

---

## 🔴 Seviye 4 — İleri (4 katman, mixed-signal, RF, yüksek hız)

Profesyonel PCB tasarımına geçiş: differential pair, impedance matching, ayrı analog/dijital ground, EMI kontrolü.

- [ ] LoRa modül kartı (RF tasarım)
- [ ] Kamera interface kartı (MIPI / parallel)
- [ ] BLDC ESC (kapalı çevrim akım kontrolü)
- [ ] Tesla coil sürücü (yüksek frekans + izolasyon)
- [ ] STM32 + analog ön uç (ADC, ayrı ground plane'ler)
- [ ] 4-layer mixed-signal kart (DAC + filtre + MCU)
- [ ] Class-D amplifikatör
- [ ] Switching bench power supply (programmable)
- [ ] Hot air rework station kontrol kartı
- [ ] Reflow fırın kontrolcü (PID + termokupul)
- [ ] FPGA breakout (iCE40 / Tang Nano)
- [ ] USB hub (USB 2.0)
- [ ] Ethernet PHY breakout

---

## 📋 İlerleme Takibi

| Ay | Seçilen Proje | Seviye | Şematik | Layout | Üretim | Lehim | Test |
|----|---------------|--------|:-------:|:------:|:------:|:-----:|:----:|
| 1  |               |        |         |        |        |       |      |
| 2  |               |        |         |        |        |       |      |
| 3  |               |        |         |        |        |       |      |
| 4  |               |        |         |        |        |       |      |
| 5  |               |        |         |        |        |       |      |
| 6  |               |        |         |        |        |       |      |
| 7  |               |        |         |        |        |       |      |
| 8  |               |        |         |        |        |       |      |
| 9  |               |        |         |        |        |       |      |
| 10 |               |        |         |        |        |       |      |
| 11 |               |        |         |        |        |       |      |
| 12 |               |        |         |        |        |       |      |

---

## 📝 Notlar

- Her proje için ayrı bir klasör tut: `şematik`, `gerber`, `BOM`, `fotoğraflar`, `notlar.md`
- Her tasarımdan sonra kısa bir "ne öğrendim / ne yanlış gitti" notu yaz — bir yıl sonra çok değerli olur
- Bir projeyi bitiremezsen sorun değil, bir sonraki aya devret veya listeden başka bir şey seç
- Aynı bileşeni iki kez kullanmamaya çalış (çeşitlilik için)
