# Hugging Face Kursu — Türkçe

[**Türkçe**](README.md) | [English](README_EN.md)

Bu depo, [Hugging Face Course](https://github.com/huggingface/course) projesinin Türkçe yerelleştirme çalışmasını içeren bir forktur. Kurs; Transformer modellerini doğal dil işleme görevlerinde ve farklı makine öğrenmesi uygulamalarında kullanmayı öğretir.

Kurs boyunca şu Hugging Face araçlarını tanıyabilirsin:

- [🤗 Transformers](https://github.com/huggingface/transformers)
- [🤗 Datasets](https://github.com/huggingface/datasets)
- [🤗 Tokenizers](https://github.com/huggingface/tokenizers)
- [🤗 Accelerate](https://github.com/huggingface/accelerate)
- [Hugging Face Hub](https://huggingface.co/models)

Kurs tamamen ücretsiz ve açık kaynaklıdır.

## Türkçe içerikler

Türkçe ders kaynakları [`chapters/tr`](chapters/tr) klasöründe bulunur. Şu anda yerelleştirilmiş bölümler şunlardır:

| Bölüm | Konu |
|---|---|
| 0.1 | Kurulum ve giriş |
| 1.1 | Transformer modellerine giriş |
| 1.2 | Doğal dil işleme |
| 1.5 | Encoder modelleri |
| 1.6 | Decoder modelleri |
| 2.1 | 🤗 Transformers kullanımı |
| 3.1 | Önceden eğitilmiş bir modele ince ayar yapma |
| 4.1 | [Hugging Face Hub](chapters/tr/chapter4/1.mdx) |

İçindekiler yapısı [`chapters/tr/_toctree.yml`](chapters/tr/_toctree.yml) dosyasında tutulur.

> Türkçe çeviri henüz tamamlanmamıştır. Eksik bölümlerde İngilizce kaynak dosyaları kullanılabilir.

## Kursta neler öğreneceksin?

### Transformer modelleri

Transformer mimarisinin temel bileşenlerini, encoder ve decoder modellerini, attention mekanizmasını ve farklı model ailelerinin hangi görevlerde kullanıldığını öğrenebilirsin.

### Tokenization

Metnin modeller tarafından işlenebilen token'lara nasıl dönüştürüldüğünü ve Hugging Face Tokenizers kütüphanesinin nasıl kullanıldığını inceleyebilirsin.

### Model eğitimi ve ince ayar

Önceden eğitilmiş modelleri kendi veri kümen üzerinde eğitmeyi, eğitim sonuçlarını değerlendirmeyi ve farklı görevler için uyarlamayı öğrenebilirsin.

### Veri kümeleri

Hugging Face Datasets ile veri yükleme, dönüştürme, işleme ve paylaşma adımlarını uygulayabilirsin.

### Model paylaşımı

Modelleri ve tokenizer'ları Hugging Face Hub üzerinde sürüm kontrollü biçimde yayımlamayı ve başkalarının kullanımına sunmayı öğrenebilirsin.

## Klasör yapısı

- `chapters/en`: İngilizce kaynak dersler.
- `chapters/tr`: Türkçe yerelleştirilmiş dersler.
- `subtitles`: Video altyazıları.
- `utils`: Notebook ve dokümantasyon yardımcı araçları.
- `.github`: Dokümantasyon oluşturma iş akışları.

## Yerel önizleme

Önce sanal ortam oluşturup gerekli araçları yükle:

```bash
python -m venv .venv
python -m pip install --upgrade pip
python -m pip install "git+https://github.com/huggingface/doc-builder.git"
```

Ardından Türkçe içeriği önizle:

```bash
doc-builder preview course ./chapters/tr --not_python_module
```

> `doc-builder preview` komutunun Windows üzerinde çalışmadığı upstream dokümantasyonunda belirtilmektedir. Gerekirse WSL veya Linux ortamı kullanılabilir.

## Notebook oluşturma

Kurstaki kod örneklerini Jupyter notebook dosyalarına dönüştürmek için:

```bash
python -m pip install -r requirements.txt
python utils/generate_notebooks.py --output_dir nbs
```

Oluşturulan notebook'lar `nbs` klasörüne kaydedilir.

## Çeviri yaklaşımı

Türkçe yerelleştirmede:

- Kod blokları ve dosya yolları değiştirilmez.
- Teknik terimlerin anlamı korunur.
- Başlıklar ve açıklamalar doğal Türkçeyle yazılır.
- MDX bileşenleri ve bağlantılar kaynak yapıyla uyumlu tutulur.
- Yalnızca çevrilmiş dosyalar Türkçe içindekiler tablosuna eklenir.

## Orijinal proje

Bu çalışma, [huggingface/course](https://github.com/huggingface/course) deposunu temel alır. Orijinal projenin yazarları ve katkıda bulunanları GitHub geçmişinde korunmaktadır.

## Lisans

Proje [Apache License 2.0](LICENSE) ile dağıtılır. Türkçe yerelleştirme de aynı lisans koşulları kapsamında sunulur.
