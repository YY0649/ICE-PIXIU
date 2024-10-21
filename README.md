
# No Language is an Island: Unifying Chinese and English in Financial Large Language Models, Instruction Data, and Benchmarks
=======

**Languages**

[Chinese](https://github.com/YY0649/ICE-PIXIU/blob/master/README.zh.md)


**Disclaimer**

This repository and its contents are for **academic and educational purposes only**. All materials do not constitute financial, legal, or investment advice. No express or implied warranty is provided for the accuracy, completeness, or usefulness of the content. The authors and contributors are not responsible for any errors, omissions, or consequences arising from the use of the information on this website. Users should exercise their own judgment and consult professional advisors before making any financial, legal, or investment decisions. The use of any software and information contained in this repository is entirely at the user's own risk.

**By using or accessing information in this repository, you agree to indemnify, defend, and hold harmless the authors, contributors, and any affiliated organizations or individuals from any and all claims or damages.**

---

## News
**📢 Update (Date: 2024/03/12)**

🐹 We are excited to share our paper, "No Language is an Island: Unifying Chinese and English in Financial Large Language Models, Instruction Data, and Benchmarks".

---

# Overview

**ICE-PIXIU** is our comprehensive framework, featuring the first cross-lingual bilingual financial instruction dataset ICE-FIND, large language model ICE-INTENT, and evaluation benchmark ICE-FLARE. ICE-PIXIU combines various Chinese classification, extraction, reasoning, and prediction financial NLP tasks, enhancing training and performance to address the shortcomings in Chinese financial NLP. It simultaneously integrates a series of translated and original English datasets, enriching the breadth and depth of bilingual financial modeling. It offers unrestricted access to various model variants, a compilation of diverse cross-lingual and multi-modal instruction data, and an evaluation benchmark with expert annotations, encompassing 10 NLP tasks and 20 bilingual specific tasks. Our comprehensive evaluation emphasizes the advantages of combining these bilingual datasets, particularly in translation tasks and leveraging original English data, thereby enhancing language flexibility and analytical acumen in financial contexts.

### Key Features

- **Bilingual Capability**: ICE-INTENT, a component of ICE-PIXIU, excels in Chinese-English bilingual abilities, crucial for global financial data processing and analysis.
- **Diverse Data**: ICE-PIXIU combines various Chinese classification, extraction, reasoning, and prediction NLP tasks, strengthening training and performance to address shortcomings in Chinese financial NLP.
- **Expert Prompts**: ICE-PIXIU offers a set of diverse, high-quality, expert-annotated prompts and adopts similar fine-tuning instructions to enhance understanding of financial tasks.
- **Multilingual**: ICE-PIXIU extends its capabilities by incorporating translation tasks and English datasets, thereby strengthening its bilingual training and application.
- **Cross-lingual Evaluation**: ICE-PIXIU introduces ICE-FLARE, a rigorous cross-lingual evaluation benchmark ensuring consistent model performance across different language contexts.
- **Openness**: ICE-PIXIU adopts an open-access approach, offering resources to the research community to foster collaborative development in financial NLP.

## ICE-FIND: Chinese-English Cross-lingual Instruction Data

#### ICE-PIXIU provides services in various financial scenarios for different user groups with its unique data types, financial tasks, and data sources in Chinese and English bilingual domains.
<p align="center" width="100%">    
<img src="https://i.postimg.cc/hvM78JyB/figure-1.png" width="90%" height="90%">
</p>

#### Sunburst chart describing the distribution of ICE-PIXIU across different language capabilities, data types, financial NLP tasks, specific financial tasks, and datasets
<p align="center" width="100%">
<img src="https://i.postimg.cc/3RYMCvHc/20240311171548.png" width="60%" height="60%">
</p>

**Evaluation Data**            
All our evaluation datasets can be found [here](https://huggingface.co/ICE-PIXIU).

**Datasets (Evaluation Test)**

> Sentiment Analysis(FinSA)
> 
- [ICE-FLARE (zh-FE)](https://huggingface.co/datasets/ICE-PIXIU/FE)
- [ICE-FLARE (zh-stockB)](https://huggingface.co/datasets/ICE-PIXIU/stockB)
- [ICE-FLARE (zh-FPB)](https://huggingface.co/datasets/ChanceFocus/flare-zh-fpb)
- [ICE-FLARE (zh-Fiqasa)](https://huggingface.co/datasets/ChanceFocus/flare-zh-fiqasa)
- [ICE-FLARE (en-FPB)](https://huggingface.co/datasets/ICE-PIXIU/FPB)
- [ICE-FLARE (en-Fiqasa)](https://huggingface.co/datasets/ICE-PIXIU/Fiqasa)
  
> Semantic Matching(FinSM)
- [ICE-FLARE (zh-AFQMC)](https://huggingface.co/datasets/ICE-PIXIU/AFQMC)
- [ICE-FLARE (zh-BQC)](https://huggingface.co/datasets/ICE-PIXIU/corpus)
  
> News Classification(FinNS)
- [ICE-FLARE (zh-NL)](https://huggingface.co/datasets/ICE-PIXIU/NL)
- [ICE-FLARE (zh-NL2)](https://huggingface.co/datasets/ICE-PIXIU/NL2)
  
> Negative Judgment(FinNJ)
- [ICE-FLARE (zh-NSP)](https://huggingface.co/datasets/ICE-PIXIU/NSP)
  
> Answer Selection(FinAS)
- [ICE-FLARE (zh-FinEvalF)](https://huggingface.co/datasets/ICE-PIXIU/fineval)
  
> Relationship Extraction(FinRE)
- [ICE-FLARE (zh-RE)](https://huggingface.co/datasets/ICE-PIXIU/RE)
  
> Headline Classification(FinHC)
- [ICE-FLARE (zh-Headlines)](https://huggingface.co/datasets/ChanceFocus/flare-zh-headlines)
- [ICE-FLARE (en-Headlines)](https://huggingface.co/datasets/ICE-PIXIU/Headlines)
  
> Credit Classification(FinCC)
- [ICE-FLARE (en-German)](https://huggingface.co/datasets/ICE-PIXIU/german)
- [ICE-FLARE (en-Australian)](https://huggingface.co/datasets/ICE-PIXIU/Australian)
> Hawkish-dovish Classification(FinDC)
- [ICE-FLARE (en-FOMC)](https://huggingface.co/datasets/ICE-PIXIU/FOMC)
  
> Event Detection(FinED)
- [ICE-FLARE (zh-19CCKS)](https://huggingface.co/datasets/ICE-PIXIU/CCKS)
- [ICE-FLARE (zh-20CCKS)](https://huggingface.co/datasets/ICE-PIXIU/CCKS)
- [ICE-FLARE (zh-21CCKS)](https://huggingface.co/datasets/ICE-PIXIU/CCKS)
- [ICE-FLARE (zh-22CCKS)](https://huggingface.co/datasets/ICE-PIXIU/CCKS)
  
> Entity Recognition(FinER)
- [ICE-FLARE (zh-NER)](https://huggingface.co/datasets/ICE-PIXIU/cner)
- [ICE-FLARE (en-ner)](https://huggingface.co/datasets/ICE-PIXIU/NER)
- [ICE-FLARE (en-finer-ord)](https://huggingface.co/datasets/ICE-PIXIU/finer-ord)
  
> Question Answering(FinQA)
- [ICE-FLARE (zh-QA)](https://huggingface.co/datasets/ICE-PIXIU/QA)
- [ICE-FLARE (zh-EnQA)](https://huggingface.co/datasets/ChanceFocus/flare-zh-finqa)
- [ICE-FLARE (zh-ConvFinQa)](https://huggingface.co/datasets/ChanceFocus/flare-zh-convfinqa)
- [ICE-FLARE (en-EnQA)](https://huggingface.co/datasets/ICE-PIXIU/Finqa)
- [ICE-FLARE (en-ConvFinQa)](https://huggingface.co/datasets/ICE-PIXIU/convfinqa)
  
> Stock Prediction(FinSF)
- [ICE-FLARE (zh-stockA)](https://huggingface.co/datasets/ICE-PIXIU/stockA)
- [ICE-FLARE (zh-BigData)](https://huggingface.co/datasets/ChanceFocus/flare-zh-bigdata)
- [ICE-FLARE (zh-ACL)](https://huggingface.co/datasets/ChanceFocus/flare-zh-acl)
- [ICE-FLARE (zh-CIKM)](https://huggingface.co/datasets/ChanceFocus/flare-zh-cikm)
- [ICE-FLARE (en-BigData)](https://huggingface.co/datasets/ICE-PIXIU/Bigdata)
- [ICE-FLARE (en-ACL)](https://huggingface.co/datasets/ICE-PIXIU/acl)
- [ICE-FLARE (en-CIKM)](https://huggingface.co/datasets/ICE-PIXIU/cikm)
  
> Text Summarization(FinTS)
- [ICE-FLARE (zh-NA)](https://huggingface.co/datasets/ICE-PIXIU/NA)
- [ICE-FLARE (en-ECTSUM)](https://huggingface.co/datasets/ICE-PIXIU/ectsum)
- [ICE-FLARE (en-EDTSUM)](https://huggingface.co/datasets/ICE-PIXIU/edtsum)

> Adding Cross-Lingual Datasets
- [ICE-FLARE (BCIKM18)](https://huggingface.co/datasets/ICE-PIXIU/Bcikm)
- [ICE-FLARE (M&A)](https://huggingface.co/datasets/ICE-PIXIU/MA)

**Data Summary Table**: Detailed information on Chinese-English bilingual multi-task financial teaching and evaluation raw data, including language capability (Lang), data type (D_T), NLP task (NLP_T), specific task (S_T), dataset name, instruction data size, evaluation data size, data source, and license information.

<table border= "1" width= "600" align="center">
    <tr bgcolor="#C0C0C0">
        <td align="center">Lang</td>  
        <td align="center">D_T</td>  
        <td align="center">NLP_T</td>  
        <td align="center">S_T</td>  
        <td align="center">Dataset</td>
        <td align="center">Raw</td>  
        <td align="center">Instruction</td>  
        <td align="center">Evaluation</td>  
        <td align="center">Data Source</td>  
        <td align="center">License</td>  
     </tr>
    <tr>
        <td rowspan=25 align="center">ZH</td>  
        <td rowspan=10 align="center">DLC</td>  
        <td rowspan=9 align="center">ZH-CLS</td>  
        <td rowspan=2 align="center">FinSA</td>  
        <td align="center">FE</td>
        <td align="center">18,177</td>
        <td align="center">18,177</td>
        <td align="center">2,020</td>
        <td align="center">social texts</td>
        <td align="center">Public</td>
     </tr>
     <tr>
        <td align="center">StockB</td>
        <td align="center">9,812</td>
        <td align="center">9,812</td>
        <td align="center">1,962</td>
        <td align="center">social texts</td>
        <td align="center">Apache-2.0</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">FinSM</td>  
        <td align="center">BQC</td>
        <td align="center">120,000</td>
        <td align="center">110,000</td>
        <td align="center">10,000</td>
        <td align="center">bank service logs</td>
        <td align="center">Public</td>
     </tr>
     <tr>
        <td align="center">AFQMC</td>
        <td align="center">38,650</td>
        <td align="center">38,650</td>
        <td align="center">4,316</td>
        <td align="center">online chat service</td>
        <td align="center">Apache-2.0</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">FinNC</td>  
        <td align="center">NL</td>
        <td align="center">7,955</td>
        <td align="center">7,955</td>
        <td align="center">884</td>
        <td align="center">news articles</td>
        <td align="center">Public</td>
     </tr>
     <tr>
        <td align="center">NL2</td>
        <td align="center">7,955</td>
        <td align="center">7,955</td>
        <td align="center">884</td>
        <td align="center">news articles</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">FinNJ</td>  
        <td align="center">NSP</td>
        <td align="center">4,499</td>
        <td align="center">4,499</td>
        <td align="center">500</td>
        <td align="center">social texts</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">FinAS</td>  
        <td align="center">FinevalF</td>
        <td align="center">1,115</td>
        <td align="center">1,115</td>
        <td align="center">222</td>
        <td align="center">financial exam</td>
        <td align="center">Apache-2.0</td>
     </tr>
    <tr>
        <td align="center">FinRE</td>  
        <td align="center">RE</td>
        <td align="center">14,973</td>
        <td align="center">14,973</td>
        <td align="center">1,489</td>
        <td align="center">news, entity pairs</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">ZH-PRE</td>  
        <td align="center">FinSP</td>  
        <td align="center">StockA</td>
        <td align="center">14,769</td>
        <td align="center">14,769</td>
        <td align="center">1,477</td>
        <td align="center">news, historical prices</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td rowspan=7 align="center">DLE</td>  
        <td rowspan=6 align="center">ZH-EXT</td>  
        <td align="center">FinQA</td>  
        <td align="center">QA</td>
        <td align="center">22,375</td>
        <td align="center">22,375</td>
        <td align="center">2,469</td>
        <td align="center">QA pairs of news</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">FinER</td>  
        <td align="center">CNER</td>
        <td align="center">1,685</td>
        <td align="center">1,685</td>
        <td align="center">337</td>
        <td align="center">financial reports</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td rowspan=4 align="center">FinED</td>  
        <td align="center">19CCKS</td>
        <td align="center">156,834</td>
        <td align="center">14,674</td>
        <td align="center">2,936</td>
        <td align="center">social texts</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
     <tr>
        <td align="center">20CCKS</td>
        <td align="center">372,810</td>
        <td align="center">45,796</td>
        <td align="center">9,159</td>
        <td align="center">news, reports</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
     <tr>
        <td align="center">21CCKS</td>
        <td align="center">8,000</td>
        <td align="center">7,000</td>
        <td align="center">1,400</td>
        <td align="center">news, reports</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
     <tr>
        <td align="center">22CCKS</td>
        <td align="center">109,555</td>
        <td align="center">59,143</td>
        <td align="center">11,829</td>
        <td align="center">news, reports</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
    <tr>
        <td align="center">ZH-GEN</td>
        <td align="center">FinTS</td>  
        <td align="center">NA</td>
        <td align="center">32,400</td>
        <td align="center">32,400</td>
        <td align="center">3,600</td>
        <td align="center">news, announcements</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td rowspan=8 align="center">DTT</td>  
        <td rowspan=8 align="center">ZH-TRA</td>  
        <td rowspan=2 align="center">FinSA</td>  
        <td align="center">CFPB</td>
        <td align="center">4,845</td>
        <td align="center">4,838</td>
        <td align="center">970</td>
        <td align="center">economic news</td>
        <td align="center">MIT license</td>
     </tr>
     <tr>
        <td align="center">CFiQA-SA</td>
        <td align="center">1,173</td>
        <td align="center">1,143</td>
        <td align="center">233</td>
        <td align="center">news headlines, tweets</td>
        <td align="center">MIT license</td>
     </tr>
    <tr>
        <td rowspan=3 align="center">FinSP</td>  
        <td align="center">CACL</td>
        <td align="center">27,056</td>
        <td align="center">2,555</td>
        <td align="center">511</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">MIT license</td>
     </tr>
     <tr>
        <td align="center">CBigdata</td>
        <td align="center">7,167</td>
        <td align="center">798</td>
        <td align="center">159</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">MIT license</td>
     </tr>
     <tr>
        <td align="center">CCIKM</td>
        <td align="center">4,970</td>
        <td align="center">431</td>
        <td align="center">86</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">MIT license</td>
     </tr>
    <tr>
        <td align="center">FinHC</td>  
        <td align="center">CHeadlines</td>
        <td align="center">102,708</td>
        <td align="center">10,256</td>
        <td align="center">2,051</td>
        <td align="center">news headlines</td>
        <td align="center">MIT license</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">FinQA</td>  
        <td align="center">CEnQA</td>
        <td align="center">8,281</td>
        <td align="center">668</td>
        <td align="center">133</td>
        <td align="center">earnings reports</td>
        <td align="center">MIT license</td>
     </tr>
     <tr>
        <td align="center">CConvFinQA</td>
        <td align="center">12,594</td>
        <td align="center">1,189</td>
        <td align="center">237</td>
        <td align="center">earnings reports</td>
        <td align="center">MIT license</td>
     </tr>
    <tr>
        <td rowspan=25 align="center">EN</td>  
        <td rowspan=11 align="center">DTE</td>  
        <td rowspan=5 align="center">EN-CLS</td>  
        <td rowspan=2 align="center">FinSA</td>  
        <td align="center">FPB</td>
        <td align="center">4,845</td>
        <td align="center">4,845</td>
        <td align="center">970</td>
        <td align="center">economic news</td>
        <td align="center">CC BY-SA 3.0</td>
     </tr>
     <tr>
        <td align="center">FiQA-SA</td>
        <td align="center">1,173</td>
        <td align="center">1,173</td>
        <td align="center">235</td>
        <td align="center">news headlines, tweets</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">FinHC</td>  
        <td align="center">Headlines</td>
        <td align="center">11,412</td>
        <td align="center">102,708</td>
        <td align="center">20,547</td>
        <td align="center">news headlines</td>
        <td align="center">CC BY-SA 3.0</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">FinCC</td>  
        <td align="center">German</td>
        <td align="center">1,000</td>
        <td align="center">1,000</td>
        <td align="center">200</td>
        <td align="center">credit records</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
     <tr>
        <td align="center">Australian</td>
        <td align="center">690</td>
        <td align="center">690</td>
        <td align="center">139</td>
        <td align="center">credit records</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
    <tr>
        <td rowspan=3 align="center">EN-PRE</td>  
        <td rowspan=3 align="center">FinSP</td>  
        <td align="center">ACL18</td>
        <td align="center">27,053</td>
        <td align="center">27,053</td>
        <td align="center">3,720</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">MIT License</td>
     </tr>
     <tr>
        <td align="center">BigData22</td>
        <td align="center">7,164</td>
        <td align="center">7,164</td>
        <td align="center">1,472</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">Public</td>
     </tr>
     <tr>
        <td align="center">CIKM18</td>
        <td align="center">4,967</td>
        <td align="center">4,967</td>
        <td align="center">1,143</td>
        <td align="center">tweets, historical prices</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">EN-EXT</td>  
        <td align="center">FinER</td>  
        <td align="center">NER</td>
        <td align="center">609</td>
        <td align="center">609</td>
        <td align="center">98</td>
        <td align="center">financial agreements</td>
        <td align="center">CC BY-SA-3.0</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">EN-REA</td>  
        <td rowspan=2 align="center">FinQA</td>  
        <td align="center">EnQA</td>
        <td align="center">8,281</td>
        <td align="center">8,281</td>
        <td align="center">1,147</td>
        <td align="center">earnings reports</td>
        <td align="center">MIT License</td>
     </tr>
     <tr>
        <td align="center">ConvFinQA</td>
        <td align="center">3,458</td>
        <td align="center">12,594</td>
        <td align="center">1,490</td>
        <td align="center">earnings reports</td>
        <td align="center">MIT License</td>
     </tr>
    <tr>
        <td rowspan=5 align="center">DOF</td>
        <td rowspan=5 align="center">EN-DOF</td>  
        <td align="center">FinER</td>  
        <td align="center">Finer-Ord</td>
        <td align="center">1,075</td>
        <td align="center">-</td>
        <td align="center">1,075</td>
        <td align="center">news articles</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
    <tr>
        <td rowspan=2 align="center">FinTS</td>  
        <td align="center">ECTSUM</td>
        <td align="center">495</td>
        <td align="center">-</td>
        <td align="center">495</td>
        <td align="center">earning call transcripts</td>
        <td align="center">Public</td>
     </tr>
     <tr>
        <td align="center">EDTSUM</td>
        <td align="center">2,000</td>
        <td align="center">-</td>
        <td align="center">2,000</td>
        <td align="center">news articles</td>
        <td align="center">Public</td>
     </tr>
    <tr>
        <td align="center">FinDC</td>  
        <td align="center">FOMC</td>
        <td align="center">496</td>
        <td align="center">-</td>
        <td align="center">496</td>
        <td align="center">FOMC transcripts</td>
        <td align="center">CC BY-SA 4.0</td>
     </tr>
</table>


## ICE-INTERN: Bilingual Financial Large Model

- [ICE-INTERN-7B (Instruction-tuned model with all DLC data)](https://huggingface.co/jasion/ICE-INTERN-dlc-7B)
- [ICE-INTERN-7B (Instruction-tuned model with all DCL+DLE data)](https://huggingface.co/jasion/ICE-INTERN-dle-7B)
- [ICE-INTERN-7B (Instruction-tuned model with all DCL+DLE+DTT data)](https://huggingface.co/jasion/ICE-INTERN-dtt-7B)
- [ICE-INTERN-7B (Instruction-tuned model with all instruction data)](https://huggingface.co/jasion/ICE-INTERN-Full-7B)

During the fine-tuning process, we employed QLoRA, an efficient parameter tuning technique, using a uniform sequence length of 2048 tokens. The fine-tuning process utilized the AdamW optimizer with an initial learning rate of 5e-5 and a weight decay of 1e-5, along with a 1% total step warm-up. All models underwent one round of fine-tuning on eight A100 40GB GPUs with a batch size of 24, using consistent hyperparameter settings.



## ICE-FLARE: Cross-Language Financial Evaluation Benchmark

In order to conduct comparative analysis with other general large models (including Baichuan, ChatGPT, Qwen, etc.) and financial large models, we have selected a series of tasks and metrics that cover various aspects of financial natural language processing and financial forecasting.

### Tasks

| Data                  | Task                             | Raw    | Data Types                | Modalities        | License         | Paper |
| --------------------- | -------------------------------- | ------ | ------------------------- | ----------------- | --------------- | ----- |
| AFQMC                 | Semantic Matching                | 38,650 | Question Data, Dialogue   | Text              | Apache-2.0      | [1]   |
| corpus                | Semantic Matching                | 120,000| Question Data, Dialogue   | Text              | Public          | [2]   |
| stockA                | Stock Classification             | 14,769 | News, Historical Prices   | Text, Time Series  | Public          | [3]   |
| Fineval               | Multiple Choice                  | 1,115  | Financial Exams           | Text              | Apache-2.0      | [4]   |
| NL                    | News Classification              | 7,955  | News Reports              | Text              | Public          | [5]   |
| NL2                   | News Classification              | 7,955  | News Reports              | Text              | Public          | [5]   |
| NSP                   | Negative News Judgement          | 4,499  | News, Social Media Text   | Text              | Public          | [5]   |
| RE                    | Relation Extraction              | 14,973 | News, Entity Pair         | Text              | Public          | [5]   |
| FE                    | Sentiment Analysis               | 18,177 | Financial Social Media Text| Text              | Public          | [5]   |
| stockB                | Sentiment Analysis               | 9,812  | Financial Social Media Text| Text              | Apache-2.0      | [6]   |
| QA                    | Financial Q&A                    | 22,375 | Financial News Announcements| Text, Tables      | Public          | [5]   |
| NA                    | Text Summarization              | 32,400 | News Articles, Announcements| Text              | Public          | [5]   |
| 19CCKS                | Event Subject Extraction         | 156,834| News Reports              | Text              | CC BY-SA 4.0    | [7]   |
| 20CCKS                | Event Subject Extraction         | 372,810| News Reports              | Text              | CC BY-SA 4.0    | [8]   |
| 21CCKS                | Event Causal Relationship Extraction| 8,000| News Reports              | Text              | CC BY-SA 4.0    | [9]   |
| 22CCKS                | Event Subject Extraction         | 109,555| News Reports              | Text              | CC BY-SA 4.0    | [10]  |
| CNER                  | Named Entity Recognition         | 1,685  | News Reports              | Text              | Public          | [11]  |
| CFPB                  | Sentiment Analysis               | 4,845  | News                      | Text              | MIT license     | [12]  |
| CFIQASA               | Sentiment Analysis               | 1,173  | News Headlines, Tweets     | Text              | MIT license     | [12]  |
| CHeadlines            | News Headline Classification     | 11,412 | News Headlines            | Text              | MIT license     | [12]  |
| CBigData              | Stock Trend Prediction           | 7,164  | Tweets, Historical Prices | Text, Time Series  | MIT license     | [12]  |
| CACL                  | Stock Trend Prediction           | 27,053 | Tweets, Historical Prices | Text, Time Series  | MIT license     | [12]  |
| CCIKM                 | Stock Trend Prediction           | 4,967  | Tweets, Historical Prices | Text, Time Series  | MIT license     | [12]  |
| CFinQA                | Financial Q&A                    | 14,900 | Earnings Reports          | Text, Tables      | MIT license     | [12]  |
| CConvFinQA            | Multi-Turn Q&A                   | 48,364 | Earnings Reports          | Text, Tables      | MIT license     | [12]  |

1. Xu L, Hu H, Zhang X, et al. CLUE: A Chinese language understanding evaluation benchmark[J]. arXiv preprint arXiv:2004.05986, 2020.
2. Jing Chen, Qingcai Chen, Xin Liu, Haijun Yang, Daohe Lu, and Buzhou Tang. 2018. The BQ Corpus: A Large-scale Domain-specific Chinese Corpus For Sentence Semantic Equivalence Identification. In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pages 4946–4951, Brussels, Belgium. Association for Computational Linguistics.
3. Jinan Zou, Haiyao Cao, Lingqiao Liu, Yuhao Lin, Ehsan Abbasnejad, and Javen Qinfeng Shi. 2022. Astock: A New Dataset and Automated Stock Trading based on Stock-specific News Analyzing Model. In Proceedings of the Fourth Workshop on Financial Technology and Natural Language Processing (FinNLP), pages 178–186, Abu Dhabi, United Arab Emirates (Hybrid). Association for Computational Linguistics.
4. Zhang L, Cai W, Liu Z, et al. FinEval: A Chinese Financial Domain Knowledge Evaluation Benchmark for Large Language Models[J]. arxiv preprint arxiv:2308.09975, 2023.
5. Lu D, Liang J, Xu Y, et al. BBT-Fin: Comprehensive Construction of Chinese Financial Domain Pre-trained Language Model, Corpus and Benchmark[J]. arxiv preprint arxiv:2302.09432, 2023.
6. https://huggingface.co/datasets/kuroneko5943/stock11
7. https://www.biendata.xyz/competition/ccks_2019_4/
8. https://www.biendata.xyz/competition/ccks_2020_4_1/
9. https://www.biendata.xyz/competition/ccks_2021_task6_2/
10. https://www.biendata.xyz/competition/ccks2022_eventext/
11. Jia C, Shi Y, Yang Q, et al. Entity enhanced BERT pre-training for Chinese NER[C]//Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP). 2020: 6384-6396.
12. Xie Q, Han W, Zhang X, et al. PIXIU: A Large Language Model, Instruction Data and Evaluation Benchmark for Finance[J]. arXiv preprint arXiv:2306.05443, 2023.


----

**Benchmark Evaluation Environment Deployment**

##### Local Installation

```bash
git clone https://github.com/chancefocus/PIXIU.git --recursive
cd PIXIU
pip install -r requirements.txt
cd PIXIU/src/financial-evaluation
pip install -e .[multilingual]
```
##### Docker Image
```bash
sudo bash scripts/docker_run.sh
```

The above command will start a Docker container. You can modify `docker_run.sh` according to your own environment. We provide the pre-compiled image by running `sudo docker pull tothemoon/pixiu:latest`.

```bash
docker run --gpus all --ipc=host --ulimit memlock=-1 --ulimit stack=67108864 \
    --network host \
    --env https_proxy=$https_proxy \
    --env http_proxy=$http_proxy \
    --env all_proxy=$all_proxy \
    --env HF_HOME=$hf_home \
    -it [--rm] \
    --name pixiu \
    -v $pixiu_path:$pixiu_path \
    -v $hf_home:$hf_home \
    -v $ssh_pub_key:/root/.ssh/authorized_keys \
    -w $workdir \
    $docker_user/pixiu:$tag \
    [--sshd_port 2201 --cmd "echo 'Hello, world!' && /bin/bash"]
```
Parameter Description:
- `[]` indicates optional parameters
- `HF_HOME`: Hugging Face cache directory
- `sshd_port`: The SSHD port of the container. You can run `ssh -i private_key -p $sshd_port root@$ip` to connect to the container. The default is 22001.
- `--rm`: Remove the container upon exit (i.e., `CTRL + D`).

#### Automated Task Evaluation
Before evaluation, please download the [BART checkpoint](https://drive.google.com/u/0/uc?id=1_7JfF7KOInb7ZrxKHIigTMR4ChVET01m&export=download) to `src/metrics/BARTScore/bart_score.pth`.

To perform automatic evaluation, please follow the instructions below:

1. Hugging Face Transformer

To evaluate models hosted on the Hugging Face Hub (e.g., ICE-INTERN-Full-7B), please use this command:

```bash
python eval.py \
    --model "hf-causal-llama" \
    --model_args "use_accelerate=True,pretrained=chancefocus/finma-7b-full,tokenizer=chancefocus/finma-7b-full,use_fast=False" \
    --tasks "flare_ner,flare_sm_acl,flare_fpb"
```

For more details, please refer to the [lm_eval](https://github.com/EleutherAI/lm-evaluation-harness) documentation.

2. Commercial API

Please note that for tasks such as NER, automatic evaluation is based on specific patterns. This may not extract relevant information in zero-shot settings, resulting in performance that is relatively lower than previous human-annotated results.

```bash
export OPENAI_API_SECRET_KEY=YOUR_KEY_HERE
python eval.py \
    --model gpt-4 \
    --tasks flare_zh_fe,flare_cner,flare_sm_acl
```

3. Self-Hosted Evaluation

To run the inference backend, please execute the following command:
```bash
bash scripts/run_interface.sh
```

#### Predefined Task Metrics

| Task                                     | Metric                                 | Illustration                                                 |
| ---------------------------------------- | -------------------------------------- | ------------------------------------------------------------ |
| Classification                           | Accuracy                               | This metric represents the ratio of correctly predicted observations to the total observations. The calculation formula is (correct predictions + incorrect predictions) / total observations. |
| Classification                           | F1 Score                               | The F1 score represents the harmonic mean of precision and recall, achieving a balance between these two factors. It is particularly useful when one factor is more important than the other. The score ranges from 0 to 1, where 1 indicates perfect precision and recall, and 0 indicates the worst case. Additionally, we provide "weighted" and "macro" versions of the F1 score. |
| Classification                           | Missing Ratio                          | This metric calculates the proportion of responses that did not return any option among the given options in the task. |
| Classification                           | Matthews Correlation Coefficient (MCC) | MCC is a metric for assessing the quality of binary classification, with scores ranging from -1 to +1. A score of +1 indicates perfect prediction, 0 indicates no better than random chance, and -1 indicates completely opposite predictions. |
| Sequence Labeling                        | F1 Score                               | In "sequence labeling" tasks, we use the F1 score calculated by the "seqeval" library, which is a robust entity-level evaluation metric. This metric requires a complete match of entity spans and types between predicted entities and ground truth entities for correct evaluation. True positives (TP) represent correctly predicted entities, false positives (FP) represent incorrectly predicted entities or spans/types that do not match, and false negatives (FN) represent entities missed from the ground truth. These quantities are then used to calculate precision, recall, and F1 score, where the F1 score represents the harmonic mean of precision and recall. |
| Sequence Labeling                        | Label F1 Score                         | This metric evaluates model performance solely based on the correctness of predicted labels, without considering entity spans. |
| Relation Extraction                      | Precision                              | Precision measures the proportion of correctly predicted relations among all predicted relations. It is calculated as the number of true positives (TP) divided by the total of true positives and false positives (FP). |
| Relation Extraction                      | Recall                                 | Recall measures the proportion of correctly predicted relations among all actual relations. It is calculated as the number of true positives (TP) divided by the total of true positives and false negatives (FN). |
| Relation Extraction                      | F1 Score                               | The F1 score is the harmonic mean of precision and recall, achieving a balance between these two metrics. The F1 score is best at 1 (both precision and recall are perfect) and worst at 0. |
| Extractive and Abstractive Summarization | Rouge-L                                | This metric assesses the longest common subsequence (LCS) between the system and the reference summary. The LCS naturally considers structural similarity at the sentence level and automatically identifies the longest co-occurring n-gram. |
| Extractive and Abstractive Summarization | Rouge-N                                | It measures the overlap of N-grams (a continuous sequence of N items in the given text sample) between the system-generated summary and the reference summary. "N" can be 1, 2, or more; ROUGE-1 and ROUGE-2 are typically used to evaluate unigram overlap and bigram overlap, respectively. |
| Question Answering                      | EMACC                                  | EMACC evaluates the exact match between the model-generated answer and the reference answer. In other words, a model-generated answer is considered correct only if it matches the reference answer exactly. |

---

#### Sample Input and Output for Specific Tasks
For specific financial tasks such as Question Answering (FinQA), Text Summarization (FinTS), Relation Extraction (FinRE), Event Detection (FinED), Entity Recognition (FinER), and News Classification (FinNC), various LLM input and response examples are provided.

| Task       | Query                      |     Baichuan-7B   |     GPT-4      |    ICE-INTERN-full-7B    |
| ---------- | -------------------------- | ----------------- | -------------- | ------------------------ |
|FinQA       |浦东建设公告，公司子公司上海市浦东新区建设（集团）有限公司、上海浦兴路桥建设工程有限公司中标多项重大工程项目，中标金额总计为10.94亿元。***请问中标事件对应的主体有哪些?***|浦东建设、浦兴路桥、浦东建设(集团)|中标事件对应的主体有上海市浦东新区建设（集团）有限公司|上海市浦东新区建设（集团）有限公司,上海浦兴路桥建设工程有限公司|
|FinTS       |市场普遍预期日本央行将维持其超宽松货币政策不变，但知情人士表示，周二将公布的经济展望报告中，可能上调4月起财政年度的通胀预估。能源和原材料成本的上涨已将批发价格推高至40年来的最高水平，企业已开始将上涨的成本转嫁给消费者。近期通胀温和上升，主要是投入成本上升和日元疲软推动的，而不是强劲的国内需求。日本央行行长黑田东彦曾表示，物价上涨应该伴随着工资的强劲增长。***请对上述金融报道进行总结，给出具有中心主旨的摘要，回答要求尽量简短。***|日本央行行长黑田东彦曾表示，物价上涨应该伴随着工资的强劲增长。|日本央行预计将上调4月起的通胀预估，尽管市场普遍预期货币政策将保持超宽松。成本上涨推高批发价格，企业已将涨成本转嫁给消费者，但通胀主要由投入成本上升和日元疲软推动，而非国内需求强劲。|知情人士：日本央行可能上调4月起财政年度的通胀预估。|
|FinRE       |新希望集团销售额约为上市公司<N>倍有余,由于背靠农业帝国“希望系”, 资本市场一直预期集团能够向新希望股份注入农业资产, 如果集团资产整合启动, 新希望股份的股。***请分析上述涉及实体对(新希望股份,新希望集团)的关系。***|被收购|被注资|自己|
|FinED       |大智慧(601519)信披违规遭调查“互联网+”炒作或终结金鹰等多家基金公司高管离职 基民担忧业绩波动。***请分析上述金融报道中的事件类型及及其事件主体，并以‘事件类型，事件主体’的格式输出。***|套现约1.5亿元|交易违规, 大智慧|信批违规, 大智慧|
|FinER       |本公司非执行董事孙月英女士不再担任中国远洋海运集团有限公司总会计师和中远财务有限责任公司董事长。***请给出上述金融报道中存在的个人(’PER’)、组 织(’ORG’)或地点(’LOC’)的特定命 名实体，回答应遵循的格式’实体名称, 实体类型’。***|中国远洋海运集团有限公司，ORG|中远海运发展股份有限公司, ORG|孙月英, PER;中国远洋海运集团有限公司, ORG;中远财务有限责任公司, ORG|
|FinNC       |WTI原油涨幅回升至0.5\%，现报75.58美元/桶。***请对该金融报道进行分类，具体属于['中国','外国','国际','公司','行业','大盘','经济','政策','政治','期货','债券','房地产','外汇','虚拟货币','新冠','能源']中的哪些类别？***|~输出与内容无关~|国际,能源|国际期货|


## Citation

If you use ICE-PIXIU in your project, please cite our article.

```

```

---

## License

ICE-PIXIU is licensed under the [MIT] license. For details, please refer to the [MIT](LICENSE) file.
