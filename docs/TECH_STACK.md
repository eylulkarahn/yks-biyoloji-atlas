# 🛠 Tech Stack — YKS Biyoloji Atlası

## Frontend

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| Flutter | 3.19+ | Cross-platform mobil uygulama |
| Dart | 3.3+ | Programlama dili |

## State Management

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| flutter_riverpod | ^2.5.0 | Reactive state yönetimi |
| riverpod_annotation | ^2.3.0 | Code generation için annotation'lar |
| riverpod_generator | ^2.4.0 | Provider code generation |

## Backend & Veri

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| supabase_flutter | ^2.5.0 | Auth, Database, Storage, Realtime |
| hive_flutter | ^1.1.0 | Offline-first local storage |
| connectivity_plus | ^6.0.0 | İnternet bağlantısı kontrolü |

## UI & Animasyon

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| flutter_svg | ^2.0.10 | SVG diyagram render |
| rive | ^0.13.0 | İnteraktif mikro-animasyonlar |
| shimmer | ^3.0.0 | Loading skeleton efekti |

## Navigasyon

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| go_router | ^14.0.0 | Declarative routing |

## Yardımcı Paketler

| Paket | Versiyon | Kullanım |
|-------|----------|----------|
| flutter_dotenv | ^5.1.0 | Environment variables |
| shared_preferences | ^2.2.0 | Basit key-value storage |
| intl | ^0.19.0 | Tarih/saat formatı |
| freezed_annotation | ^2.4.0 | Immutable data classes |
| json_annotation | ^4.9.0 | JSON serialization |

## Dev Dependencies

| Paket | Kullanım |
|-------|----------|
| build_runner | Code generation çalıştırma |
| freezed | Data class generation |
| json_serializable | JSON serialization generation |
| hive_generator | Hive adapter generation |
| flutter_lints | Kod kalite kuralları |

## Mimari

Proje **Clean Architecture** prensipleri ile geliştirilmektedir:

```
lib/
├── core/          # Sabitler, tema, utils
├── data/          # API, local storage, modeller
├── domain/        # Entity'ler, repository interface'leri
├── presentation/  # UI, provider'lar, widget'lar
└── routes/        # Navigasyon
```

## Supabase Tabloları

| Tablo | Açıklama |
|-------|----------|
| `users` | Kullanıcı profilleri |
| `topics` | Biyoloji konuları ve SVG yolları |
| `regions` | SVG üzerindeki etkileşimli bölgeler |
| `progress` | Kullanıcı ilerleme verileri |
