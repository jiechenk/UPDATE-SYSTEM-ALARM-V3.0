# UPDATE-SYSTEM-ALARM-V3.0
UPDATE SYSTEM ALARM V3.0
1. Konfigurasi IP Statis (Sesuaikan dengan Router Anda)
Di bagian atas kode, sesuaikan dengan jaringan router Anda:
          // Jika router Anda 192.168.1.1
    IPAddress local_IP(192, 168, 1, 100);  
    IPAddress gateway(192, 168, 1, 1);

         // Atau jika router Anda 192.168.0.1
    IPAddress local_IP(192, 168, 0, 100);  
    IPAddress gateway(192, 168, 0, 1);

        // Atau jika router Anda 10.0.0.1
    IPAddress local_IP(10, 0, 0, 100);  
    IPAddress gateway(10, 0, 0, 1);

2. Upload Kode & HTML

Upload HTML ke LittleFS (folder data)
Upload sketch ke ESP32

3. Cara Akses:
Mode AP (Pertama kali):

SSID: Futsal_Timer_Setup
Password: 12345678
IP: http://192.168.4.1

Setelah Connect ke WiFi Router:

IP Statis: http://192.168.1.100 ← Akses ini
mDNS: http://futsal-timer.local ← Atau ini
Lihat Serial Monitor untuk konfirmasi IP
 
   ✓ WiFi Connected!
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📶 SSID: NamaWiFiAnda
📍 IP Address: http://192.168.1.100
🌐 mDNS: http://futsal-timer.local
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
