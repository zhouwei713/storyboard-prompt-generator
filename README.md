# Storyboard Prompt Generator

## Bahasa Melayu

`Storyboard Prompt Generator` ialah Codex skill untuk menukar satu idea, gambar produk, atau deskripsi produk kepada **storyboard video menegak 9:16 selama 16 saat**.

Ia direka untuk TikTok, Reels, Shorts, iklan produk, dan aliran kerja image-to-video seperti Google Flow.

### Apa yang dihasilkan

Setiap permintaan menghasilkan:

1. Satu arah kreatif ringkas.
2. Fakta produk yang digunakan — berdasarkan imej atau maklumat pengguna sahaja.
3. Arahan suara/audio.
4. Tepat **2 scene berurutan**, setiap satu **8 saat**:
   - Scene 1: `0:00–0:08` — hook atau pengenalan produk.
   - Scene 2: `0:08–0:16` — demo, payoff dan CTA semula jadi.
5. Prompt image-to-video yang boleh terus digunakan bagi setiap scene.
6. Arahan kesinambungan dan negative prompt.

Output mengikuti bahasa pengguna. Untuk arahan Melayu, dialog, voice-over, dan arahan visual adalah dalam Bahasa Melayu Malaysia. Ia tidak menggunakan teks atau label bahasa Cina melainkan pengguna memintanya secara khusus.

### Contoh

```text
Use $storyboard-prompt-generator to turn this toothpaste product image into a 16-second TikTok animation. Make the toothpaste tube speak in Bahasa Melayu.
```

Hasilnya ialah storyboard 2 scene menegak: produk yang sama kekal konsisten, ada dialog/suara, arahan bunyi, pergerakan kamera, dan prompt Flow yang berasingan untuk Scene 1 dan Scene 2.

### Peraturan penting

- Menegak **9:16**, bukan horizontal 16:9.
- Tepat **2 scene × 8 saat = 16 saat**.
- Setiap scene ada arahan voice-over/dialogue dan audio.
- Jangan reka claim, harga, bahan, result, UI, kad, teks atas skrin, atau produk tambahan.
- Kekalkan rupa, warna, bentuk, dan label produk berpandukan gambar rujukan.
- Storyboard siap tidak bermaksud video sudah dirender.

## English

`Storyboard Prompt Generator` is a Codex skill that turns one idea, product image, or product description into a **16-second vertical 9:16 video storyboard**.

It is designed for TikTok, Reels, Shorts, product ads, and image-to-video workflows such as Google Flow.

### Output

Each request returns:

1. A concise creative direction.
2. Product facts used, based only on the image or user input.
3. Voice and audio direction.
4. Exactly **two sequential 8-second scenes**:
   - Scene 1: `0:00–0:08` — hook or product introduction.
   - Scene 2: `0:08–0:16` — demo, payoff, and a natural CTA.
5. One copy-ready image-to-video prompt per scene.
6. Continuity and negative-prompt rules.

The output follows the user's language. Malay requests receive natural Bahasa Melayu Malaysia dialogue and voice-over. Chinese text or labels are never added unless explicitly requested.

### Example

```text
Use $storyboard-prompt-generator to turn this toothpaste product image into a 16-second TikTok animation. Make the toothpaste tube speak in Bahasa Melayu.
```

### Non-negotiable constraints

- Vertical **9:16**, never horizontal 16:9.
- Exactly **2 scenes × 8 seconds = 16 seconds**.
- Every scene includes dialogue/voice-over and audio direction.
- No invented claims, prices, ingredients, results, UI, cards, on-screen text, or extra products.
- Preserve the referenced product's visible identity.
- A completed storyboard is not a rendered video.

## Files

```text
storyboard-prompt-generator
  SKILL.md
  agents/openai.yaml
  references/prompt-patterns.md
```
