# HKU-Captone
Patents-to-Products: Knowledge Evolution in Medical devices  
Online docs:https://www.dropbox.com/scl/fi/zz8ccrotmif4yf3ldvn93/MscAI-Capstone-Patents-to-Products.gdoc?dl=0&rlkey=79k831jugyqy8oai6o1kas24q

## Abbreviations in different parts
### FDA 510k
1. SE: Substantially Equivalent(实质等同), 在食品安全方面，实质等同性概念认为，可以通过将一种新食品（特别是经过基因改造的食品）与类似的传统食品进行比较来评估其安全性，这种传统食品已被证明随着时间的推移可以正常使用。(wiki)
2. PMA: Premarket approval (PMA) is the FDA process of scientific and regulatory review to evaluate the safety and effectiveness of Class III medical devices.(https://www.fda.gov/medical-devices/premarket-submissions-selecting-and-preparing-correct-submission/premarket-approval-pma)

### Patentsview
1. CPC: Cooperative Patent Classification, CPC is the name of the new patent classification system jointly developed by the EPO and USPTO launched in 2010. At the EPO, the CPC replaces the ECLA classification scheme, and at the USPTO it replaces the USPC scheme.
2. USPC: U.S. Patent Classification, basically another patent classification scheme.
3. NBER: National Bureau of Economic Research, another patent classification scheme.

According to the below image, should basically using CPC and IPC system.
<img width="716" alt="availability table" src="https://github.com/TiaolyuShi/HKU-Captone/assets/81952160/48852bff-64f4-49e1-b8f8-2121136d021f">

## Timeline
### 23/5/19
1. Literature review and reconsider the framework
2. Data perspective: How to obtain the data?
    patents data: from patentsview using API
    (Test case passed.)
    products/devices data: combine fda-510k and device classification together to get more detailed description

3. How to link patents with products?
    products to patents: Using applicants' name to match several patents
    patents to products: The device classification dataset contains the device type, which is a clustering itself. We are trying to use the patents' abstract to match wiki-based description of certain device types. The idea comes from Argente D, et al. Patents to products: Product innovation and firm dynamics[J]. 2020. 

### 23/6/7
