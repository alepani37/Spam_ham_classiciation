# Spam_ham_classiciation

Materiale del progetto per il corso di Deep Learning and Applications

# Prerequisiti ed installazione

-Python >= 3.11

### 1. Clonazione della repository

```bash
git clone https://github.com/alepani37/Spam_ham_classiciation
cd Spam_ham_classiciation
```

### 2. Crea un ambiente virtuale

### 🪟 Windows (CMD o PowerShell)

```bash
python3.11 -m venv venv
venv\Scripts\activate
```

### 🍎 macOS

```bash
python3.11 -m venv venv
source venv/bin/activate
```

### 🐧 Ubuntu/Linux

```bash
sudo apt update
sudo apt install python3-venv -y
python3.11 -m venv venv
source venv/bin/activate
```

### 3. Installazione delle dipendenze

#### IF SE USI COLAB IGNORA QUESTA SEZIONE E INSTALLA SOLO QUESTI DUE PACCHETTI:
```bash
!pip install peft
```

```bash
!pip install --quiet bitsandbytes
```

#### 3.1 Installazione di torch
```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

#### 3.2 Installazione delle altre librerie

```bash
pip install -r requirements.txt
```

### 4. Avvio di Jupyter Notebook

### Se Jupyter non è installato:

```bash
pip install notebook
```

### Scaricare i modelli

Scaricare al link https://1drv.ms/u/c/9e23e1a65fd6baef/EfZ_9ENVUExPlSxMf_8E6nUBaAoNjz7F1ahsjEScCi3Mbw?e=qNuOHj tlo zip, estrarlo e inserire singolarmente nella cartella Spam_ham_classiciation tutti i file e cartelle presenti nella cartella appena decompressa.

### Avvia il server Jupyter:

```bash
jupyter notebook
```

#Struttura del progetto

Se usi Colab ricorda di aggiungere ad ogni path Spam_ham_classiciation/

-/data #Il file csv contenente il dataset
-bert_fine_tuned.ipynb #il notebook per fare fine tuning e test di bert, di default PRE_TRAINED è true, in modo da usare i pesi del modello già fine-tunato.

-roberta_fine_tuned.ipynb #il notebook per fare fine tuning e test di roberta, di default PRE_TRAINED è true, in modo da usare i pesi del modello già fine-tunato.

-llama_fine_tuned.ipynb #il notebook per fare fine tuning e test di llama, di default PRE_TRAINED è true, in modo da usare i pesi del modello già fine-tunato. IMPORTANTE: inserire il proprio token di huggingface.

-phi_fine_tuned.ipynb #il notebook per fare fine tuning e test di phi, di default PRE_TRAINED è true, in modo da usare i pesi del modello già fine-tunato.IMPORTANTE: inserire il proprio token di huggingface.

-llama_infer.ipynb #il notebook per fare fine per fare test zero shot su Llama.IMPORTANTE: inserire il proprio token di huggingface.

-phi_infer.ipynb #il notebook per fare fine per fare test zero shot su Phi.IMPORTANTE: inserire il proprio token di huggingface.

