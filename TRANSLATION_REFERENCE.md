# Translation Reference: Indonesian → English

This document provides a complete mapping of all translations made during the refactoring process.

---

## Common Terms

| Indonesian | English | Context |
|------------|---------|---------|
| Pernikahan | Wedding | General term |
| Undangan | Invitation | Invitation context |
| Menikah | Wedding/Married | Verb form |
| Waktu | Time | Section heading |
| Lokasi | Location | Section heading |
| Tentang | About | Section heading |
| Calon Mempelai Wanita (CPW) | Bride | Female partner |
| Calon Mempelai Pria (CPP) | Groom | Male partner |
| Nama | Name | Person's name |
| Tempat | Place/Venue | Location |
| Tanggal | Date | Calendar date |
| Hari | Day | Day of week or countdown |
| Jam | Hour | Time unit |
| Menit | Minute | Time unit |
| Detik | Second | Time unit |
| Sabtu | Saturday | Day of week |
| Akad Nikah | Ceremony | Wedding ceremony |
| Resepsi | Reception | Wedding reception |
| Konfirmasi Kehadiran | Attendance Confirmation | RSVP |
| Kabari | Notify/Message | Contact action |
| Kami yang berbahagia | With love and gratitude | Closing phrase |
| Foto | Photo | Image/picture |

---

## Full Text Translations

### Hero Section

**Indonesian:**
```
Undangan Pernikahan
Nama Wanita & Nama Pria
Sabtu, 21 April 2021
[Nama Tempat], [Nama Area]
[Nama Kota]
```

**English:**
```
Wedding Invitation
Bride Name & Groom Name
Saturday, April 21, 2021
[Venue Name], [Area Name]
[City Name]
```

---

### Countdown Section

**Indonesian:**
```
Hari : Jam : Menit : Detik
```

**English:**
```
Days : Hours : Minutes : Seconds
```

---

### Opening Message

**Indonesian:**
```
Assalamu'alaikum Warahmatullahi Wabarakatuh.
Dengan memohon rahmat dan ridha Allah swt,
kami bermaksud mengundang Bapak/Ibu/Saudara/Saudari 
pada acara pernikahan kami
```

**English:**
```
Peace be upon you and God's mercy and blessings.
With the grace and blessings of God,
we cordially invite you to join us in celebrating our wedding
```

**Note:** The Arabic greeting "Assalamu'alaikum" was translated to English while preserving the Islamic nature of the greeting.

---

### Names Section

**Indonesian:**
```
Nama Calon Mempelai Wanita
&
Nama Calon Mempelai Pria
```

**English:**
```
Bride Full Name
&
Groom Full Name
```

---

### Time Section

**Indonesian:**
```
Waktu

Sabtu
21
Maret 2020

Akad Nikah:
17.00 WIB

Resepsi:
19.00 - 21.00 WIB
```

**English:**
```
Time

Saturday
21
March 2020

Ceremony:
5:00 PM

Reception:
7:00 PM - 9:00 PM
```

**Note:** Time format changed from 24-hour (WIB = Western Indonesian Time) to 12-hour AM/PM format.

---

### Location Section

**Indonesian:**
```
Lokasi

Nama Tempat
Jl. Alamat Lengkap No.9, RT.001/RW.006A,
Kecamatan XXX, Kota XXX, Provinsi XXX
```

**English:**
```
Location

Venue Name
Street Address No.9, RT.001/RW.006A,
District XXX, City XXX, Province XXX
```

**Note:** Indonesian address format preserved as RT/RW are specific to Indonesian addressing.

---

### About the Couple Section

**Indonesian:**
```
Tentang [Calon Mempelai Wanita] dan [Calon Mempelai Pria]

Foto 1
Pertama kali saling kenal di [Sebut Nama Tempat]

Foto 2
Satu kantor, satu divisi, dan posisi tempat duduk saling membelakangi.

Foto 3
Cerita cinta dimulai

Foto 4
Pertemuan 2 keluarga

Foto 5
Lamaran

Foto 6
Menikah
```

**English:**
```
About the Couple

Photo 1
First met at [Place Name]

Photo 2
Same office, same division, sitting back to back.

Photo 3
Love story begins

Photo 4
Meeting the families

Photo 5
Engagement

Photo 6
Wedding
```

---

### RSVP Section

**Indonesian:**
```
Konfirmasi Kehadiran

Merupakan suatu kehormatan dan kebahagiaan bagi kami
apabila Bapak/Ibu/Saudara/Saudari berkenan hadir
memberikan doa restu.

Jika bisa hadir kami tunggu konfirmasinya,
Informasi: Di meja penerima tamu akan kami sediakan 
hand sanitizer dan pemeriksaan suhu tubuh.

Jika tidak memungkinkan untuk hadir di pernikahan kami,
tidak mengapa, semoga bisa berjumpa di lain kesempatan

Stay safe & jaga kesehatan ya :)

Kabari CPW
Kabari CPP
```

