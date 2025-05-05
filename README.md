# Sentimentanalyse von Reddit-Daten im Kontext von Kryptowährungen
## 🔗 GitHub-Repository

📁 Dieses Projekt findest du auf GitHub:  
👉 [github.com/Reimser/nlp_fine_tuning](https://github.com/Reimser/nlp_fine_tuning)

📥 Repository klonen:
```bash
git clone https://github.com/Reimser/nlp_fine_tuning.git
```
## Überblick
Dieses Repository enthält alle Notebooks, Auswertungen und Ergebnisse der Studienarbeit im Modul Data Mining an der Digital Business University of Applied Sciences.
Ziel des Projekts war es, verschiedene NLP-Modelle systematisch auf ihre Eignung zur Sentimentanalyse von kryptobezogenen Reddit-Beiträgen zu untersuchen und durch gezieltes Fine-Tuning zu optimieren.

Die Arbeit folgt dem CRISP-DM-Prozessmodell und vergleicht sowohl klassische lexikonbasierte Ansätze als auch moderne transformerbasierte Modelle.

## Inhalte
/notebooks/

alle_nlp_modelle.ipynb: Vergleich verschiedener Basis-Modelle (VADER, TextBlob, FinBERT, CryptoBERT, RoBERTa, DeBERTa)

elkulako.ipynb: Fine-Tuning von CryptoBERT auf Reddit-Kommentaren

finbert.ipynb: Fine-Tuning von FinBERT auf Reddit-Posts

/plots/

Visualisierungen der Modellperformance (F1-Scores pro Klasse)

Lernkurven für unterschiedliche Lernraten

/data/

Beispielhafte Struktur der verwendeten Datensätze (keine Originaldaten wegen Datenschutz)

/report/

Studienarbeit im PDF-Format (inklusive Methodik, Ergebnisse, Literaturverzeichnis)

## Modelle und Methoden
Transformer-Modelle:

FinBERT (Finanztexte)

CryptoBERT (Krypto-Kommentare)

RoBERTa, DeBERTa (Baseline-Vergleich)

Lexikonbasierte Modelle:

VADER

TextBlob

## Trainingsansätze:

Custom-Trainer mit gewichteter Verlustfunktion

Lernratenvergleich (2e-5 bis 1e-6)

Early Stopping basierend auf F1-Score

## Metriken:

F1-Score (macro)

Cohen’s Kappa

Accuracy

Highlights der Ergebnisse
CryptoBERT erreicht nach Feintuning auf Reddit-Kommentaren einen macro-F1-Score von 0.92.

FinBERT verbessert sich auf Reddit-Posts, bleibt jedoch aufgrund der kleinen Datenbasis moderat bei F1 ≈ 0.53.

Klassische Verfahren (VADER, TextBlob) liefern auf kurzen Reddit-Kommentaren deutlich schwächere Ergebnisse.

Voraussetzungen: Python 3.9+, Hugging Face Transformers, scikit-learn, datasets, pandas, matplotlib

GPU empfohlen für das Fine-Tuning großer Modelle

## Lizenz
Dieses Projekt ist Teil einer Studienarbeit an der Digital Business University of Applied Sciences.
Die Nutzung der enthaltenen Codesnippets und Visualisierungen ist für akademische Zwecke erlaubt.
Für kommerzielle Anwendungen bitte vorher anfragen.