#### Data
1. iFind: public data downloaded from iFind, including *ADA_Data_Fund.xlsx*, *ADA_Data_Fund_Company.xlsx*, *ADA_Data_Fund_Manager.xlsx*. (data have been processed with Excel)
2. AMAC: Asset Management Association of China; mainly photos and work experiences of fund managers by web crawling, including *ADA_Data_Fund_Manager_Infos.xlsx*.
3. $\text{Face}^{++}$: facial attractiveness scores by algorithms in $\text{Face}^{++}$, including *ADA_Data_Fund_Manager_Scores.csv*.

#### Code
1. Web Crawling: Managers_infos&photos_Crawling.ipynb, crawling data from [AMAC](https://gs.amac.org.cn/amac-infodisc/res/pof/person/personOrgList.html"基金经理从业信息，含照片"); code in *Managers_infos&photos_Crawling.ipynb*
2. Scroing: utilizing API of [FacePlusPlus](https://console.faceplusplus.com.cn/documents/4888373"技术文档") to obtain scores of managers' facial attractiveness; code in *Score.ipynb*
3. Previous Experience: use history of managers work experience from AMAC's website to calculate previous experience before current job; code in *Calculate_Experience_before_Curr.ipynb*
4. Data Processing: cleaning, calculation, merging; code in *Managers_infos&photos_Crawling.ipynb*

#### Output
Manager-level data, including a manager's information, facial attractiveness, information of company where th manager works in, funds' aggregate information which the manager managed. See *ADA_Data_V3.csv*.
