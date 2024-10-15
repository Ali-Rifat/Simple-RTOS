# Monitor ADC UART pada STM32

## Deskripsi

Proyek ini merupakan implementasi sederhana untuk mikrokontroler STM32 yang membaca nilai ADC dan mengirimkannya melalui UART ketika tombol ditekan. Nilai ADC dapat dilihat pada serial monitor dengan baud rate 115200.

Proyek ini juga menampilkan nilai ADC secara real-time pada layar OLED, dan mendukung dua tombol untuk interaksi. Ketika tombol 1 ditekan, nilai ADC akan dikirimkan melalui UART.

## Fitur

- **Komunikasi UART**: Mengirimkan nilai ADC melalui UART saat tombol 1 ditekan.
- **Tampilan OLED**: Menampilkan nilai ADC secara real-time.
- **Interaksi Tombol**: 
  - Tombol 1: Mengirimkan nilai ADC melalui UART.
  - Tombol 2: Disiapkan untuk fungsi tambahan di masa depan.
  
## Komponen

- **Mikrokontroler STM32**
- **Layar OLED (SSD1306)**
- **Tombol (untuk interaksi)**
- **Komunikasi UART**

## Baudrate

- Baud rate UART: `115200`

## Cara Penggunaan

1. Hubungkan mikrokontroler STM32 ke komputer Anda dan buka serial monitor.
2. Atur baud rate ke `115200`.
3. Tekan tombol 1 untuk mengirimkan nilai ADC saat ini melalui UART.

## Struktur Kode

- `getADC`: Membaca nilai ADC dari sensor yang terhubung.
- `dispUART`: Menangani pengiriman nilai ADC melalui UART.
- `dispOLED`: Menampilkan nilai ADC pada OLED.
- `pickButton`: Mendeteksi penekanan tombol untuk memicu pengiriman UART.

## Lisensi

Proyek ini dilisensikan di bawah GNU General Public License. Untuk informasi lebih lanjut, lihat file [LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html).

## Penulis

Ditulis oleh Jonathan Burkley Rodriguez untuk Phipp's Electronics.
https://www.phippselectronics.com/writing-your-first-rtos-program-using-stm32cubemx/?srsltid=AfmBOopLhw8Ddh3q2aPZa_YRozN4li3xy0I23AQvtxdGygjmY5C3X2i9
