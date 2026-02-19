# 📱 UI & Navigasyon — YKS Biyoloji Atlası

## Ekran Haritası

```
Uygulama Başlangıcı
│
├── /splash          → SplashScreen (2sn, auth kontrol)
│
├── /onboarding      → OnboardingScreen (ilk açılış)
│
├── /login           → LoginScreen
│   └── /register    → RegisterScreen
│
└── MainShell (Bottom Navigation)
    ├── /home        → HomeScreen
    ├── /explore     → ExploreScreen
    │   └── /topic/:id → TopicDetailScreen
    │       └── /quiz/:topicId/:mode → QuizShell
    │           ├── explore_learn  → Keşfet ve Öğren
    │           ├── pinpoint       → Nokta Atışı
    │           ├── glow_identify  → Parlayanı Bil
    │           ├── drag_drop      → Sürükle Bırak
    │           └── flow_complete  → Akış Tamamlama
    ├── /progress    → ProgressScreen
    └── /settings    → SettingsScreen
```

## Bottom Navigation

| Index | Route | İkon | Label |
|-------|-------|------|-------|
| 0 | /home | home | Ana Sayfa |
| 1 | /explore | explore | Keşfet |
| 2 | /progress | bar_chart | İlerleme |
| 3 | /settings | settings | Ayarlar |

## 5 Quiz Modu

### 🧊 Keşfet ve Öğren (`explore_learn`)
- SVG üzerinde bulanık etiketler gösterilir
- Dokunulunca etiket açığa çıkar
- Stressiz keşif modu

### 📍 Nokta Atışı (`pinpoint`)
- Kullanıcıya yapı adı söylenir
- SVG üzerinde doğru yere dokunması istenir
- Mekansal hafıza güçlendirme

### ✨ Parlayanı Bil (`glow_identify`)
- SVG'de bir bölge parlar
- 4 şıktan doğrusu seçilir
- Görsel tanıma hızı

### 🎯 Sürükle ve Bırak (`drag_drop`)
- Etiketler sürüklenerek doğru bölgelere bırakılır
- Parça-bütün ilişkisi kurma

### 🔄 Akış Tamamlama (`flow_complete`)
- Biyolojik döngülerde eksik adımlar doldurulur
- Süreç mantığı anlama

## Renk Paleti

| Renk | Hex | Kullanım |
|------|-----|----------|
| Primary | `#2E7D32` | Ana renk, butonlar |
| Primary Light | `#60AD5E` | Gradient, vurgular |
| Secondary | `#00796B` | İkincil aksanlar |
| Background | `#FAFAFA` | Sayfa arka planı |
| Surface | `#FFFFFF` | Kart arka planı |
| Glow | `#64FFDA` | Quiz doğru cevap parlaması |
| Error | `#E53935` | Hata durumları |
| Success | `#4CAF50` | Başarı durumları |

## Spacing Sistemi

| İsim | Değer | Kullanım |
|------|-------|----------|
| xs | 4px | Çok küçük boşluk |
| sm | 8px | Küçük boşluk |
| md | 16px | Standart boşluk |
| lg | 24px | Büyük boşluk |
| xl | 32px | Çok büyük boşluk |
| xxl | 48px | Ekstra büyük |
