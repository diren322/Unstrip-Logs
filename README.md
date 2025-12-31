# Unstrip Logs Mod

Minecraft 1.21.11 için Fabric modu - Soyulmuş odunları normal oduna geri dönüştürün!

## Özellikler

- Elinde **balta** olan oyuncular, **stripped log** veya **stripped wood** bloklarına sağ tıklayarak onları normal odun haline geri döndürebilir
- **Vanilla uyumlu**: 
  - ✅ Client-side `PASS` döndürür → Bakır cilalama çalışır
  - ✅ Server-side sadece stripped bloklar için `SUCCESS` döndürür
  - ✅ Diğer tüm vanilla balta davranışları korunur
- **Özel animasyon sistemi**:
  - ⚡ **Anında el sallama** (client-side)
  - 🔊 **İki aşamalı ses efekti** (server-side):
    - İlk ses: Derin balta sesi (pitch 0.8F) - vurma hissi
    - İkinci ses: Tiz ahşap sesi (pitch 1.2F) - kabuk geri gelme efekti
  - ⏱️ **3 tick gecikme** (~150ms) - blok dönüşümü için doğal hissiyat
- Blok dönüşürken **axis** (yön) korunur (X, Y veya Z)
- Baltaya **1 durability hasarı** verilir
- Shift tuşuna basmanız gerekmez
- Vanilla'yı taklit etmez - **özel ve farklı bir işlem** hissi verir

## Desteklenen Bloklar

### Stripped Logs → Normal Logs
- Oak, Spruce, Birch, Jungle, Acacia, Dark Oak
- Mangrove, Cherry, Pale Oak
- Crimson Stem, Warped Stem

### Stripped Wood → Normal Wood
- Tüm ağaç türleri için wood varyantları
- Crimson Hyphae, Warped Hyphae

## Oyun İçi Deneyim

1. **Oyuncu stripped log'a sağ tıklar**
2. **Anında**: El sallanır + derin balta sesi duyulur
3. **~150ms gecikme**: Görsel feedback süresi
4. **3 tick sonra**: Blok değişir + tiz ahşap sesi duyulur
5. **Baltanın durability'si**: 1 azalır

Bu, "sihirli geri çevirme" hissi veren özel bir mekanizmadır!

## Kurulum

1. [Fabric Loader](https://fabricmc.net/use/) yükleyin
2. [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api) yükleyin
3. `unstrip-logs-1.0.0.jar` dosyasını `.minecraft/mods` klasörüne kopyalayın

## Teknik Detaylar

- **Minecraft Sürümü**: 1.21.11
- **Fabric Loader**: 0.18.4+
- **Fabric API**: 0.140.2+1.21.11
- **Java**: 21
- **API**: UseBlockCallback (Fabric API)
- **Config**: JSON tabanlı (`config/unstrip-logs.json`)
- **Animasyon**: Client/Server split
- **Ses Efektleri**: 
  - `SoundEvents.AXE_STRIP` (pitch 0.8F)
  - `SoundEvents.WOOD_PLACE` (pitch 1.2F)

## Build

```bash
./gradlew build
```

Build edilmiş mod dosyası `build/libs/unstrip-logs-1.0.0.jar` olarak oluşturulur.

## Lisans

© 2025 Diren. Tüm hakları saklıdır (All Rights Reserved).