**English:**
```
Attendance Confirmation

It would be an honor and a joy for us
if you would kindly grace us with your presence
and blessings.

If you can attend, we look forward to your confirmation,
Note: Hand sanitizer and temperature checks will be 
available at the guest reception desk.

If you are unable to attend our wedding, it's okay,
we hope to see you on another occasion

Stay safe & take care :)

Message Bride
Message Groom
```

---

### Closing

**Indonesian:**
```
Kami yang berbahagia,
@instagramaccount (CPW)
@instagramaccount (CPP)
```

**English:**
```
With love and gratitude,
@instagramaccount (Bride)
@instagramaccount (Groom)
```

---

## CSS Class Translations

### Main Classes

| Indonesian Class | English Class | Meaning |
|-----------------|---------------|----------|
| `.tempatwaktu` | `.datetime-location` | Date-time and location |
| `.nama-lengkap` | `.full-name` | Full name |
| `.waktu` | `.time` | Time |
| `.tempat` | `.venue` | Place/venue |
| `.tanggal-hari` | `.date-day` | Day of week |
| `.tanggal-angka` | `.date-number` | Date number |
| `.tanggal-bulan` | `.date-month` | Month |

### Photo Classes

| Indonesian Class | English Class |
|-----------------|---------------|
| `.foto1` | `.photo1` |
| `.foto2` | `.photo2` |
| `.foto3` | `.photo3` |
| `.foto4` | `.photo4` |
| `.foto5` | `.photo5` |
| `.foto6` | `.photo6` |
| `.title-foto` | `.title-photo` |
| `.subtitle-foto` | `.subtitle-photo` |
| `.foto-foto` | `.photos` |
| `.foto-item` | `.photo-item` |

---

## ID Translations

| Indonesian ID | English ID | Section |
|--------------|------------|---------|
| `#Waktu` | `#time` | Time section |
| `#lokasi` | `#location` | Location section |
| `#tentang-pasangan` | `#about-couple` | About couple section |
| `#hitungmundur` | `#countdown` | Countdown timer |

---

## JavaScript Variables

| Indonesian Variable | English Variable | Purpose |
|--------------------|------------------|----------|
| `harih` | `weddingDate` | Wedding date variable |

---

## File Names

| Indonesian File | English File | Purpose |
|----------------|--------------|----------|
| `menikah.css` | `wedding.css` | Main stylesheet |
| `menikah.js` | `wedding.js` | Main JavaScript |

---

## Button Text

| Indonesian | English | Type |
|-----------|---------|------|
| Kabari CPW | Message Bride | WhatsApp button |
| Kabari CPP | Message Groom | WhatsApp button |

---

## Navigation Menu

| Indonesian | English |
|-----------|---------|
| Home | Home |
| Waktu | Time |
| Lokasi | Location |
| Tentang CPW & CPP | About the Couple |
| RSVP | RSVP |

---

## Time Format Notes

### Indonesian Format
- Uses 24-hour format (e.g., 17.00)
- Uses dots as separators (17.00)
- Includes timezone (WIB = Western Indonesian Time, UTC+7)

### English Format
- Uses 12-hour format (e.g., 5:00 PM)
- Uses colons as separators (5:00)
- Timezone can be specified (EST, PST, etc.) or omitted for local time

---

## Address Format Notes

### Indonesian Address Components
- **Jl.** = Jalan (Street)
- **RT** = Rukun Tetangga (Neighborhood unit)
- **RW** = Rukun Warga (Community unit)
- **Kecamatan** = District
- **Kota** = City
- **Provinsi** = Province

### English Translation
- **Jl.** → Street/Road
- **RT/RW** → (kept as is, specific to Indonesian addressing)
- **Kecamatan** → District
- **Kota** → City
- **Provinsi** → Province

---

## Cultural Notes

1. **Islamic Greeting**: The traditional Islamic greeting "Assalamu'alaikum Warahmatullahi Wabarakatuh" was translated to maintain cultural sensitivity while being accessible to English speakers.

2. **Formal Address**: Indonesian uses "Bapak/Ibu/Saudara/Saudari" (Mr./Mrs./Brother/Sister) as formal address. This was simplified to the general invitation tone in English.

3. **CPW/CPP Abbreviations**: These are Indonesian abbreviations for bride and groom, replaced with the full English terms.

4. **"Lamaran"**: This specifically means "engagement" or "proposal ceremony" in Indonesian weddings, a significant pre-wedding event.

---

## Meta Tags

| Indonesian | English |
|-----------|---------|
| `og:locale="id_ID"` | `og:locale="en_US"` |

---

**Compiled by:** Refactoring Agent  
**Date:** March 10, 2026  
**Language Pair:** Indonesian (Bahasa Indonesia) → English (US)

