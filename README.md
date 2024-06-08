# COVID-19 Articles Analysis Project
This repository contains a Jupyter Notebook for analyzing articles related to the coronavirus. The notebook includes data preprocessing, exploration, and modeling to analyze trends, sentiments, and key topics within the collected articles.
## The main objectives of this project are:
- Introduction: Overview of the project and objectives.
- Data Loading: Load the dataset and necessary libraries.
- Data Preprocessing: Clean and prepare the data for analysis, including text cleaning and normalization.
- Natural Language Processing (NLP): Apply NLP techniques such as tokenization, stemming, lemmatization, and stopwords removal.
- Feature Extraction: Use TF-IDF to extract features from the text data.
- Dimensionality Reduction: Apply PCA to reduce the dimensionality of TF-IDF features.
- Clustering: Perform K-means clustering to group similar articles.
- Cluster Evaluation: Evaluate the clusters using metrics like Silhouette Score and Davies-Bouldin Index.
- Visualization: Visualize the clusters using t-SNE and create an interactive plot using Plotly.
- Topic Modeling: Apply LDA to extract topics from the clusters.
## Data
The dataset consists of articles related to the coronavirus. It includes various features such as the publication date, article content, and metadata. The data preprocessing section involves cleaning the text data, handling missing values, and normalizing the text for analysis.

## Results

### Key topics discussed in the articles examplr
Cluster 1:
Topic 1: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 2: lncrnas, cis, utr, noncod, rnas, outdoor, neighbor, nest, enforc, pol
Topic 3: cell, mice, express, immun, respons, activ, infect, ace, lung, cytokin
Topic 4: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 5: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo

Cluster 2:
Topic 1: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 2: sirna, pdcov, knockdown, rnai, silenc, appendix, mainland, los, stream, organell
Topic 3: sequenc, genom, virus, use, rna, sampl, gene, assay, primer, strain
Topic 4: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 5: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag

## t-SNE Visualization of TF-IDF Features with Cluster Labels

## Cluster Visualization
[Uploadi<!DOCTYPE html>
<!-- saved from url=(0095)https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId#scrollTo=ZMLknF7HJ1qH -->
<html lang="en" theme="adaptive" style="--colab-code-font-family: monospace;" editor="Default Light"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8"><meta http-equiv="origin-trial" content="Az520Inasey3TAyqLyojQa8MnmCALSEU29yQFW8dePZ7xQTvSt73pHazLFTK5f7SyLUJSo2uKLesEtEa9aUYcgMAAACPeyJvcmlnaW4iOiJodHRwczovL2dvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZyIsImV4cGlyeSI6MTcyNTQwNzk5OSwiaXNTdWJkb21haW4iOnRydWUsImlzVGhpcmRQYXJ0eSI6dHJ1ZX0="><meta http-equiv="origin-trial" content="Az520Inasey3TAyqLyojQa8MnmCALSEU29yQFW8dePZ7xQTvSt73pHazLFTK5f7SyLUJSo2uKLesEtEa9aUYcgMAAACPeyJvcmlnaW4iOiJodHRwczovL2dvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZyIsImV4cGlyeSI6MTcyNTQwNzk5OSwiaXNTdWJkb21haW4iOnRydWUsImlzVGhpcmRQYXJ0eSI6dHJ1ZX0="><script type="text/javascript" async="" src="./DataMining_Project3_HSM.ipynb - Colab_files/recaptcha__en.js.download" crossorigin="anonymous" integrity="sha384-35beLYB8J+E3oW9vsZdrYlTMm/yJU76vKQNSwKHtb4Ug7VeAPwqIzHBRAOMwbzRb" nonce=""></script><script type="text/javascript" async="" src="./DataMining_Project3_HSM.ipynb - Colab_files/recaptcha__en.js.download" crossorigin="anonymous" integrity="sha384-35beLYB8J+E3oW9vsZdrYlTMm/yJU76vKQNSwKHtb4Ug7VeAPwqIzHBRAOMwbzRb" nonce=""></script><script type="text/javascript" async="" src="./DataMining_Project3_HSM.ipynb - Colab_files/js" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/cb=gapi.loaded_1" nonce="" async=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/cb=gapi.loaded_0" nonce="" async=""></script><script async="" src="./DataMining_Project3_HSM.ipynb - Colab_files/analytics.js.download"></script><script nonce="">
      document.addEventListener('keydown', (e) => {
        // Stop propagation on ESC because otherwise it will halt outbound XHRs
        // See b/131755324 for more info.
        if (e.key === 'Escape') {
          e.stopPropagation();
          e.preventDefault();
        }
      });
    </script><meta name="referrer" content="origin"><meta name="viewport" content="width=device-width, initial-scale=1"><title>DataMining_Project3_HSM.ipynb - Colab</title><link href="./DataMining_Project3_HSM.ipynb - Colab_files/css2" rel="stylesheet"><link href="./DataMining_Project3_HSM.ipynb - Colab_files/css" rel="stylesheet"><link rel="search" type="application/opensearchdescription+xml" href="https://colab.research.google.com/opensearch.xml" title="Google Colab"><style>.gb_ib:not(.gb_kd){font:13px/27px Roboto,Arial,sans-serif;z-index:986}@-webkit-keyframes gb__a{0%{opacity:0}50%{opacity:1}}@keyframes gb__a{0%{opacity:0}50%{opacity:1}}a.gb_za{border:none;color:#4285f4;cursor:default;font-weight:bold;outline:none;position:relative;text-align:center;text-decoration:none;text-transform:uppercase;white-space:nowrap;-webkit-user-select:none}a.gb_za:hover:after,a.gb_za:focus:after{background-color:rgba(0,0,0,.12);content:"";height:100%;left:0;position:absolute;top:0;width:100%}a.gb_za:hover,a.gb_za:focus{text-decoration:none}a.gb_za:active{background-color:rgba(153,153,153,.4);text-decoration:none}a.gb_Aa{background-color:#4285f4;color:#fff}a.gb_Aa:active{background-color:#0043b2}.gb_Ba{box-shadow:0 1px 1px rgba(0,0,0,.16)}.gb_za,.gb_Aa,.gb_Ca,.gb_Da{display:inline-block;line-height:28px;padding:0 12px;border-radius:2px}.gb_Ca{background:#f8f8f8;border:1px solid #c6c6c6}.gb_Da{background:#f8f8f8}.gb_Ca,#gb a.gb_Ca.gb_Ca,.gb_Da{color:#666;cursor:default;text-decoration:none}#gb a.gb_Da{cursor:default;text-decoration:none}.gb_Da{border:1px solid #4285f4;font-weight:bold;outline:none;background:#4285f4;background:-webkit-gradient(linear,left top,left bottom,from(top),color-stop(#4387fd),to(#4683ea));background:-webkit-linear-gradient(top,#4387fd,#4683ea);background:linear-gradient(top,#4387fd,#4683ea);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#4387fd,endColorstr=#4683ea,GradientType=0)}#gb a.gb_Da{color:#fff}.gb_Da:hover{box-shadow:0 1px 0 rgba(0,0,0,.15)}.gb_Da:active{box-shadow:inset 0 2px 0 rgba(0,0,0,.15);background:#3c78dc;background:-webkit-gradient(linear,left top,left bottom,from(top),color-stop(#3c7ae4),to(#3f76d3));background:-webkit-linear-gradient(top,#3c7ae4,#3f76d3);background:linear-gradient(top,#3c7ae4,#3f76d3);filter:progid:DXImageTransform.Microsoft.gradient(startColorstr=#3c7ae4,endColorstr=#3f76d3,GradientType=0)}#gb .gb_Ea{background:#fff;border:1px solid #dadce0;color:#1a73e8;display:inline-block;text-decoration:none}#gb .gb_Ea:hover{background:#f8fbff;border-color:#dadce0;color:#174ea6}#gb .gb_Ea:focus{background:#f4f8ff;color:#174ea6;outline:1px solid #174ea6}#gb .gb_Ea:active,#gb .gb_Ea:focus:active{background:#ecf3fe;color:#174ea6}#gb .gb_Ea.gb_i{background:transparent;border:1px solid #5f6368;color:#8ab4f8;text-decoration:none}#gb .gb_Ea.gb_i:hover{background:rgba(255,255,255,.04);color:#e8eaed}#gb .gb_Ea.gb_i:focus{background:rgba(232,234,237,.12);color:#e8eaed;outline:1px solid #e8eaed}#gb .gb_Ea.gb_i:active,#gb .gb_Ea.gb_i:focus:active{background:rgba(232,234,237,.1);color:#e8eaed}.gb_m{display:none!important}.gb_3a{visibility:hidden}.gb_x{display:inline-block;vertical-align:middle}.gb_Sd .gb_q{bottom:-3px;right:-5px}.gb_f{position:relative}.gb_d{display:inline-block;outline:none;vertical-align:middle;border-radius:2px;box-sizing:border-box;height:40px;width:40px;cursor:pointer;text-decoration:none}#gb#gb a.gb_d{cursor:pointer;text-decoration:none}.gb_d,a.gb_d{color:#000}.gb_if{border-color:transparent;border-bottom-color:#fff;border-style:dashed dashed solid;border-width:0 8.5px 8.5px;display:none;position:absolute;left:11.5px;top:33px;z-index:1;height:0;width:0;-webkit-animation:gb__a .2s;animation:gb__a .2s}.gb_jf{border-color:transparent;border-style:dashed dashed solid;border-width:0 8.5px 8.5px;display:none;position:absolute;left:11.5px;z-index:1;height:0;width:0;-webkit-animation:gb__a .2s;animation:gb__a .2s;border-bottom-color:rgba(0,0,0,.2);top:32px}x:-o-prefocus,div.gb_jf{border-bottom-color:#ccc}.gb_6{background:#fff;border:1px solid #ccc;border-color:rgba(0,0,0,.2);color:#000;-webkit-box-shadow:0 2px 10px rgba(0,0,0,.2);box-shadow:0 2px 10px rgba(0,0,0,.2);display:none;outline:none;overflow:hidden;position:absolute;right:8px;top:62px;-webkit-animation:gb__a .2s;animation:gb__a .2s;border-radius:2px;-webkit-user-select:text}.gb_x.gb_Na .gb_if,.gb_x.gb_Na .gb_jf,.gb_x.gb_Na .gb_6,.gb_Na.gb_6{display:block}.gb_x.gb_Na.gb_kf .gb_if,.gb_x.gb_Na.gb_kf .gb_jf{display:none}.gb_Td{position:absolute;right:8px;top:62px;z-index:-1}.gb_9a .gb_if,.gb_9a .gb_jf,.gb_9a .gb_6{margin-top:-10px}.gb_x:first-child,#gbsfw:first-child+.gb_x{padding-left:4px}.gb_Ra.gb_Ud .gb_x:first-child{padding-left:0}.gb_Vd{position:relative}.gb_u.gb_Dd.gb_gb.gb_rd{margin:0 12px;padding:0}.gb_u .gb_d{position:relative}.gb_u .gb_x{margin:0 4px;padding:4px}.gb_u .gb_Wd{display:inline-block}.gb_u a.gb_wd{-webkit-box-align:center;-webkit-align-items:center;-webkit-align-items:center;align-items:center;-webkit-border-radius:100px;border-radius:100px;border:0;background:#0b57d0;color:#fff;display:-webkit-inline-box;display:-webkit-inline-flex;display:-webkit-inline-box;display:-webkit-inline-flex;display:inline-flex;font-size:14px;font-weight:500;height:40px;white-space:nowrap;width:auto}.gb_u a.gb_d.gb_wd{margin:0 4px;padding:4px 24px 4px 24px}.gb_u a.gb_wd.gb_Xd{padding:9px 12px 9px 16px}.gb_u a.gb_wd.gb_Zd{background:transparent;border:1px solid #747775;color:#0b57d0;outline:0}.gb_u .gb_t{fill:#0b57d0}.gb_u .gb_0d{fill:#0b57d0;margin-left:8px}.gb_u .gb_0d circle{fill:#fff}.gb_u .gb_wd .gb_Md{-webkit-box-flex:1;-webkit-flex-grow:1;-webkit-box-flex:1;box-flex:1;-webkit-flex-grow:1;flex-grow:1;text-align:center}.gb_u .gb_wd:hover{background:#3763cd}.gb_u .gb_wd:hover .gb_0d{fill:#3763cd}.gb_u .gb_wd:focus,.gb_u .gb_wd:active,.gb_u .gb_wd:focus:hover,.gb_u .gb_wd[aria-expanded=true],.gb_u .gb_wd:hover[aria-expanded=true]{background:#416acf}.gb_u .gb_wd:focus .gb_0d,.gb_u .gb_wd:active .gb_0d,.gb_u .gb_wd:focus:hover .gb_0d,.gb_u .gb_wd[aria-expanded=true] .gb_0d,.gb_u .gb_wd:hover[aria-expanded=true] .gb_0d{fill:#416acf}.gb_u .gb_wd:focus,.gb_u .gb_wd:active,.gb_u .gb_wd[aria-expanded=true]{-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_u .gb_wd:focus-visible{outline:1px solid #416acf;outline-offset:2px}.gb_u .gb_Ia:focus-visible{outline:1px solid #416acf}.gb_u .gb_i.gb_wd{background:#a8c7fa;color:#062e6f}.gb_u .gb_i.gb_wd .gb_0d{fill:#a8c7fa}.gb_u .gb_i.gb_wd .gb_0d circle{fill:#062e6f}.gb_u .gb_i.gb_wd:hover{background:#b4cbf6}.gb_u .gb_i.gb_wd:hover .gb_0d{fill:#b4cbf6}.gb_u .gb_i.gb_wd:focus,.gb_u .gb_i.gb_wd:focus:hover,.gb_u .gb_i.gb_wd:active,.gb_u .gb_i.gb_wd[aria-expanded=true],.gb_u .gb_i.gb_wd:hover[aria-expanded=true]{background:#b8cdf7}.gb_u .gb_i.gb_wd:focus .gb_0d,.gb_u .gb_i.gb_wd:focus:hover .gb_0d,.gb_u .gb_i.gb_wd:active .gb_0d,.gb_u .gb_i.gb_wd[aria-expanded=true] .gb_0d,.gb_u .gb_i.gb_wd:hover[aria-expanded=true] .gb_0d{fill:#b8cdf7}.gb_u .gb_i.gb_wd:focus-visible{outline-color:#b8cdf7}.gb_u .gb_i.gb_wd:focus,.gb_u .gb_i.gb_wd:active,.gb_u .gb_i.gb_wd[aria-expanded=true]{-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_u .gb_wd.gb_Zd:hover,.gb_u .gb_wd.gb_Zd:focus,.gb_u .gb_wd.gb_Zd[aria-expanded=true],.gb_u .gb_wd.gb_Zd:hover[aria-expanded=true]{background:rgba(11,87,208,.08);-webkit-box-shadow:none;box-shadow:none}.gb_u .gb_wd.gb_Zd:active{background:rgba(11,87,208,.12);-webkit-box-shadow:none;box-shadow:none}.gb_u .gb_wd.gb_Zd:focus-visible{border-color:#0b57d0;outline:0}.gb_u .gb_i.gb_wd.gb_Zd{background:transparent;color:#a8c7fa}.gb_u .gb_i.gb_wd.gb_Zd:hover,.gb_u .gb_i.gb_wd.gb_Zd:focus,.gb_u .gb_i.gb_wd.gb_Zd[aria-expanded=true],.gb_u .gb_i.gb_wd.gb_Zd:hover[aria-expanded=true]{background:rgba(168,199,250,.08);-webkit-box-shadow:none;box-shadow:none}.gb_u .gb_i.gb_wd.gb_Zd:active{background:rgba(168,199,250,.12);-webkit-box-shadow:none;box-shadow:none}.gb_u .gb_i.gb_wd.gb_Zd:focus-visible{border-color:#a8c7fa;outline:0}.gb_i .gb_u .gb_t{fill:#a8c7fa}.gb_i .gb_u .gb_Ia:focus-visible{outline-color:#a8c7fa}.gb_7c .gb_Vd,.gb_md .gb_Vd{float:right}.gb_d{padding:8px;cursor:pointer}.gb_d:after{content:"";position:absolute;top:-4px;bottom:-4px;left:-4px;right:-4px}.gb_Ra .gb_ne:not(.gb_za):focus img{background-color:rgba(0,0,0,.2);outline:none;-webkit-border-radius:50%;border-radius:50%}.gb_1d button svg,.gb_d{-webkit-border-radius:50%;border-radius:50%}.gb_1d button:focus:not(:focus-visible) svg,.gb_1d button:hover svg,.gb_1d button:active svg,.gb_d:focus:not(:focus-visible),.gb_d:hover,.gb_d:active,.gb_d[aria-expanded=true]{outline:none}.gb_Qc .gb_1d.gb_we button:focus-visible svg,.gb_1d button:focus-visible svg,.gb_d:focus-visible{outline:1px solid #202124}.gb_Qc .gb_1d button:focus-visible svg,.gb_Qc .gb_d:focus-visible{outline:1px solid #f1f3f4}@media (forced-colors:active){.gb_Qc .gb_1d.gb_we button:focus-visible svg,.gb_1d button:focus-visible svg,.gb_Qc .gb_1d button:focus-visible svg{outline:1px solid currentcolor}}.gb_Qc .gb_1d.gb_we button:focus svg,.gb_Qc .gb_1d.gb_we button:focus:hover svg,.gb_1d button:focus svg,.gb_1d button:focus:hover svg,.gb_d:focus,.gb_d:focus:hover{background-color:rgba(60,64,67,.1)}.gb_Qc .gb_1d.gb_we button:active svg,.gb_1d button:active svg,.gb_d:active{background-color:rgba(60,64,67,.12)}.gb_Qc .gb_1d.gb_we button:hover svg,.gb_1d button:hover svg,.gb_d:hover{background-color:rgba(60,64,67,.08)}.gb_Fa .gb_d.gb_Ia:hover{background-color:transparent}.gb_d[aria-expanded=true],.gb_d:hover[aria-expanded=true]{background-color:rgba(95,99,104,.24)}.gb_d[aria-expanded=true] .gb_h{fill:#5f6368;opacity:1}.gb_Qc .gb_1d button:hover svg,.gb_Qc .gb_d:hover{background-color:rgba(232,234,237,.08)}.gb_Qc .gb_1d button:focus svg,.gb_Qc .gb_1d button:focus:hover svg,.gb_Qc .gb_d:focus,.gb_Qc .gb_d:focus:hover{background-color:rgba(232,234,237,.1)}.gb_Qc .gb_1d button:active svg,.gb_Qc .gb_d:active{background-color:rgba(232,234,237,.12)}.gb_Qc .gb_d[aria-expanded=true],.gb_Qc .gb_d:hover[aria-expanded=true]{background-color:rgba(255,255,255,.12)}.gb_Qc .gb_d[aria-expanded=true] .gb_h{fill:#fff;opacity:1}.gb_x{padding:4px}.gb_Ra.gb_Ud .gb_x{padding:4px 2px}.gb_Ra.gb_Ud .gb_b.gb_x{padding-left:6px}.gb_6{z-index:991;line-height:normal}.gb_6.gb_2d{left:0;right:auto}@media (max-width:350px){.gb_6.gb_2d{left:0}}.gb_3d .gb_6{top:56px}.gb_k .gb_d,.gb_5 .gb_k .gb_d{background-position:-64px -29px}.gb_L .gb_k .gb_d{background-position:-29px -29px;opacity:1}.gb_k .gb_d,.gb_k .gb_d:hover,.gb_k .gb_d:focus{opacity:1}.gb_n{display:none}@media screen and (max-width:319px){.gb_sd:not(.gb_yd) .gb_k{display:none;visibility:hidden}}.gb_q{display:none}.gb_fd{font-family:Google Sans,Roboto,Helvetica,Arial,sans-serif;font-size:20px;font-weight:400;letter-spacing:0.25px;line-height:48px;margin-bottom:2px;opacity:1;overflow:hidden;padding-left:16px;position:relative;text-overflow:ellipsis;vertical-align:middle;top:2px;white-space:nowrap;-webkit-flex:1 1 auto;-webkit-box-flex:1;flex:1 1 auto}.gb_fd.gb_gd{color:#3c4043}.gb_Ra.gb_Sa .gb_fd{margin-bottom:0}.gb_hd.gb_id .gb_fd{padding-left:4px}.gb_Ra.gb_Sa .gb_jd{position:relative;top:-2px}.gb_Ra{color:black;min-width:160px;position:relative;-webkit-transition:box-shadow 250ms;transition:box-shadow 250ms}.gb_Ra.gb_Zc{min-width:120px}.gb_Ra.gb_qd .gb_rd{display:none}.gb_Ra.gb_qd .gb_sd{height:56px}header.gb_Ra{display:block}.gb_Ra svg{fill:currentColor}.gb_td{position:fixed;top:0;width:100%}.gb_ud{-webkit-box-shadow:0 4px 5px 0 rgba(0,0,0,.14),0 1px 10px 0 rgba(0,0,0,.12),0 2px 4px -1px rgba(0,0,0,.2);box-shadow:0 4px 5px 0 rgba(0,0,0,.14),0 1px 10px 0 rgba(0,0,0,.12),0 2px 4px -1px rgba(0,0,0,.2)}.gb_vd{height:64px}.gb_sd{-webkit-box-sizing:border-box;box-sizing:border-box;position:relative;width:100%;display:-webkit-box;display:-webkit-flex;display:flex;-webkit-box-pack:space-between;-webkit-justify-content:space-between;justify-content:space-between;min-width:-webkit-min-content;min-width:min-content}.gb_Ra:not(.gb_Sa) .gb_sd{padding:8px}.gb_Ra.gb_xd .gb_sd{-webkit-flex:1 0 auto;-webkit-box-flex:1;flex:1 0 auto}.gb_Ra .gb_sd.gb_yd.gb_zd{min-width:0}.gb_Ra.gb_Sa .gb_sd{padding:4px;padding-left:8px;min-width:0}.gb_rd{height:48px;vertical-align:middle;white-space:nowrap;-webkit-box-align:center;-webkit-align-items:center;align-items:center;display:-webkit-box;display:-webkit-flex;display:flex;-webkit-user-select:none}.gb_Bd>.gb_rd{display:table-cell;width:100%}.gb_hd{padding-right:30px;box-sizing:border-box;-webkit-flex:1 0 auto;-webkit-box-flex:1;flex:1 0 auto}.gb_Ra.gb_Sa .gb_hd{padding-right:14px}.gb_Cd{-webkit-flex:1 1 100%;-webkit-box-flex:1;flex:1 1 100%}.gb_Cd>:only-child{display:inline-block}.gb_Dd.gb_8c{padding-left:4px}.gb_Dd.gb_Ed,.gb_Ra.gb_xd .gb_Dd,.gb_Ra.gb_Sa:not(.gb_md) .gb_Dd{padding-left:0}.gb_Ra.gb_Sa .gb_Dd.gb_Ed{padding-right:0}.gb_Ra.gb_Sa .gb_Dd.gb_Ed .gb_Fa{margin-left:10px}.gb_8c{display:inline}.gb_Ra.gb_2c .gb_Dd.gb_Fd,.gb_Ra.gb_md .gb_Dd.gb_Fd{padding-left:2px}.gb_fd{display:inline-block}.gb_Dd{-webkit-box-sizing:border-box;box-sizing:border-box;height:48px;line-height:normal;padding:0 4px;padding-left:30px;-webkit-flex:0 0 auto;-webkit-box-flex:0;flex:0 0 auto;-webkit-box-pack:flex-end;-webkit-justify-content:flex-end;justify-content:flex-end}.gb_md{height:48px}.gb_Ra.gb_md{min-width:auto}.gb_md .gb_Dd{float:right;padding-left:32px}.gb_md .gb_Dd.gb_Hd{padding-left:0}.gb_Id{font-size:14px;max-width:200px;overflow:hidden;padding:0 12px;text-overflow:ellipsis;white-space:nowrap;-webkit-user-select:text}.gb_ld{-webkit-transition:background-color .4s;-webkit-transition:background-color .4s;transition:background-color .4s}.gb_Od{color:black}.gb_Qc{color:white}.gb_Ra a,.gb_Vc a{color:inherit}.gb_V{color:rgba(0,0,0,.87)}.gb_Ra svg,.gb_Vc svg,.gb_hd .gb_pd,.gb_7c .gb_pd{color:#5f6368;opacity:1}.gb_Qc svg,.gb_Vc.gb_0c svg,.gb_Qc .gb_hd .gb_pd,.gb_Qc .gb_hd .gb_Pc,.gb_Qc .gb_hd .gb_jd,.gb_Vc.gb_0c .gb_pd{color:rgba(255,255,255,.87)}.gb_Qc .gb_hd .gb_Oc:not(.gb_Pd){opacity:.87}.gb_gd{color:inherit;opacity:1;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased}.gb_Qc .gb_gd,.gb_Od .gb_gd{opacity:1}.gb_Jd{position:relative}.gb_Kd{font-family:arial,sans-serif;line-height:normal;padding-right:15px}a.gb_I,span.gb_I{color:rgba(0,0,0,.87);text-decoration:none}.gb_Qc a.gb_I,.gb_Qc span.gb_I{color:white}a.gb_I:focus{outline-offset:2px}a.gb_I:hover{text-decoration:underline}.gb_J{display:inline-block;padding-left:15px}.gb_J .gb_I{display:inline-block;line-height:24px;vertical-align:middle}.gb_nd{font-family:Google Sans,Roboto,Helvetica,Arial,sans-serif;font-weight:500;font-size:14px;letter-spacing:.25px;line-height:16px;margin-left:10px;margin-right:8px;min-width:96px;padding:9px 23px;text-align:center;vertical-align:middle;border-radius:4px;box-sizing:border-box}.gb_Ra.gb_md .gb_nd{margin-left:8px}#gb a.gb_Da.gb_nd{cursor:pointer}.gb_Da.gb_nd:hover{background:#1b66c9;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_Da.gb_nd:focus,.gb_Da.gb_nd:hover:focus{background:#1c5fba;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_Da.gb_nd:active{background:#1b63c1;-webkit-box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3);box-shadow:0 1px 3px 1px rgba(66,64,67,.15),0 1px 2px 0 rgba(60,64,67,.3)}.gb_nd{background:#1a73e8;border:1px solid transparent}.gb_Ra.gb_Sa .gb_nd{padding:9px 15px;min-width:80px}.gb_Ld{text-align:left}#gb .gb_Qc a.gb_nd:not(.gb_i),#gb.gb_Qc a.gb_nd:not(.gb_Qd){background:#fff;border-color:#dadce0;-webkit-box-shadow:none;box-shadow:none;color:#1a73e8}#gb a.gb_Da.gb_i.gb_nd{background:#8ab4f8;border:1px solid transparent;-webkit-box-shadow:none;box-shadow:none;color:#202124}#gb .gb_Qc a.gb_nd:hover:not(.gb_i),#gb.gb_Qc a.gb_nd:not(.gb_Qd):hover{background:#f8fbff;border-color:#cce0fc}#gb a.gb_Da.gb_i.gb_nd:hover{background:#93baf9;border-color:transparent;-webkit-box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.3);box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.3)}#gb .gb_Qc a.gb_nd:focus:not(.gb_i),#gb .gb_Qc a.gb_nd:focus:hover:not(.gb_i),#gb.gb_Qc a.gb_nd:focus:not(.gb_i),#gb.gb_Qc a.gb_nd:focus:hover:not(.gb_i){background:#f4f8ff;outline:1px solid #c9ddfc}#gb a.gb_Da.gb_i.gb_nd:focus,#gb a.gb_Da.gb_i.gb_nd:focus:hover{background:#a6c6fa;border-color:transparent;-webkit-box-shadow:none;box-shadow:none}#gb .gb_Qc a.gb_nd:active:not(.gb_i),#gb.gb_Qc a.gb_nd:not(.gb_Qd):active{background:#ecf3fe}#gb a.gb_Da.gb_i.gb_nd:active{background:#a1c3f9;-webkit-box-shadow:0 1px 2px rgba(60,64,67,.3),0 2px 6px 2px rgba(60,64,67,.15);box-shadow:0 1px 2px rgba(60,64,67,.3),0 2px 6px 2px rgba(60,64,67,.15)}.gb_l{display:none}@media screen and (max-width:319px){.gb_sd:not(.gb_yd) .gb_k{display:none;visibility:hidden}}.gb_Fa{background-color:rgba(255,255,255,.88);border:1px solid #dadce0;-webkit-box-sizing:border-box;box-sizing:border-box;cursor:pointer;display:inline-block;max-height:48px;overflow:hidden;outline:none;padding:0;vertical-align:middle;width:134px;-webkit-border-radius:8px;border-radius:8px}.gb_Fa.gb_i{background-color:transparent;border:1px solid #5f6368}.gb_Ma{display:inherit}.gb_Fa.gb_i .gb_Ma{background:#fff;-webkit-border-radius:4px;border-radius:4px;display:inline-block;left:8px;margin-right:5px;position:relative;padding:3px;top:-1px}.gb_Fa:hover{border:1px solid #d2e3fc;background-color:rgba(248,250,255,.88)}.gb_Fa.gb_i:hover{background-color:rgba(241,243,244,.04);border:1px solid #5f6368}.gb_Fa:focus-visible,.gb_Fa:focus{background-color:#fff;outline:1px solid #202124;-webkit-box-shadow:0 1px 2px 0 rgba(60,64,67,.3),0 1px 3px 1px rgba(60,64,67,.15);box-shadow:0 1px 2px 0 rgba(60,64,67,.3),0 1px 3px 1px rgba(60,64,67,.15)}.gb_Fa.gb_i:focus-visible,.gb_Fa.gb_i:focus{background-color:rgba(241,243,244,.12);outline:1px solid #f1f3f4;-webkit-box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px 0 rgba(0,0,0,.3);box-shadow:0 1px 3px 1px rgba(0,0,0,.15),0 1px 2px 0 rgba(0,0,0,.3)}.gb_Fa.gb_i:active,.gb_Fa.gb_Na.gb_i:focus{background-color:rgba(241,243,244,.1);border:1px solid #5f6368}.gb_Oa{display:inline-block;padding-bottom:2px;padding-left:7px;padding-top:2px;text-align:center;vertical-align:middle;line-height:32px;width:78px}.gb_Fa.gb_i .gb_Oa{line-height:26px;margin-left:0;padding-bottom:0;padding-left:0;padding-top:0;width:72px}.gb_Oa.gb_Pa{background-color:#f1f3f4;-webkit-border-radius:4px;border-radius:4px;margin-left:8px;padding-left:0;line-height:30px}.gb_Oa.gb_Pa .gb_Qa{vertical-align:middle}.gb_Ra:not(.gb_Sa) .gb_Fa{margin-left:10px;margin-right:4px}.gb_Ta{max-height:32px;width:78px}.gb_Fa.gb_i .gb_Ta{max-height:26px;width:72px}.gb_p{-webkit-background-size:32px 32px;background-size:32px 32px;border:0;-webkit-border-radius:50%;border-radius:50%;display:block;margin:0px;position:relative;height:32px;width:32px;z-index:0}.gb_4a{background-color:#e8f0fe;border:1px solid rgba(32,33,36,.08);position:relative}.gb_4a.gb_p{height:30px;width:30px}.gb_4a.gb_p:hover,.gb_4a.gb_p:active{-webkit-box-shadow:none;box-shadow:none}.gb_5a{background:#fff;border:none;-webkit-border-radius:50%;border-radius:50%;bottom:2px;-webkit-box-shadow:0px 1px 2px 0px rgba(60,64,67,.30),0px 1px 3px 1px rgba(60,64,67,.15);box-shadow:0px 1px 2px 0px rgba(60,64,67,.30),0px 1px 3px 1px rgba(60,64,67,.15);height:14px;margin:2px;position:absolute;right:0;width:14px}.gb_6a{color:#1f71e7;font:400 22px/32px Google Sans,Roboto,Helvetica,Arial,sans-serif;text-align:center;text-transform:uppercase}@media (-webkit-min-device-pixel-ratio:1.25),(min-resolution:1.25dppx),(min-device-pixel-ratio:1.25){.gb_p::before,.gb_7a::before{display:inline-block;-webkit-transform:scale(0.5);-webkit-transform:scale(0.5);transform:scale(0.5);-webkit-transform-origin:left 0;-webkit-transform-origin:left 0;transform-origin:left 0}.gb_N .gb_7a::before{-webkit-transform:scale(scale(0.416666667));-webkit-transform:scale(scale(0.416666667));transform:scale(scale(0.416666667))}}.gb_p:hover,.gb_p:focus{-webkit-box-shadow:0 1px 0 rgba(0,0,0,.15);box-shadow:0 1px 0 rgba(0,0,0,.15)}.gb_p:active{-webkit-box-shadow:inset 0 2px 0 rgba(0,0,0,.15);box-shadow:inset 0 2px 0 rgba(0,0,0,.15)}.gb_p:active::after{background:rgba(0,0,0,.1);-webkit-border-radius:50%;border-radius:50%;content:"";display:block;height:100%}.gb_8a{cursor:pointer;line-height:40px;min-width:30px;opacity:.75;overflow:hidden;vertical-align:middle;text-overflow:ellipsis}.gb_d.gb_8a{width:auto}.gb_8a:hover,.gb_8a:focus{opacity:.85}.gb_9a .gb_8a,.gb_9a .gb_ab{line-height:26px}#gb#gb.gb_9a a.gb_8a,.gb_9a .gb_ab{font-size:11px;height:auto}.gb_bb{border-top:4px solid #000;border-left:4px dashed transparent;border-right:4px dashed transparent;display:inline-block;margin-left:6px;opacity:.75;vertical-align:middle}.gb_Ia:hover .gb_bb{opacity:.85}.gb_Fa>.gb_b{padding:3px 3px 3px 4px}.gb_cb.gb_3a{color:#fff}.gb_L .gb_8a,.gb_L .gb_bb{opacity:1}#gb#gb.gb_L.gb_L a.gb_8a,#gb#gb .gb_L.gb_L a.gb_8a{color:#fff}.gb_L.gb_L .gb_bb{border-top-color:#fff;opacity:1}.gb_5 .gb_p:hover,.gb_L .gb_p:hover,.gb_5 .gb_p:focus,.gb_L .gb_p:focus{-webkit-box-shadow:0 1px 0 rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.2);box-shadow:0 1px 0 rgba(0,0,0,.15),0 1px 2px rgba(0,0,0,.2)}.gb_db .gb_b,.gb_eb .gb_b{position:absolute;right:1px}.gb_b.gb_K,.gb_fb.gb_K,.gb_Ia.gb_K{-webkit-flex:0 1 auto;-webkit-box-flex:0;flex:0 1 auto}.gb_gb.gb_hb .gb_8a{width:30px!important}.gb_o{height:40px;position:absolute;right:-5px;top:-5px;width:40px}.gb_ib .gb_o,.gb_jb .gb_o{right:0;top:0}.gb_b .gb_d{padding:4px}.gb_r{display:none}sentinel{}</style><script nonce="">;this.gbar_={CONFIG:[[[0,"www.gstatic.com","og.qtm.en_US.GJkyMsvcljY.2019.O","com","en","425",0,[4,2,"","","","639614954","0"],null,"NphkZp2VCIefp84Pgf60sQI",null,0,"og.qtm.qmT6DQgbzEQ.L.W.O","AA2YrTtmD1oWXfR6WhUiAKksxBHsMK4_SQ","AA2YrTuUoxtuyUDvYGtQ10hK7I_33XgLMg","",2,1,200,"IRN",null,null,"425","425",1,null,null,114591953,1],null,[1,0.1000000014901161,2,1],null,[1,0,0,null,"0","maryaamjabbari@gmail.com","","AJ5SeQKfCEwCjrYVgar9WQC2VEwyRqzi_EeqJV4k-NqUcDNTNK7fw2i1AI_T-9BHRfcK6qJ31UEEkEbcyZbrMGRr4qQdD6m23g",0,0,0],[0,0,"",1,0,0,0,0,0,0,null,0,0,null,0,0,null,null,0,0,0,"","","","","","",null,0,0,0,0,0,null,null,null,"rgba(32,33,36,1)","rgba(255,255,255,1)",0,0,0,null,null,1,0,0],["%1$s (default)","Brand account",1,"%1$s (delegated)",1,null,83,"https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId?authuser=$authuser",null,null,null,1,"https://accounts.google.com/ListAccounts?listPages=0\u0026pid=425\u0026gpsia=1\u0026source=ogb\u0026atic=1\u0026mo=1\u0026mn=1\u0026hl=en\u0026ts=250",0,"dashboard",null,null,null,null,"Profile","",1,null,"Signed out","https://accounts.google.com/AccountChooser?source=ogb\u0026continue=$continue\u0026Email=$email\u0026ec=GAhAqQM","https://accounts.google.com/RemoveLocalAccount?source=ogb","Remove","Sign in",0,1,1,0,1,1,0,null,null,null,"Session expired",null,null,null,"Visitor",null,"Default","Delegated","Sign out of all accounts",0,null,null,0,null,null,"myaccount.google.com","https",0,1,0],null,["1","gci_91f30755d6a6b787dcc2a4062e6e9824.js","googleapis.client:gapi.iframes","0","en"],null,null,null,null,["m;/_/scs/abc-static/_/js/k=gapi.gapi.en.JHoMBbBABZg.O/am=AAAQ/d=1/rs=AHpOoo_6Zf8M75AJqSyaaLg_vD7Vr9kevQ/m=__features__","https://apis.google.com","","","1","",null,1,"es_plusone_gc_20240506.0_p0","en",null,0],[0.009999999776482582,"com","425",[null,"","0",null,1,5184000,null,null,"",null,null,null,null,null,0,null,0,null,1,0,0,0,null,null,0,0,null,0,0,0,0,0],null,null,null,0,null,null,["5061451","google\\.(com|ru|ca|by|kz|com\\.mx|com\\.tr)$",1]],[1,1,null,40400,425,"IRN","en","639614954.0",8,1,1,0,null,null,null,null,"3700949,3701310,3701353,3701387",null,null,null,"NphkZp2VCIefp84Pgf60sQI",0,0,0,null,2,5,"nn",51,0,0,1,1,1,114591953,0],[[null,null,null,"https://www.gstatic.com/og/_/js/k=og.qtm.en_US.GJkyMsvcljY.2019.O/rt=j/m=qabr,qgl,q_dnp,qcwid,qbd,qapid,qrcd,q_dg/exm=qaaw,qadd,qaid,qein,qhaw,qhba,qhbr,qhch,qhga,qhid,qhin/d=1/ed=1/rs=AA2YrTtmD1oWXfR6WhUiAKksxBHsMK4_SQ"],[null,null,null,"https://www.gstatic.com/og/_/ss/k=og.qtm.qmT6DQgbzEQ.L.W.O/m=qcwid/excm=qaaw,qadd,qaid,qein,qhaw,qhba,qhbr,qhch,qhga,qhid,qhin/d=1/ed=1/ct=zgms/rs=AA2YrTuUoxtuyUDvYGtQ10hK7I_33XgLMg"]],null,null,null,[[[null,null,[null,null,null,"https://ogs.google.com/u/0/widget/account?amb=1\u0026sea=1"],0,414,436,57,4,1,0,0,65,66,8000,"https://accounts.google.com/SignOutOptions?hl=en\u0026continue=https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId\u0026ec=GBRAqQM",68,2,null,null,1,113,"Something went wrong.%1$s Refresh to try again or %2$schoose another account%3$s.",3,null,null,75,0,null,null,null,null,null,null,null,"/widget/account",["https","myaccount.google.com",0,32,83,0],0,0,1,["Critical security alert","Important account alert","Storage usage alert"],0,1,null,1,1,0,0,null,null,0,0,0,0,0,0]],null,null,"425","425",1,0,null,"en",0,["https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId?authuser=$authuser","https://accounts.google.com/AddSession?hl=en\u0026continue=https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId\u0026ec=GAlAqQM","https://accounts.google.com/Logout?hl=en\u0026continue=https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId\u0026timeStmp=1717868598\u0026secTok=.AG5fkS_rhqHR1uwYeZi9ygyDL4qel2UetA\u0026ec=GAdAqQM","https://accounts.google.com/ListAccounts?listPages=0\u0026pid=425\u0026gpsia=1\u0026source=ogb\u0026atic=1\u0026mo=1\u0026mn=1\u0026hl=en\u0026ts=250",0,0,"",0,0,null,0,0,"https://accounts.google.com/ServiceLogin?passive=true\u0026continue=https%3A%2F%2Fcolab.research.google.com%2Fdrive%2F1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId\u0026ec=GAZAqQM",0,0],0,0,0,null,0,null,0,1],null,[["mousedown","touchstart","touchmove","wheel","keydown"],300000],[[null,null,null,"https://accounts.google.com/RotateCookiesPage"],3,null,null,null,0,0]]],};this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
_._F_toggles_initialize=function(a){("undefined"!==typeof globalThis?globalThis:"undefined"!==typeof self?self:this)._F_toggles=a||[]};(0,_._F_toggles_initialize)([]);
/*

 Copyright The Closure Library Authors.
 SPDX-License-Identifier: Apache-2.0
*/
var ha,ia,ma,oa,pa,ya,za,Aa,Ca,Da,Ea,Ha,Xa,Wa,$a,bb,ab,cb,db,gb,mb,ob,pb,qb,rb;_.aa=function(a,b){if(Error.captureStackTrace)Error.captureStackTrace(this,_.aa);else{const c=Error().stack;c&&(this.stack=c)}a&&(this.message=String(a));void 0!==b&&(this.cause=b)};_.ca=function(a){_.r.setTimeout(()=>{throw a;},0)};_.da=function(){var a=_.r.navigator;return a&&(a=a.userAgent)?a:""};ha=function(a){return ea?fa?fa.brands.some(({brand:b})=>b&&-1!=b.indexOf(a)):!1:!1};_.u=function(a){return-1!=_.da().indexOf(a)};
ia=function(){return ea?!!fa&&0<fa.brands.length:!1};_.ja=function(){return ia()?!1:_.u("Opera")};_.ka=function(){return ia()?!1:_.u("Trident")||_.u("MSIE")};_.la=function(){return _.u("Firefox")||_.u("FxiOS")};_.na=function(){return _.u("Safari")&&!(ma()||(ia()?0:_.u("Coast"))||_.ja()||(ia()?0:_.u("Edge"))||(ia()?ha("Microsoft Edge"):_.u("Edg/"))||(ia()?ha("Opera"):_.u("OPR"))||_.la()||_.u("Silk")||_.u("Android"))};
ma=function(){return ia()?ha("Chromium"):(_.u("Chrome")||_.u("CriOS"))&&!(ia()?0:_.u("Edge"))||_.u("Silk")};oa=function(){return ea?!!fa&&!!fa.platform:!1};pa=function(){return _.u("iPhone")&&!_.u("iPod")&&!_.u("iPad")};_.qa=function(){return pa()||_.u("iPad")||_.u("iPod")};_.ra=function(){return oa()?"macOS"===fa.platform:_.u("Macintosh")};_.ta=function(a,b){return 0<=_.sa(a,b)};
_.ua=function(a){let b="",c=0;const d=a.length-10240;for(;c<d;)b+=String.fromCharCode.apply(null,a.subarray(c,c+=10240));b+=String.fromCharCode.apply(null,c?a.subarray(c):a);return btoa(b)};_.va=function(a){return null!=a&&a instanceof Uint8Array};_.wa=function(a){return Array.prototype.slice.call(a)};ya=function(a,b){_.xa(b,(a|0)&-14591)};za=function(a,b){_.xa(b,(a|34)&-14557)};Aa=function(a){a=a>>14&1023;return 0===a?536870912:a};Ca=function(a){return!(!a||"object"!==typeof a||a.i!==Ba)};
Da=function(a){return null!==a&&"object"===typeof a&&!Array.isArray(a)&&a.constructor===Object};Ea=function(a,b,c){if(!Array.isArray(a)||a.length)return!1;const d=a[_.v]|0;if(d&1)return!0;if(!(b&&(Array.isArray(b)?b.includes(c):b.has(c))))return!1;_.xa(a,d|1);return!0};_.Fa=function(a){if(a&2)throw Error();};Ha=function(a,b){(b=_.Ga?b[_.Ga]:void 0)&&(a[_.Ga]=_.wa(b))};_.Ja=function(){const a=Error();Ia(a,"incident");_.ca(a)};_.Ka=function(a){a=Error(a);Ia(a,"warning");return a};
_.Ma=function(a){if("boolean"!==typeof a)throw Error("r`"+_.La(a)+"`"+a);return a};_.Na=function(a){if(!Number.isFinite(a))throw _.Ka("enum");return a|0};_.Oa=function(a){if("number"!==typeof a)throw _.Ka("int32");if(!Number.isFinite(a))throw _.Ka("int32");return a|0};_.Pa=function(a){if(null!=a&&"string"!==typeof a)throw Error();return a};_.Qa=function(a){return null==a||"string"===typeof a?a:void 0};
_.Sa=function(a,b,c){if(null!=a&&"object"===typeof a&&a.Hd===_.Ra)return a;if(Array.isArray(a)){var d=a[_.v]|0,e=d;0===e&&(e|=c&32);e|=c&2;e!==d&&_.xa(a,e);return new b(a)}};_.Ua=function(a,b){Ta=b;a=new a(b);Ta=void 0;return a};
_.Va=function(a,b,c){null==a&&(a=Ta);Ta=void 0;if(null==a){var d=96;c?(a=[c],d|=512):a=[];b&&(d=d&-16760833|(b&1023)<<14)}else{if(!Array.isArray(a))throw Error("s");d=a[_.v]|0;if(d&2048)throw Error("t");if(d&64)return a;d|=64;if(c&&(d|=512,c!==a[0]))throw Error("u");a:{c=a;const e=c.length;if(e){const f=e-1;if(Da(c[f])){d|=256;b=f-(+!!(d&512)-1);if(1024<=b)throw Error("v");d=d&-16760833|(b&1023)<<14;break a}}if(b){b=Math.max(b,e-(+!!(d&512)-1));if(1024<b)throw Error("w");d=d&-16760833|(b&1023)<<14}}}_.xa(a,
d);return a};Xa=function(a,b){return Wa(b)};Wa=function(a){switch(typeof a){case "number":return isFinite(a)?a:String(a);case "boolean":return a?1:0;case "object":if(a)if(Array.isArray(a)){if(Ea(a,void 0,0))return}else{if(_.va(a))return _.ua(a);if("function"==typeof _.Ya&&a instanceof _.Ya)return a.j()}}return a};$a=function(a,b,c){const d=_.wa(a);var e=d.length;const f=b&256?d[e-1]:void 0;e+=f?-1:0;for(b=b&512?1:0;b<e;b++)d[b]=c(d[b]);if(f){b=d[b]={};for(const g in f)b[g]=c(f[g])}Ha(d,a);return d};
bb=function(a,b,c,d,e){if(null!=a){if(Array.isArray(a))a=Ea(a,void 0,0)?void 0:e&&(a[_.v]|0)&2?a:ab(a,b,c,void 0!==d,e);else if(Da(a)){const f={};for(let g in a)f[g]=bb(a[g],b,c,d,e);a=f}else a=b(a,d);return a}};ab=function(a,b,c,d,e){const f=d||c?a[_.v]|0:0;d=d?!!(f&32):void 0;const g=_.wa(a);for(let h=0;h<g.length;h++)g[h]=bb(g[h],b,c,d,e);c&&(Ha(g,a),c(f,g));return g};cb=function(a){return a.Hd===_.Ra?a.toJSON():Wa(a)};
db=function(a,b,c=za){if(null!=a){if(a instanceof Uint8Array)return b?a:new Uint8Array(a);if(Array.isArray(a)){var d=a[_.v]|0;d&2||(b&&(b=0===d||!!(d&32)&&!(d&64||!(d&16))),a=b?_.xa(a,(d|34)&-12293):ab(a,db,d&4?za:c,!0,!0));return a}a.Hd===_.Ra&&(c=a.ka,d=c[_.v],a=d&2?a:_.Ua(a.constructor,_.eb(c,d,!0)));return a}};_.eb=function(a,b,c){const d=c||b&2?za:ya,e=!!(b&32);a=$a(a,b,f=>db(f,e,d));a[_.v]=a[_.v]|32|(c?2:0);return a};
_.fb=function(a){const b=a.ka,c=b[_.v];return c&2?_.Ua(a.constructor,_.eb(b,c,!1)):a};gb=function(a,b,c,d){b=d+(+!!(b&512)-1);if(!(0>b||b>=a.length||b>=c))return a[b]};_.hb=function(a,b,c,d,e){const f=Aa(b);if(c>=f||e){let g=b;if(b&256)e=a[a.length-1];else{if(null==d)return g;e=a[f+(+!!(b&512)-1)]={};g|=256}e[c]=d;c<f&&(a[c+(+!!(b&512)-1)]=void 0);g!==b&&_.xa(a,g);return g}a[c+(+!!(b&512)-1)]=d;b&256&&(a=a[a.length-1],c in a&&delete a[c]);return b};
_.jb=function(a,b,c,d){a=a.ka;let e=a[_.v];const f=_.ib(a,e,c,d);b=_.Sa(f,b,e);b!==f&&null!=b&&_.hb(a,e,c,b,d);return b};_.kb=function(a,b){return null!=a?a:b};
mb=function(a,b,c){var d=lb?void 0:a.constructor.ta;const e=(c?a.ka:b)[_.v];a=b.length;if(!a)return b;let f,g;if(Da(c=b[a-1])){a:{var h=c;let n={},p=!1;for(var k in h){let t=h[k];if(Array.isArray(t)){let q=t;if(Ea(t,d,+k)||Ca(t)&&0===t.size)t=null;t!=q&&(p=!0)}null!=t?n[k]=t:p=!0}if(p){for(var l in n){h=n;break a}h=null}}h!=c&&(f=!0);a--}for(k=+!!(e&512)-1;0<a;a--){l=a-1;c=b[l];l-=k;if(!(null==c||Ea(c,d,l)||Ca(c)&&0===c.size))break;g=!0}if(!f&&!g)return b;b=Array.prototype.slice.call(b,0,a);h&&b.push(h);
return b};_.w=function(a,b){return null!=a?!!a:!!b};_.x=function(a,b){void 0==b&&(b="");return null!=a?a:b};_.nb=function(a){for(const b in a)return!1;return!0};ob="function"==typeof Object.defineProperties?Object.defineProperty:function(a,b,c){if(a==Array.prototype||a==Object.prototype)return a;a[b]=c.value;return a};
pb=function(a){a=["object"==typeof globalThis&&globalThis,a,"object"==typeof window&&window,"object"==typeof self&&self,"object"==typeof global&&global];for(var b=0;b<a.length;++b){var c=a[b];if(c&&c.Math==Math)return c}throw Error("a");};qb=pb(this);rb=function(a,b){if(b)a:{var c=qb;a=a.split(".");for(var d=0;d<a.length-1;d++){var e=a[d];if(!(e in c))break a;c=c[e]}a=a[a.length-1];d=c[a];b=b(d);b!=d&&null!=b&&ob(c,a,{configurable:!0,writable:!0,value:b})}};rb("globalThis",function(a){return a||qb});
rb("Promise.prototype.finally",function(a){return a?a:function(b){return this.then(function(c){return Promise.resolve(b()).then(function(){return c})},function(c){return Promise.resolve(b()).then(function(){throw c;})})}});var vb,wb,yb,zb;_.sb=_.sb||{};_.r=this||self;vb=function(a){var b=_.tb("WIZ_global_data.oxN3nb");a=b&&b[a];return null!=a?a:!1};wb=_.r._F_toggles||[];_.tb=function(a,b){a=a.split(".");b=b||_.r;for(var c=0;c<a.length;c++)if(b=b[a[c]],null==b)return null;return b};_.La=function(a){var b=typeof a;return"object"!=b?b:a?Array.isArray(a)?"array":b:"null"};_.xb="closure_uid_"+(1E9*Math.random()>>>0);yb=function(a,b,c){return a.call.apply(a.bind,arguments)};
zb=function(a,b,c){if(!a)throw Error();if(2<arguments.length){var d=Array.prototype.slice.call(arguments,2);return function(){var e=Array.prototype.slice.call(arguments);Array.prototype.unshift.apply(e,d);return a.apply(b,e)}}return function(){return a.apply(b,arguments)}};_.y=function(a,b,c){_.y=Function.prototype.bind&&-1!=Function.prototype.bind.toString().indexOf("native code")?yb:zb;return _.y.apply(null,arguments)};
_.z=function(a,b){a=a.split(".");var c=_.r;a[0]in c||"undefined"==typeof c.execScript||c.execScript("var "+a[0]);for(var d;a.length&&(d=a.shift());)a.length||void 0===b?c[d]&&c[d]!==Object.prototype[d]?c=c[d]:c=c[d]={}:c[d]=b};_.A=function(a,b){function c(){}c.prototype=b.prototype;a.X=b.prototype;a.prototype=new c;a.prototype.constructor=a;a.ej=function(d,e,f){for(var g=Array(arguments.length-2),h=2;h<arguments.length;h++)g[h-2]=arguments[h];return b.prototype[e].apply(d,g)}};_.A(_.aa,Error);_.aa.prototype.name="CustomError";_.Ab=String.prototype.trim?function(a){return a.trim()}:function(a){return/^[\s\xa0]*([\s\S]*?)[\s\xa0]*$/.exec(a)[1]};var Bb=!!(wb[0]&512),Cb=!!(wb[0]&1024),Db=!!(wb[0]&8);var ea=Bb?Cb:vb(610401301),lb=Bb?Db:vb(188588736);var fa,Eb=_.r.navigator;fa=Eb?Eb.userAgentData||null:null;_.sa=function(a,b){return Array.prototype.indexOf.call(a,b,void 0)};_.Fb=function(a,b,c){Array.prototype.forEach.call(a,b,c)};_.Gb=function(a){_.Gb[" "](a);return a};_.Gb[" "]=function(){};var Tb;_.Hb=_.ja();_.Ib=_.ka();_.Jb=_.u("Edge");_.Kb=_.u("Gecko")&&!(-1!=_.da().toLowerCase().indexOf("webkit")&&!_.u("Edge"))&&!(_.u("Trident")||_.u("MSIE"))&&!_.u("Edge");_.Lb=-1!=_.da().toLowerCase().indexOf("webkit")&&!_.u("Edge");_.Mb=_.ra();_.Nb=oa()?"Windows"===fa.platform:_.u("Windows");_.Ob=oa()?"Android"===fa.platform:_.u("Android");_.Pb=pa();_.Qb=_.u("iPad");_.Rb=_.u("iPod");_.Sb=_.qa();
a:{var Ub="",Vb=function(){var a=_.da();if(_.Kb)return/rv:([^\);]+)(\)|;)/.exec(a);if(_.Jb)return/Edge\/([\d\.]+)/.exec(a);if(_.Ib)return/\b(?:MSIE|rv)[: ]([^\);]+)(\)|;)/.exec(a);if(_.Lb)return/WebKit\/(\S+)/.exec(a);if(_.Hb)return/(?:Version)[ \/]?(\S+)/.exec(a)}();Vb&&(Ub=Vb?Vb[1]:"");if(_.Ib){var Wb,Xb=_.r.document;Wb=Xb?Xb.documentMode:void 0;if(null!=Wb&&Wb>parseFloat(Ub)){Tb=String(Wb);break a}}Tb=Ub}_.Yb=Tb;_.Zb=_.la();_.$b=pa()||_.u("iPod");_.ac=_.u("iPad");_.bc=_.u("Android")&&!(ma()||_.la()||_.ja()||_.u("Silk"));_.cc=ma();_.dc=_.na()&&!_.qa();_.ec="undefined"!==typeof TextDecoder;_.fc="undefined"!==typeof TextEncoder;var gc;_.v=Symbol();gc=Symbol();_.hc=Symbol();_.xa=(a,b)=>{a[_.v]=b;return a};var Ba,ic,kc,lc,mc;_.Ra={};Ba={};kc=[];_.xa(kc,55);_.jc=Object.freeze(kc);lc=class{};mc=class{};Object.freeze(new lc);Object.freeze(new mc);_.nc=Object.freeze(new mc);var Ia=function(a,b){a.__closure__error__context__984382||(a.__closure__error__context__984382={});a.__closure__error__context__984382.severity=b};var oc;var Ta;_.pc=function(a,b){a=a.ka;return _.ib(a,a[_.v],b)};_.ib=function(a,b,c,d){if(-1===c)return null;const e=Aa(b);if(c>=e){if(b&256)return a[a.length-1][c]}else{var f=a.length;if(d&&b&256&&(d=a[f-1][c],null!=d)){if(gb(a,b,e,c)&&null!=gc){var g;a=null!=(g=oc)?g:oc={};g=a[gc]||0;4<=g||(a[gc]=g+1,_.Ja())}return d}return gb(a,b,e,c)}};_.qc=function(a,b,c){const d=a.ka;let e=d[_.v];_.Fa(e);_.hb(d,e,b,c);return a};
_.C=function(a,b,c,d=!1){b=_.jb(a,b,c,d);if(null==b)return b;a=a.ka;let e=a[_.v];if(!(e&2)){const f=_.fb(b);f!==b&&(b=f,_.hb(a,e,c,b,d))}return b};_.E=function(a,b,c){null==c&&(c=void 0);return _.qc(a,b,c)};_.F=function(a,b){a=_.pc(a,b);return null==a||"boolean"===typeof a?a:"number"===typeof a?!!a:void 0};_.G=function(a,b){return _.Qa(_.pc(a,b))};_.I=function(a,b,c=!1){return _.kb(_.F(a,b),c)};_.J=function(a,b){return _.kb(_.G(a,b),"")};_.K=function(a,b,c){return _.qc(a,b,null==c?c:_.Ma(c))};
_.L=function(a,b,c){return _.qc(a,b,null==c?c:_.Oa(c))};_.M=function(a,b,c){return _.qc(a,b,_.Pa(c))};_.N=function(a,b,c){return _.qc(a,b,null==c?c:_.Na(c))};_.O=class{constructor(a,b,c){this.ka=_.Va(a,b,c)}toJSON(){return ic?mb(this,this.ka,!1):mb(this,ab(this.ka,cb,void 0,void 0,!1),!0)}Ga(){ic=!0;try{return JSON.stringify(this.toJSON(),Xa)}finally{ic=!1}}vc(){return!!((this.ka[_.v]|0)&2)}};_.O.prototype.Hd=_.Ra;_.O.prototype.toString=function(){return mb(this,this.ka,!1).toString()};_.rc=Symbol();_.sc=Symbol();_.tc=Symbol();_.uc=Symbol();_.vc=Symbol();var wc=class extends _.O{constructor(){super()}};_.xc=class extends _.O{constructor(){super()}D(a){return _.L(this,3,a)}};var yc=class extends _.O{constructor(a){super(a)}Mc(a){return _.M(this,24,a)}};_.zc=class extends _.O{constructor(a){super(a)}};_.P=function(){this.Ea=this.Ea;this.ha=this.ha};_.P.prototype.Ea=!1;_.P.prototype.isDisposed=function(){return this.Ea};_.P.prototype.fa=function(){this.Ea||(this.Ea=!0,this.O())};_.P.prototype.O=function(){if(this.ha)for(;this.ha.length;)this.ha.shift()()};var Ac=class extends _.P{constructor(){var a=window;super();this.o=a;this.i=[];this.j={}}resolve(a){var b=this.o;a=a.split(".");for(var c=a.length,d=0;d<c;++d)if(b[a[d]])b=b[a[d]];else return null;return b instanceof Function?b:null}Eb(){for(var a=this.i.length,b=this.i,c=[],d=0;d<a;++d){var e=b[d].i(),f=this.resolve(e);if(f&&f!=this.j[e])try{b[d].Eb(f)}catch(g){}else c.push(b[d])}this.i=c.concat(b.slice(a))}};var Cc=class extends _.P{constructor(){var a=_.Bc;super();this.o=a;this.A=this.i=null;this.v=0;this.B={};this.j=!1;a=window.navigator.userAgent;0<=a.indexOf("MSIE")&&0<=a.indexOf("Trident")&&(a=/\b(?:MSIE|rv)[: ]([^\);]+)(\)|;)/.exec(a))&&a[1]&&9>parseFloat(a[1])&&(this.j=!0)}C(a,b){this.i=b;this.A=a;b.preventDefault?b.preventDefault():b.returnValue=!1}};_.Dc=class extends _.O{constructor(a){super(a)}};var Ec=class extends _.O{constructor(a){super(a)}};var Hc;_.Fc=function(a,b,c=98){if(a.i){const d=new wc;_.M(d,1,b.message);_.M(d,2,b.stack);_.L(d,3,b.lineNumber);_.N(d,5,1);b=new _.xc;_.E(b,40,d);a.i.log(c,b)}};Hc=class{constructor(){var a=Gc;this.i=null;_.I(a,4,!0)}log(a){_.Fc(this,a)}};var Ic,Jc;Ic=function(a){if(0<a.o.length){var b=void 0!==a.i,c=void 0!==a.j;if(b||c){b=b?a.v:a.A;c=a.o;a.o=[];try{_.Fb(c,b,a)}catch(d){console.error(d)}}}};_.Kc=class{constructor(a){this.i=a;this.j=void 0;this.o=[]}then(a,b,c){this.o.push(new Jc(a,b,c));Ic(this)}resolve(a){if(void 0!==this.i||void 0!==this.j)throw Error("B");this.i=a;Ic(this)}reject(a){if(void 0!==this.i||void 0!==this.j)throw Error("B");this.j=a;Ic(this)}v(a){a.j&&a.j.call(a.i,this.i)}A(a){a.o&&a.o.call(a.i,this.j)}};
Jc=class{constructor(a,b,c){this.j=a;this.o=b;this.i=c}};_.Lc=a=>{var b="tc";if(a.tc&&a.hasOwnProperty(b))return a.tc;b=new a;return a.tc=b};_.Q=class{constructor(){this.v=new _.Kc;this.i=new _.Kc;this.D=new _.Kc;this.B=new _.Kc;this.C=new _.Kc;this.A=new _.Kc;this.o=new _.Kc;this.j=new _.Kc;this.F=new _.Kc}K(){return this.v}M(){return this.i}N(){return this.D}L(){return this.B}Ea(){return this.C}ha(){return this.A}J(){return this.o}G(){return this.j}static i(){return _.Lc(_.Q)}};var Qc;_.Nc=function(){return _.C(_.Mc,yc,1)};_.Oc=function(){return _.C(_.Mc,_.zc,5)};Qc=class extends _.O{constructor(){super(Pc)}};var Pc;window.gbar_&&window.gbar_.CONFIG?Pc=window.gbar_.CONFIG[0]||{}:Pc=[];_.Mc=new Qc;var Gc=_.C(_.Mc,Ec,3)||new Ec;_.Nc()||new yc;_.Bc=new Hc;_.z("gbar_._DumpException",function(a){_.Bc?_.Bc.log(a):console.error(a)});_.Rc=new Cc;var Tc;_.Uc=function(a,b){var c=_.Sc.i();if(a in c.i){if(c.i[a]!=b)throw new Tc;}else{c.i[a]=b;const h=c.j[a];if(h)for(let k=0,l=h.length;k<l;k++){b=h[k];var d=c.i;delete b.i[a];if(_.nb(b.i)){for(var e=b.j.length,f=Array(e),g=0;g<e;g++)f[g]=d[b.j[g]];b.o.apply(b.v,f)}}delete c.j[a]}};_.Sc=class{constructor(){this.i={};this.j={}}static i(){return _.Lc(_.Sc)}};_.Vc=class extends _.aa{constructor(){super()}};Tc=class extends _.Vc{};_.z("gbar.A",_.Kc);_.Kc.prototype.aa=_.Kc.prototype.then;_.z("gbar.B",_.Q);_.Q.prototype.ba=_.Q.prototype.M;_.Q.prototype.bb=_.Q.prototype.N;_.Q.prototype.bd=_.Q.prototype.Ea;_.Q.prototype.bf=_.Q.prototype.K;_.Q.prototype.bg=_.Q.prototype.L;_.Q.prototype.bh=_.Q.prototype.ha;_.Q.prototype.bj=_.Q.prototype.J;_.Q.prototype.bk=_.Q.prototype.G;_.z("gbar.a",_.Q.i());window.gbar&&window.gbar.ap&&window.gbar.ap(window.gbar.a);var Wc=new Ac;_.Uc("api",Wc);var Xc=_.Oc()||new _.zc,Yc=window,Zc=_.x(_.G(Xc,8));
Yc.__PVT=Zc;_.Uc("eq",_.Rc);
}catch(e){_._DumpException(e)}
try{
_.$c=class extends _.O{constructor(a){super(a)}};
}catch(e){_._DumpException(e)}
try{
var ad=class extends _.O{constructor(){super()}};var bd=class extends _.P{constructor(){super();this.j=[];this.i=[]}o(a,b){this.j.push({features:a,options:b})}init(a,b,c){window.gapi={};var d=window.___jsl={};d.h=_.x(_.G(a,1));null!=_.F(a,12)&&(d.dpo=_.w(_.I(a,12)));d.ms=_.x(_.G(a,2));d.m=_.x(_.G(a,3));d.l=[];_.J(b,1)&&(a=_.G(b,3))&&this.i.push(a);_.J(c,1)&&(c=_.G(c,2))&&this.i.push(c);_.z("gapi.load",(0,_.y)(this.o,this));return this}};var cd=_.C(_.Mc,_.Dc,14);if(cd){var dd=_.C(_.Mc,_.$c,9)||new _.$c,ed=new ad,fd=new bd;fd.init(cd,dd,ed);_.Uc("gs",fd)};
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script><script nonce="">try {const preferences = JSON.parse(window.localStorage.getItem("datalab_prefs_maryaamjabbari@gmail.com")); document.querySelector('html') .setAttribute('theme', preferences['siteTheme'] || 'default');} catch (e) {}</script><script nonce="">window.performance.mark('head_start');</script><link rel="stylesheet" href="./DataMining_Project3_HSM.ipynb - Colab_files/bundle.css"><script nonce="">var colabVersionTag = 'colab_20240606-060106_RC00_640854796'; var colabScsVersion = 'dd376bea74f0519c3e5384e119cf7f59'; var hl = 'en'; var colabExperiments = JSON.parse('\x7b\x22ai_unsubscribed_warning\x22: true, \x22aida_complete_code_model_id\x22: \x22\x22, \x22aida_do_conversation_model_id\x22: \x22\x22, \x22aida_generate_code_model_id\x22: \x22\x22, \x22aida_in_editor\x22: false, \x22allowed_public_url_domains\x22: \x5b\x22huggingface.co\x22, \x22dagshub.com\x22, \x22storage.googleapis.com\x22\x5d, \x22auto_execute_prereqs\x22: false, \x22backend_version\x22: \x22next\x22, \x22cell_tags\x22: false, \x22chat\x22: true, \x22chat_model_id_override\x22: \x22\x22, \x22classified_generate\x22: false, \x22classroom_iframe_parent_origin\x22: \x22\x22, \x22client_text_compose\x22: true, \x22client_trim_completion_text\x22: 400, \x22cloud_origin\x22: \x22\x22, \x22commands_in_toolbar\x22: false, \x22comment_poll_long\x22: 900000, \x22comment_poll_short\x22: 60000, \x22compose_skip_suffix_check\x22: false, \x22converse_server_side_history\x22: false, \x22converse_temp\x22: \x22\x22, \x22crawler\x22: false, \x22critique_comments\x22: false, \x22dbu\x22: \x22\x22, \x22debug_external\x22: \x22external\x22, \x22debug_prod\x22: \x22prod\x22, \x22dep_cells_commands\x22: false, \x22dep_graph\x22: false, \x22development\x22: false, \x22document_change_poll_interval\x22: 30000, \x22drive_anon_api_key\x22: \x22AIzaSyB10s2vWUTwP0pj20wZoxmpZIt3rRodYeg\x22, \x22drive_api_key\x22: \x22AIzaSyCN_sSPJMpYrAzC5AtTrltNC8oRmLtoqBk\x22, \x22drive_background_save_project_number\x22: \x22948411933973\x22, \x22drive_realtime_project_number\x22: \x22\x22, \x22embedded_connection_poll\x22: false, \x22embedding_app\x22: \x22\x22, \x22enable_adhoc_backends\x22: false, \x22enable_more_reprs\x22: true, \x22explain_cell\x22: false, \x22explain_error\x22: true, \x22explain_error_model_id_override\x22: \x22\x22, \x22explain_error_prompt_next\x22: true, \x22explain_error_trim_traceback\x22: true, \x22external_trusted_github_org_repos_quick_add\x22: \x22GoogleChrome\/CrUX,google\/generative-ai-docs\x22, \x22file_upload_rate_limit\x22: 5, \x22filter_repetitive_suggestions\x22: false, \x22first_party_auth\x22: true, \x22fix_imports\x22: false, \x22gemini_rebrand\x22: true, \x22generate_code\x22: true, \x22generate_df\x22: true, \x22generate_prompt_reduce_name_errors\x22: false, \x22generate_temp\x22: \x22\x22, \x22get_started\x22: false, \x22gis_auth\x22: true, \x22github_client_id\x22: \x225036cf6d81e65aaa6340\x22, \x22gpu_utilization_check_interval_ms\x22: 600000, \x22granular_browser_permissions\x22: false, \x22hats_surveys\x22: true, \x22hrc\x22: false, \x22import_data\x22: false, \x22inline_completions_persist_toolbar\x22: false, \x22interactive_sheet_next_steps\x22: false, \x22internal_chat\x22: false, \x22internal_schedule\x22: false, \x22is_prober\x22: false, \x22jsraw\x22: \x22compiled\x22, \x22key_promoter\x22: false, \x22kr\x22: false, \x22local_cloud_apis\x22: false, \x22local_service_worker\x22: false, \x22lsp_diagnostic_threshold_b312769838\x22: 0, \x22lsp_diagnostics_reporting\x22: false, \x22lsp_inlay_hint\x22: false, \x22lsrp\x22: 0, \x22ml_banner\x22: false, \x22ml_enabled\x22: false, \x22mlpp\x22: false, \x22mlpp_multiline\x22: false, \x22mlpp_on_by_default\x22: true, \x22mobile\x22: false, \x22next_steps\x22: true, \x22nl2code_missing_imports\x22: true, \x22no_fun\x22: false, \x22notebook_context_length\x22: 0, \x22outage_notification\x22: \x22\x22, \x22outage_notification_link\x22: \x22\x22, \x22output_menu\x22: true, \x22outputframe_version\x22: \x22\x22, \x22override_suf_params_for_test\x22: false, \x22recaptcha_polling_frequency_ms\x22: 300000, \x22recaptcha_v2_site_key\x22: \x226LfQttQUAAAAADuPanA_VZMaZgBAOnHZNuuqUewp\x22, \x22recaptcha_v3_site_key\x22: \x226LfQPtEUAAAAAHBpAdFng54jyuB1V5w5dofknpip\x22, \x22recent_borg_runtimes\x22: true, \x22reconnect_max_delay_seconds\x22: 300, \x22require_ai_consent\x22: true, \x22resource_poll_interval_ms\x22: 10000, \x22rp_kxhr\x22: false, \x22rp_lsp\x22: false, \x22rp_serve_kernel_port\x22: false, \x22rp_term\x22: true, \x22rp_token_refresh_headroom_millis\x22: 300000, \x22rt\x22: false, \x22runtime_env_overrides\x22: \x22\\n          \x5b\\n            \x5b\\\x22ENABLE_DIRECTORYPREFETCHER\\\x22, \\\x221\\\x22\x5d\\n          \x5d\\n        \x22, \x22runtime_type_for_test\x22: \x22\x22, \x22server_execution_queue\x22: true, \x22session_resume_coalesce\x22: true, \x22show_internal_ai_warning\x22: false, \x22show_payments_interstitial\x22: false, \x22show_relnotes_on_open\x22: true, \x22show_signup_survey\x22: true, \x22show_subscription_renewal_time\x22: false, \x22show_switch_to_prod_link\x22: false, \x22smartpaste\x22: false, \x22smartpaste_serving_config\x22: \x22pl_700m_smart_paste_3.0.25\x22, \x22sql_cell\x22: false, \x22sql_cell_buttons\x22: false, \x22storage_partition_trial\x22: true, \x22storage_partition_trial_token\x22: \x22AmUpB2+Hlwk73pYiEMbnkef\/dprJi1I9rClec33apyFsbVOaCIRN29Rk9M4ht5Otgbp+thCc3MMD73GyCNfEWAkAAAB3eyJvcmlnaW4iOiJodHRwczovL2NvbGFiLnJlc2VhcmNoLmdvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZyIsImV4cGlyeSI6MTcyNTQwNzk5OX0\x3d\x22, \x22suspicious_code_matches\x22: \x22\x22, \x22suspicious_code_regexs\x22: \x22\x22, \x22term4all\x22: false, \x22text_compose_report_changes_millis\x22: 10000, \x22text_span_comments\x22: false, \x22tpu_node_deprecation_warning\x22: true, \x22tpu_node_selector_grayed_out\x22: true, \x22tpu_node_selector_visible\x22: true, \x22tpu_vm\x22: true, \x22unmanaged_vm_min_label_block\x22: \x22\x22, \x22unmanaged_vm_min_label_warn\x22: \x22\x22, \x22unmanaged_vm_min_release_tag_block\x22: \x22\x22, \x22unmanaged_vm_min_release_tag_warn\x22: \x22\x22, \x22use_corplogin\x22: true, \x22use_dm_sql_lsp\x22: false, \x22use_upticks_for_internalai\x22: false, \x22user_visible_gpu_types\x22: \x5b\x22T4\x22, \x22V100\x22, \x22A100\x22, \x22L4\x22\x5d, \x22verbose_warnings\x22: false, \x22vertex_ai_api_environment_override\x22: \x22\x22, \x22waffle\x22: false, \x22workstations\x22: false, \x22ids\x22: \x5b20730159, 20730177, 20730189, 20730129, 20730224, 20730183, 20730252, 20730150, 20730185, 20730250, 20730230\x5d, \x22flag_ids\x22: \x7b\x22ai_unsubscribed_warning\x22: 45504730, \x22aida_complete_code_model_id\x22: 45427660, \x22aida_do_conversation_model_id\x22: 45427664, \x22aida_generate_code_model_id\x22: 45427663, \x22aida_in_editor\x22: 45425507, \x22allowed_public_url_domains\x22: 45425558, \x22auto_execute_prereqs\x22: 45624305, \x22backend_version\x22: 45425541, \x22cell_tags\x22: 45425779, \x22chat\x22: 45425490, \x22chat_model_id_override\x22: 45631876, \x22classified_generate\x22: 45425499, \x22classroom_iframe_parent_origin\x22: 45425537, \x22client_text_compose\x22: 45425512, \x22client_trim_completion_text\x22: 45425628, \x22cloud_origin\x22: 45425538, \x22commands_in_toolbar\x22: 45425502, \x22comment_poll_long\x22: 45425588, \x22comment_poll_short\x22: 45425587, \x22compose_skip_suffix_check\x22: 45615470, \x22converse_server_side_history\x22: 45634472, \x22converse_temp\x22: 45425509, \x22crawler\x22: 45425491, \x22critique_comments\x22: 45612076, \x22dbu\x22: 45425545, \x22debug_external\x22: 45425470, \x22debug_prod\x22: 45425471, \x22dep_cells_commands\x22: 45622249, \x22dep_graph\x22: 45629071, \x22development\x22: 45425544, \x22document_change_poll_interval\x22: 45425589, \x22drive_anon_api_key\x22: 45425478, \x22drive_api_key\x22: 45425473, \x22drive_background_save_project_number\x22: 45425479, \x22drive_realtime_project_number\x22: 45425629, \x22embedded_connection_poll\x22: 45491618, \x22enable_adhoc_backends\x22: 45425506, \x22enable_more_reprs\x22: 45613354, \x22explain_cell\x22: 45425505, \x22explain_error\x22: 45425487, \x22explain_error_model_id_override\x22: 45631875, \x22explain_error_prompt_next\x22: 45615229, \x22explain_error_trim_traceback\x22: 45618831, \x22external_trusted_github_org_repos_quick_add\x22: 45425555, \x22file_upload_rate_limit\x22: 45637799, \x22filter_repetitive_suggestions\x22: 45615781, \x22first_party_auth\x22: 45425560, \x22fix_imports\x22: 45624140, \x22gemini_rebrand\x22: 45631310, \x22generate_code\x22: 45425492, \x22generate_df\x22: 45425503, \x22generate_prompt_reduce_name_errors\x22: 45634392, \x22generate_temp\x22: 45425508, \x22get_started\x22: 45430267, \x22gis_auth\x22: 45425625, \x22github_client_id\x22: 45425556, \x22gpu_utilization_check_interval_ms\x22: 45425561, \x22granular_browser_permissions\x22: 45630936, \x22hats_surveys\x22: 45425559, \x22import_data\x22: 45430411, \x22inline_completions_persist_toolbar\x22: 45630170, \x22interactive_sheet_next_steps\x22: 45634324, \x22internal_chat\x22: 45622872, \x22internal_schedule\x22: 45425578, \x22is_prober\x22: 45429104, \x22jsraw\x22: 45425557, \x22key_promoter\x22: 45425570, \x22local_cloud_apis\x22: 45425630, \x22local_service_worker\x22: 45425550, \x22lsp_diagnostic_threshold_b312769838\x22: 45618432, \x22lsp_diagnostics_reporting\x22: 45425604, \x22lsp_inlay_hint\x22: 45614695, \x22lsrp\x22: 45425612, \x22ml_banner\x22: 45425631, \x22ml_enabled\x22: 45425493, \x22mlpp\x22: 45425608, \x22mlpp_multiline\x22: 45425623, \x22mlpp_on_by_default\x22: 45425609, \x22mobile\x22: 45425562, \x22next_steps\x22: 45428239, \x22nl2code_missing_imports\x22: 45615676, \x22no_fun\x22: 45425540, \x22notebook_context_length\x22: 45633457, \x22outage_notification\x22: 45425584, \x22outage_notification_link\x22: 45425585, \x22output_menu\x22: 45617054, \x22outputframe_version\x22: 45425591, \x22override_suf_params_for_test\x22: 45425592, \x22recaptcha_polling_frequency_ms\x22: 45425582, \x22recaptcha_v2_site_key\x22: 45425581, \x22recaptcha_v3_site_key\x22: 45425580, \x22recent_borg_runtimes\x22: 45632689, \x22reconnect_max_delay_seconds\x22: 45425539, \x22require_ai_consent\x22: 45425489, \x22resource_poll_interval_ms\x22: 45425590, \x22rp_kxhr\x22: 45491686, \x22rp_lsp\x22: 45462965, \x22rp_serve_kernel_port\x22: 45572083, \x22rp_term\x22: 45426219, \x22rp_token_refresh_headroom_millis\x22: 45517773, \x22rt\x22: 45425624, \x22runtime_env_overrides\x22: 45425583, \x22runtime_type_for_test\x22: 45425586, \x22server_execution_queue\x22: 45425600, \x22session_resume_coalesce\x22: 45425603, \x22show_internal_ai_warning\x22: 45622780, \x22show_payments_interstitial\x22: 45425543, \x22show_relnotes_on_open\x22: 45428128, \x22show_signup_survey\x22: 45425620, \x22show_subscription_renewal_time\x22: 45425569, \x22show_switch_to_prod_link\x22: 45425483, \x22smartpaste\x22: 45627425, \x22smartpaste_serving_config\x22: 45630585, \x22sql_cell\x22: 45425497, \x22sql_cell_buttons\x22: 45425498, \x22suspicious_code_matches\x22: 45425615, \x22suspicious_code_regexs\x22: 45425616, \x22term4all\x22: 45425542, \x22text_compose_report_changes_millis\x22: 45425568, \x22text_span_comments\x22: 45545873, \x22tpu_node_deprecation_warning\x22: 45630619, \x22tpu_node_selector_grayed_out\x22: 45630664, \x22tpu_node_selector_visible\x22: 45630663, \x22tpu_vm\x22: 45614812, \x22unmanaged_vm_min_label_block\x22: 45425546, \x22unmanaged_vm_min_label_warn\x22: 45425547, \x22unmanaged_vm_min_release_tag_block\x22: 45425548, \x22unmanaged_vm_min_release_tag_warn\x22: 45425549, \x22use_corplogin\x22: 45425606, \x22use_dm_sql_lsp\x22: 45425610, \x22use_upticks_for_internalai\x22: 45629267, \x22user_visible_gpu_types\x22: 45620529, \x22verbose_warnings\x22: 45425551, \x22vertex_ai_api_environment_override\x22: 45612077, \x22waffle\x22: 45446491, \x22workstations\x22: 45425626\x7d\x7d'); var colabUserEmail = 'maryaamjabbari@gmail.com'; var colabRenderDataToken = 'AFWLbD0L7l1kQWlOL-4Na245Y_CkYL4gIxL2CR7GqWbsok0m43geM-cwGWA1IX65Lv1EovecCbsQXH72RychjUzzVMLeAhHwFS6I'; var colabConfig = '\x5b\x5b\x22maryaamjabbari@gmail.com\x22,\x5b1,\x22AHXL0D3pnAzvcXxTy14avtsrq5ut4oPxISUlzMOlUtmLpIvifjBHR0I3DbRqyJzFF\/715a+hfQ3t3ujlTG+tvxnOzqulRvvuhh6Dt\/RcJrMfv2e5m+fx0YlJsvNUxlPhf6hEQrz8WSjGkFfkdWOF0n0RCH3IwWJfxKEHogm07yvgz8gVyDwjLEJfg8rMfg17s5COVaCLLusGX2q98fKZtnOcuNDWAL+j+8ZeqCLnyoDvnF7slBkp+0IpnjSDDT4cNAwpo52eLoPPLrevaeu9pk6i5tHYxYPg8GQLqxLUgX8KACJNCfiV4OfpFGwGjHscKnTQMYKy2JOEhvq5fRJ6qVlwqksbUZFBxVEi5us18Ibh4RkMskFKVL8BLFywkcjQZDB2u4TFFb+KaZRBJWJw\/STGMWjmbPvhgmIt20yTUlt486m98GTXWVDUNAes+4BXrB3mtbbssEKQ3P4NK08vfnoJVYEQGURAhTChYuEJomfKAdE5TKnQHnRPeiVJSI2Ad57BGTqt9XLFrMP16GE08iz8AMlGlPTBQnm+UsaowF3OeWDf4kuxwEhu9tc4XerOtPCwF9\/okvizmrMMIlTAxuzJ4riI1WGe2YunEK80O17cdEGUXejajNpoTh3EePhbXCcCt6MmH80hilP20c27viB8\/3YXJ2XzruR6CeI8MF\/pkvxenLiAw8tR75ObQnNnDlpsWDEgd4dBfK2JQLYkzYmv2owVzTCeZbOuZaZF+BBIUjnY5RiOJtd2XEdy7Yws0D79QGWTaCiYBlxgJccMuf47xlpzRki0e+py\/a5g904vDbht5oiYXrRE+LCICPKT7Av6GTrAMUzBpmUis8WCzohaJLn8LnFG10yBMBJpYd6vMoIp2J9vkdSESq5yLuoNf3JfY88ZdZpKcuqKrT9Fzpej9bSCeUNeNpwuBDunmmSiB+puYe+9dfF\/qRxP9rZiTXxwZ176IB8tDfA423Q4NiUy69lUE8MVg+dtXGdOTNO1HiM67l9+SKazyFxi\/r2p7ttqbqWmGCZAfGWE9sB\/7xUstc5lOpQIqD4Aj0UCPRI6z6PumRckHS6UCptA5r04S99qjmBiT+ZKauXGGYmACax8IAj\/B66QI39+GlXEfWjdrZVbPWKq9A4F9zB04zl3NldtBt\/0\/S0\/dSSRGOpuWCObdVoWmJ55\/ZunmM+\/yHRFObJHrEV\/yODzkaThcHsqj09I4edZkItaFtNsqCiqRpP8w5h7ePGY2EbFnQfpIXljy07APGkL0dBWdQ5mIQmwLkSv7W1ANGAMq6Al\/xCu3UgGMzlUEfnEVMLBlFOE2pavd1GlrldARslzHa4B9Fve6tDM0DgLWtkpKqnhv1KFDJtNso6x72t65lw6S3O82T4VD9XIyYCJw4scdT36jtEFtEWmcFTGhVHURCLHWQuRolct\/S\/Jjxre0v71QxX2nOawRAeG+61nl\/g20RUI7DOYWj9dNTG3m4Jn+0JLx5WkzAb9LCCAU4fAUoVl1nU8XXnZkBqDntJwWJRqtteih1\/aGCvDtvzdz3weQSzuVNPaflQCZB8dHwsoc9HGai2r\/3mESmTUo3qv9P9MNeaiD26+RDAlFSBojYv1OlqPSxTj32pxEJZpiH1J4ukZd9+qtm0+hJWUltLe2n9Fo2psuuim4\/kPKAqZAZ6ngMMqiq7qyJ+j3\/5x8G8lx29kiBG3QOPxqa3POlxsfXO9jmuwuT5OgTq+omYT9zbCjXS5AqVWopfwFck1Lt0oabRCBxOBsUU6Yb8qdWUDhyprZ4gy\/CW5StSN8w0L+7zY4RmMzn5K52SopScghqofjLIAqFRrZYIRAKanwENF45XTfcNOABn0K8Igr8J5fD6QzE4PR2kdyKMVnnVN8HmsG82E2D91P+ECjlIJUgupkTw\x3d\x22,\x22AJ9oCCwNJXjjSi2bsRoZX\/aSPCDtu2EXY5K\/ZYS2irstOe7FdRYn1Fu5zFLDD6BWoyKQmzmcuKdWzNN4azV+CXkoxrjYwMchz\/m7gzK\/VUiefBy8gkzHOhqr5b4vXhVlQHO1tKWmUTeP\x22,\x22https:\/\/payments.google.com\/payments\x22,0,0,null,null,null,\x22$9.99\x22,\x22$49.99\x22,\x22$9.99\x22,\x22$49.99\x22\x5d,\x5b4\x5d,\x22IR\x22\x5d\x5d';</script><link id="favicon-link" rel="shortcut icon" href="https://ssl.gstatic.com/colaboratory-static/common/dd376bea74f0519c3e5384e119cf7f59/img/favicon.ico"><meta name="google-site-verification" content="wRgpUU3mIRZPD1GORBPNonaotM72092B_DsqQFWNa4s"><meta name="google-site-verification" content="f5qdvL6RAXlBgHezvCLpPtvx2wU5ZgIzzPULroprlnA"><meta name="google-site-verification" content="-wL8iYJTC7X0zF9qBNDQUAd-P1ZkQUK-OhSgv4Wkf1M"><meta name="google-site-verification" content="o-EECwEDQeUpZv0jTmoGfCDX7dUI8Kul4ESepXmDnO0"><meta name="google-site-verification" content="sNOroO9gXrazN-oMODOm0Bs0_vw1R5QwZ-BfrSHn8Io"><meta name="google-site-verification" content="K1UdZBHJXQYnJGXIK1KuutmVy6dn3vG2sEyV9D1C6dM"><meta name="google-site-verification" content="wdGthzzfu0IjM3qpFqTuQL9poAQZAvAaFKyuzetLpIM"><meta name="google-site-verification" content="qZJ77guHGO0TObHUBRYVdXQlIhXBBuz8dahJVmIlzCo"><meta name="google-site-verification" content="7ahoeOOKT2ZR781GZ5xK4L9t7yO1ZOHc-gaoUALEYgw"><meta name="google-site-verification" content="PHgaSKwdxZELS21aixtLhfpvaHtKen9pnVJ25EI35Zs"><meta name="google-site-verification" content="Ozey1ptWUQW13_lCEhpPMOcmRBLqdyB3WEL-TJUjskU"><meta name="google-site-verification" content="rF5iXzWe9KZXJes1dQNhOUkS4_z_e97IrsVoCx2trek"><meta name="google-site-verification" content="z-WR3zzv8XZ5FFfBLLDbyTiN35UXm01nWUS2Uej5pwg"><meta name="google-site-verification" content="cpB5oulaGwqSxsg4E-9q2MVbK87iE9NAUUVxdveucPw"><meta name="google-site-verification" content="8P-D5fVWgUIhw8X2BxnKJbf5itK0zxX0QhoBjbJFTe8"><meta name="google-site-verification" content="88fgsZDoVRBuRnDPMIEjcHCxsEXzODOqEsJoqtvQsDc"><meta name="google-site-verification" content="sMarhZgb4va_L_7UTdMR43gDZ2gVqc_5GHN4REpQPGY"><meta name="google-site-verification" content="26aKGBCw3XblB5Ou01UhxY5WDtMqHjoTm6P-lvF6AqE"><meta name="google-site-verification" content="DGionF7db9g0dOgeBXwOAN2tmCzWBdo5yOdc_-5UcuE"><meta name="google-site-verification" content="Q9LlidR0toR7UtSyVO23xNeaqJmRp8I6r4ghBQTtntU"><meta name="google-site-verification" content="rQawcZaTEK_UrDG30cz_7nVKOVvBass61QEes0Tm04g"><meta name="google-site-verification" content="8L3ghjzKIj241AYAmEygniTe604tsXFkIrb1v-DBtGo"><meta name="google-site-verification" content="Osw7QcOK045GmOYJI2MM2_7AaL-s4q6pdn8gIv6JNxA"><meta name="google-site-verification" content="KiunYPvrY5x8umvAWcjhwPrB677xCar2LeT_8yaVrDg"><meta name="google-site-verification" content="b6bOMRzMVX2bJABYDGBPtpGcB_AUZ-o2SOTggQXErkg"><meta name="google-site-verification" content="v2MQvJk6wTiBarKTbe1mdivqYCVtw-5m6w0HDzV5X_4"><meta name="google-site-verification" content="-N1hdkiHJQ6kwJALkHVh2ZzV2fFNER0schZl2AU6zvc"><meta property="og:type" content="article"><meta property="og:image" content="https://colab.research.google.com/img/colab_favicon_256px.png"><meta property="og:title" content="Google Colab"><meta http-equiv="origin-trial" content="AmUpB2+Hlwk73pYiEMbnkef/dprJi1I9rClec33apyFsbVOaCIRN29Rk9M4ht5Otgbp+thCc3MMD73GyCNfEWAkAAAB3eyJvcmlnaW4iOiJodHRwczovL2NvbGFiLnJlc2VhcmNoLmdvb2dsZS5jb206NDQzIiwiZmVhdHVyZSI6IkRpc2FibGVUaGlyZFBhcnR5U3RvcmFnZVBhcnRpdGlvbmluZyIsImV4cGlyeSI6MTcyNTQwNzk5OX0="><script nonce="">window.performance.mark('head_end'); window.performance.measure('head', 'head_start', 'head_end');</script><script async="" src="./DataMining_Project3_HSM.ipynb - Colab_files/lazy.min.js.download" nonce=""></script><style id="inert-style">
[inert] {
  pointer-events: none;
  cursor: default;
}

[inert], [inert] * {
  user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
}
</style><style>
    html {
      <!---->
      <!---->
      --code-cell-background: #f7f7f7;
      --colab-anchor-color: #00e;
      --colab-border-color: #dadada;
      --colab-bold-border-color: #111;
      --colab-callout-color: var(--paper-blue-700);
      --colab-divider-color: var(--paper-grey-300);
      --colab-debugger-line-color: var(--paper-red-100);
      --colab-editor-focus-color: var(--paper-grey-200);
      --colab-highlighted-surface-color: var(--paper-grey-200);
      --colab-icon-color: var(--paper-grey-700);
      --colab-input-button-hover-background: #6161611a;
      --colab-secondary-icon-color: #93adcf;
      --colab-input-placeholder-color: var(--colab-secondary-text-color);
      --colab-primary-surface-color: var(--paper-white);
      --colab-primary-text-color: var(--paper-grey-900);
      --colab-secondary-text-color: #616161;
      --colab-tertiary-text-color: var(--paper-grey-600);
      --colab-secondary-surface-color: #f7f7f7;
      --colab-snackbar-surface-color: #333333;
      --colab-scrollbar-color: rgba(0, 0, 0, 0.1);
      --colab-gutter-icon-color: #8c8c8c;
      --colab-active-execution-icon-color: var(--paper-grey-800);
      --colab-error-icon-color: var(--paper-red-a700);
      --colab-title-color: #000;
      --colab-form-field-underline-color: var(--paper-grey-400);
      --colab-editor-focus-border-thickness: 2px;
      --colab-diff-editor-background: #fff;
      --colab-local-diff-background: #eef;
      --colab-remote-diff-background: #feffe0;
      --colab-merged-diff-background: #d7fed8;
      --colab-status-okay: var(--google-green-700);
      --ansi-black: rgb(0, 0, 0);
      --ansi-red: rgb(139, 0, 0);
      --ansi-green: rgb(0, 100, 0);
      --ansi-yellow: rgb(205, 205, 0);
      --ansi-blue: rgb(0, 0, 238);
      --ansi-magenta: rgb(205, 0, 205);
      --ansi-cyan: rgb(70, 130, 180);
      --ansi-gray: rgb(229, 229, 229);
      --ansi-bright-black: rgb(127, 127, 127);
      --ansi-bright-red: rgb(255, 0, 0);
      --ansi-bright-green: rgb(0, 208, 0);
      --ansi-bright-yellow: rgb(255, 255, 0);
      --ansi-bright-blue: rgb(92, 92, 255);
      --ansi-bright-magenta: rgb(255, 0, 255);
      --ansi-bright-cyan: rgb(0, 255, 255);
      --ansi-bright-gray: rgb(255, 255, 255);
      --gcp-success-icon-color: var(--google-green-700);
      --colab-comment-anchor-color: var(--google-blue-600);
      --colab-filled-button-ripple-color: #000;
      --colab-comment-highlight-color: #ffe082; /* material amber-200 */
      --colab-smartpaste-highlight-color: rgba(255, 224, 130, 0.5);
      <!---->
      --colab-input-border-color: #a9a9a9;
      --colab-logo-dark: var(--google-orange-600);
      --colab-logo-light: var(--google-yellow-600);
      --colab-status-error: #e51c23;
      --colab-status-warning: #f09300;
      --colab-chrome-font-family: 'Roboto', 'Noto', sans-serif;
      --colab-google-sans-font-family: 'Google Sans', 'Roboto', 'Noto',
        sans-serif;
      --colab-chrome-font-size: 14px;
      <!---->
      --colab-icon-hover-color: var(--colab-primary-text-color);
      --colab-fresh-execution-count-color: var(--colab-primary-text-color);
      --colab-stale-execution-count-color: var(--colab-input-placeholder-color);
      --error-color: #b3261e;
      --primary-color: var(--google-blue-700);
      --google-green-700: #188038;
      --google-grey-800: #3c4043;
      --google-blue-200: #aecbfa;
      --google-blue-300: #8ab4f8;
      --google-blue-700: #1967d2;
      --google-blue-900: #174ea6;
      --hairline-button-secondary: var(--google-blue-900);
      --mdc-theme-primary: var(--primary-color);
      --mdc-theme-on-primary: var(--colab-primary-surface-color);
      --md-sys-color-primary: var(--primary-color);
      --md-sys-color-on-primary: var(--colab-primary-surface-color);
    }
    html[theme='dark'] {
      <!---->
      --colab-anchor-color: var(--paper-blue-300);
      --colab-callout-color: var(--google-blue-600);
      --code-cell-background: #1e1e1e;
      --colab-border-color: var(--paper-grey-700);
      --colab-bold-border-color: #eee;
      --colab-divider-color: var(--paper-grey-700);
      --colab-debugger-line-color: var(--paper-red-900);
      --colab-editor-focus-color: #282828;
      --colab-highlighted-surface-color: #525252;
      --colab-icon-color: var(--paper-grey-400);
      --colab-input-button-hover-background: #bdbdbd1a;
      --colab-input-placeholder-color: var(--colab-tertiary-text-color);
      --colab-primary-surface-color: #383838;
      --colab-primary-text-color: #d5d5d5;
      --colab-secondary-text-color: #f7f7f7;
      --colab-tertiary-text-color: #b3b3b3;
      --colab-secondary-surface-color: #454545;
      --colab-snackbar-surface-color: var(--colab-secondary-surface-color);
      --colab-scrollbar-color: rgba(255, 255, 255, 0.2);
      --colab-gutter-icon-color: #858585;
      --colab-active-execution-icon-color: var(--colab-icon-color);
      --colab-error-icon-color: #ef5350;
      --colab-title-color: #fff;
      --colab-form-field-underline-color: var(--paper-grey-600);
      --colab-diff-editor-background: #000;
      --colab-local-diff-background: #292935;
      --colab-remote-diff-background: #2e2f08;
      --colab-merged-diff-background: #09380b;
      --colab-status-okay: #00c752;
      --ansi-black: rgb(127, 127, 127);
      --ansi-red: rgb(255, 122, 136);
      --ansi-green: rgb(87, 187, 138);
      --ansi-yellow: rgb(255, 255, 102);
      --ansi-blue: rgb(130, 177, 255);
      --ansi-magenta: rgb(205, 0, 205);
      --ansi-cyan: rgb(153, 187, 215);
      --ansi-gray: rgb(229, 229, 229);
      --ansi-bright-green: rgb(0, 255, 0);
      --gcp-success-icon-color: #81c995;
      --colab-comment-anchor-color: var(--paper-blue-300);
      --colab-filled-button-ripple-color: #fff;
      --colab-comment-highlight-color: #1a237e; /* material indigo-900 */
      --colab-smartpaste-highlight-color: rgba(255, 224, 130, 0.3);
      --error-color: var(--paper-deep-orange-a100);
      --primary-color: var(--google-blue-300);
      --hairline-button-secondary: var(--google-blue-200);
    }
    @media (prefers-color-scheme: dark) {
      html[theme='adaptive'] {
        <!---->
        --colab-anchor-color: var(--paper-blue-400);
        --colab-callout-color: var(--paper-blue-900);
        --code-cell-background: #1e1e1e;
        --colab-border-color: var(--paper-grey-700);
        --colab-bold-border-color: #eee;
        --colab-divider-color: var(--paper-grey-700);
        --colab-debugger-line-color: var(--paper-red-900);
        --colab-editor-focus-color: #282828;
        --colab-highlighted-surface-color: #525252;
        --colab-icon-color: var(--paper-grey-100);
        --colab-input-button-hover-background: #bdbdbd1a;
        --colab-input-placeholder-color: var(--colab-tertiary-text-color);
        --colab-primary-surface-color: #383838;
        --colab-primary-text-color: #d5d5d5;
        --colab-secondary-text-color: #f7f7f7;
        --colab-tertiary-text-color: #b3b3b3;
        --colab-secondary-surface-color: #454545;
        --colab-snackbar-surface-color: var(--colab-secondary-surface-color);
        --colab-scrollbar-color: rgba(255, 255, 255, 0.2);
        --colab-gutter-icon-color: #858585;
        --colab-execution-count: var(--colab-primary-text-color);
        --colab-active-execution-icon-color: var(--colab-icon-color);
        --colab-error-icon-color: #ef5350;
        --colab-title-color: #fff;
        --colab-form-field-underline-color: var(--paper-grey-600);
        --colab-diff-editor-background: #000;
        --colab-local-diff-background: #292935;
        --colab-remote-diff-background: #2e2f08;
        --colab-merged-diff-background: #09380b;
        --colab-status-okay: #00c752;
        --ansi-black: rgb(63, 63, 63);
        --ansi-red: rgb(255, 122, 136);
        --ansi-green: rgb(87, 187, 138);
        --ansi-yellow: rgb(255, 255, 102);
        --ansi-blue: rgb(130, 177, 255);
        --ansi-magenta: rgb(205, 0, 205);
        --ansi-cyan: rgb(153, 187, 215);
        --ansi-gray: rgb(229, 229, 229);
        --colab-filled-button-ripple-color: #fff;
        --error-color: var(--paper-deep-orange-a100);
        --primary-color: var(--google-blue-300);
        --hairline-button-secondary: var(--google-blue-200);
      }
    }
    html[editor='High Contrast Dark'] {
      --code-cell-background: #000;
      --colab-editor-focus-color: #f38518;
      --colab-editor-focus-border-thickness: 1px;
    }
    html[editor='Monokai'] {
      --code-cell-background: #272822;
    }
    html[editor='All Hallows Eve'] {
      --code-cell-background: #000;
    }
    html[editor='Amy'] {
      --code-cell-background: #200020;
    }
    html[editor='Birds Of Paradise'] {
      --code-cell-background: #372725;
    }
    html[editor='Blackboard'] {
      --code-cell-background: #0c1021;
    }
    html[editor='Clouds Midnight'] {
      --code-cell-background: #191919;
    }
    html[editor='Dominion Day'] {
      --code-cell-background: #372725;
    }
    html[editor='Espresso Libre'] {
      --code-cell-background: #2a211c;
    }
    html[editor='Merbivore'] {
      --code-cell-background: #161616;
    }
    html[editor='Night Owl'] {
      --code-cell-background: #011627;
    }
    html[editor='Oceanic Next'] {
      --code-cell-background: #1b2b34;
    }
    html[editor='Pastels On Dark'] {
      --code-cell-background: #211e1e;
    }
    html[editor='Space Cadet'] {
      --code-cell-background: #0d0d0d;
    }
    html[editor='Sunburst'] {
      --code-cell-background: #000;
    }
    html[editor='Twilight'] {
      --code-cell-background: #141414;
    }
    html[editor='Vibrant Ink'] {
      --code-cell-background: #000;
    }
    html[editor='Zenburnesque'] {
      --code-cell-background: #404040;
    }
    html[editor='Idle Fingers'] {
      --code-cell-background: #323232;
    }
    html[editor='Mono Industrial'] {
      --code-cell-background: #222c28;
    }
    html[editor='Synthwave84'] {
      --colab-primary-surface-color: #241b2f;
      --colab-secondary-surface-color: #49549539;
      --code-cell-background: #262335;
      --colab-highlighted-surface-color: #372d4b;
      --colab-border-color: #34294fb3;
      --colab-anchor-color: #f97e72;
      --ansi-red: #fe4450;
      --ansi-green: #72f1b8;
      --ansi-yellow: #f97e72;
      --ansi-blue: #03edf9;
      --ansi-magenta: #ff7edb;
      --ansi-cyan: #03edf9;
      --ansi-bright-red: #fe4450;
      --ansi-bright-green: #72f1b8;
      --ansi-bright-yellow: #fede5d;
      --ansi-bright-blue: #03edf9;
      --ansi-bright-magenta: #ff7edb;
      --ansi-bright-cyan: #03edf9;
    }
    <!---->
  <!----></style><script async="async" type="text/javascript" src="./DataMining_Project3_HSM.ipynb - Colab_files/editor.main.js.download"></script><script async="" type="text/javascript" charset="UTF-8" src="./DataMining_Project3_HSM.ipynb - Colab_files/rs=AA2YrTtmD1oWXfR6WhUiAKksxBHsMK4_SQ" nonce=""></script><link type="text/css" rel="stylesheet" href="./DataMining_Project3_HSM.ipynb - Colab_files/rs=AA2YrTuUoxtuyUDvYGtQ10hK7I_33XgLMg"><link rel="stylesheet" type="text/css" data-name="vs/editor/editor.main" href="./DataMining_Project3_HSM.ipynb - Colab_files/editor.main.css"><script async="async" type="text/javascript" src="./DataMining_Project3_HSM.ipynb - Colab_files/editor.main.nls.js.download"></script><style type="text/css">.MathJax_Hover_Frame {border-radius: .25em; -webkit-border-radius: .25em; -moz-border-radius: .25em; -khtml-border-radius: .25em; box-shadow: 0px 0px 15px #83A; -webkit-box-shadow: 0px 0px 15px #83A; -moz-box-shadow: 0px 0px 15px #83A; -khtml-box-shadow: 0px 0px 15px #83A; border: 1px solid #A6D ! important; display: inline-block; position: absolute}
.MathJax_Menu_Button .MathJax_Hover_Arrow {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 4px; -webkit-border-radius: 4px; -moz-border-radius: 4px; -khtml-border-radius: 4px; font-family: 'Courier New',Courier; font-size: 9px; color: #F0F0F0}
.MathJax_Menu_Button .MathJax_Hover_Arrow span {display: block; background-color: #AAA; border: 1px solid; border-radius: 3px; line-height: 0; padding: 4px}
.MathJax_Hover_Arrow:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_Hover_Arrow:hover span {background-color: #CCC!important}
</style><style type="text/css">#MathJax_About {position: fixed; left: 50%; width: auto; text-align: center; border: 3px outset; padding: 1em 2em; background-color: #DDDDDD; color: black; cursor: default; font-family: message-box; font-size: 120%; font-style: normal; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; border-radius: 15px; -webkit-border-radius: 15px; -moz-border-radius: 15px; -khtml-border-radius: 15px; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_About.MathJax_MousePost {outline: none}
.MathJax_Menu {position: absolute; background-color: white; color: black; width: auto; padding: 2px; border: 1px solid #CCCCCC; margin: 0; cursor: default; font: menu; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
.MathJax_MenuItem {padding: 2px 2em; background: transparent}
.MathJax_MenuArrow {position: absolute; right: .5em; padding-top: .25em; color: #666666; font-size: .75em}
.MathJax_MenuActive .MathJax_MenuArrow {color: white}
.MathJax_MenuArrow.RTL {left: .5em; right: auto}
.MathJax_MenuCheck {position: absolute; left: .7em}
.MathJax_MenuCheck.RTL {right: .7em; left: auto}
.MathJax_MenuRadioCheck {position: absolute; left: 1em}
.MathJax_MenuRadioCheck.RTL {right: 1em; left: auto}
.MathJax_MenuLabel {padding: 2px 2em 4px 1.33em; font-style: italic}
.MathJax_MenuRule {border-top: 1px solid #CCCCCC; margin: 4px 1px 0px}
.MathJax_MenuDisabled {color: GrayText}
.MathJax_MenuActive {background-color: Highlight; color: HighlightText}
.MathJax_MenuDisabled:focus, .MathJax_MenuLabel:focus {background-color: #E8E8E8}
.MathJax_ContextMenu:focus {outline: none}
.MathJax_ContextMenu .MathJax_MenuItem:focus {outline: none}
#MathJax_AboutClose {top: .2em; right: .2em}
.MathJax_Menu .MathJax_MenuClose {top: -10px; left: -10px}
.MathJax_MenuClose {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; font-family: 'Courier New',Courier; font-size: 24px; color: #F0F0F0}
.MathJax_MenuClose span {display: block; background-color: #AAA; border: 1.5px solid; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; line-height: 0; padding: 8px 0 6px}
.MathJax_MenuClose:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_MenuClose:hover span {background-color: #CCC!important}
.MathJax_MenuClose:hover:focus {outline: none}
</style><style type="text/css">.MJX_Assistive_MathML {position: absolute!important; top: 0; left: 0; clip: rect(1px, 1px, 1px, 1px); padding: 1px 0 0 0!important; border: 0!important; height: 1px!important; width: 1px!important; overflow: hidden!important; display: block!important; -webkit-touch-callout: none; -webkit-user-select: none; -khtml-user-select: none; -moz-user-select: none; -ms-user-select: none; user-select: none}
.MJX_Assistive_MathML.MJX_Assistive_MathML_Block {width: 100%!important}
</style><style type="text/css">#MathJax_Zoom {position: absolute; background-color: #F0F0F0; overflow: auto; display: block; z-index: 301; padding: .5em; border: 1px solid black; margin: 0; font-weight: normal; font-style: normal; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; -webkit-box-sizing: content-box; -moz-box-sizing: content-box; box-sizing: content-box; box-shadow: 5px 5px 15px #AAAAAA; -webkit-box-shadow: 5px 5px 15px #AAAAAA; -moz-box-shadow: 5px 5px 15px #AAAAAA; -khtml-box-shadow: 5px 5px 15px #AAAAAA; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_ZoomOverlay {position: absolute; left: 0; top: 0; z-index: 300; display: inline-block; width: 100%; height: 100%; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
#MathJax_ZoomFrame {position: relative; display: inline-block; height: 0; width: 0}
#MathJax_ZoomEventTrap {position: absolute; left: 0; top: 0; z-index: 302; display: inline-block; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
</style><style type="text/css">.MathJax_Preview {color: #888}
#MathJax_Message {position: fixed; left: 1em; bottom: 1.5em; background-color: #E6E6E6; border: 1px solid #959595; margin: 0px; padding: 2px 8px; z-index: 102; color: black; font-size: 80%; width: auto; white-space: nowrap}
#MathJax_MSIE_Frame {position: absolute; top: 0; left: 0; width: 0px; z-index: 101; border: 0px; margin: 0px; padding: 0px}
.MathJax_Error {color: #CC0000; font-style: italic}
</style><style type="text/css">.MJXp-script {font-size: .8em}
.MJXp-right {-webkit-transform-origin: right; -moz-transform-origin: right; -ms-transform-origin: right; -o-transform-origin: right; transform-origin: right}
.MJXp-bold {font-weight: bold}
.MJXp-italic {font-style: italic}
.MJXp-scr {font-family: MathJax_Script,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-frak {font-family: MathJax_Fraktur,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-sf {font-family: MathJax_SansSerif,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-cal {font-family: MathJax_Caligraphic,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-mono {font-family: MathJax_Typewriter,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-largeop {font-size: 150%}
.MJXp-largeop.MJXp-int {vertical-align: -.2em}
.MJXp-math {display: inline-block; line-height: 1.2; text-indent: 0; font-family: 'Times New Roman',Times,STIXGeneral,serif; white-space: nowrap; border-collapse: collapse}
.MJXp-display {display: block; text-align: center; margin: 1em 0}
.MJXp-math span {display: inline-block}
.MJXp-box {display: block!important; text-align: center}
.MJXp-box:after {content: " "}
.MJXp-rule {display: block!important; margin-top: .1em}
.MJXp-char {display: block!important}
.MJXp-mo {margin: 0 .15em}
.MJXp-mfrac {margin: 0 .125em; vertical-align: .25em}
.MJXp-denom {display: inline-table!important; width: 100%}
.MJXp-denom > * {display: table-row!important}
.MJXp-surd {vertical-align: top}
.MJXp-surd > * {display: block!important}
.MJXp-script-box > *  {display: table!important; height: 50%}
.MJXp-script-box > * > * {display: table-cell!important; vertical-align: top}
.MJXp-script-box > *:last-child > * {vertical-align: bottom}
.MJXp-script-box > * > * > * {display: block!important}
.MJXp-mphantom {visibility: hidden}
.MJXp-munderover, .MJXp-munder {display: inline-table!important}
.MJXp-over {display: inline-block!important; text-align: center}
.MJXp-over > * {display: block!important}
.MJXp-munderover > *, .MJXp-munder > * {display: table-row!important}
.MJXp-mtable {vertical-align: .25em; margin: 0 .125em}
.MJXp-mtable > * {display: inline-table!important; vertical-align: middle}
.MJXp-mtr {display: table-row!important}
.MJXp-mtd {display: table-cell!important; text-align: center; padding: .5em 0 0 .5em}
.MJXp-mtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-mlabeledtr {display: table-row!important}
.MJXp-mlabeledtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mlabeledtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 1px 3px; font-style: normal; font-size: 90%}
.MJXp-scale0 {-webkit-transform: scaleX(.0); -moz-transform: scaleX(.0); -ms-transform: scaleX(.0); -o-transform: scaleX(.0); transform: scaleX(.0)}
.MJXp-scale1 {-webkit-transform: scaleX(.1); -moz-transform: scaleX(.1); -ms-transform: scaleX(.1); -o-transform: scaleX(.1); transform: scaleX(.1)}
.MJXp-scale2 {-webkit-transform: scaleX(.2); -moz-transform: scaleX(.2); -ms-transform: scaleX(.2); -o-transform: scaleX(.2); transform: scaleX(.2)}
.MJXp-scale3 {-webkit-transform: scaleX(.3); -moz-transform: scaleX(.3); -ms-transform: scaleX(.3); -o-transform: scaleX(.3); transform: scaleX(.3)}
.MJXp-scale4 {-webkit-transform: scaleX(.4); -moz-transform: scaleX(.4); -ms-transform: scaleX(.4); -o-transform: scaleX(.4); transform: scaleX(.4)}
.MJXp-scale5 {-webkit-transform: scaleX(.5); -moz-transform: scaleX(.5); -ms-transform: scaleX(.5); -o-transform: scaleX(.5); transform: scaleX(.5)}
.MJXp-scale6 {-webkit-transform: scaleX(.6); -moz-transform: scaleX(.6); -ms-transform: scaleX(.6); -o-transform: scaleX(.6); transform: scaleX(.6)}
.MJXp-scale7 {-webkit-transform: scaleX(.7); -moz-transform: scaleX(.7); -ms-transform: scaleX(.7); -o-transform: scaleX(.7); transform: scaleX(.7)}
.MJXp-scale8 {-webkit-transform: scaleX(.8); -moz-transform: scaleX(.8); -ms-transform: scaleX(.8); -o-transform: scaleX(.8); transform: scaleX(.8)}
.MJXp-scale9 {-webkit-transform: scaleX(.9); -moz-transform: scaleX(.9); -ms-transform: scaleX(.9); -o-transform: scaleX(.9); transform: scaleX(.9)}
.MathJax_PHTML .noError {vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
</style><style type="text/css">.MathJax_Display {text-align: center; margin: 0; position: relative; display: block!important; text-indent: 0; max-width: none; max-height: none; min-width: 0; min-height: 0; width: 100%}
.MathJax .merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 1px 3px; font-style: normal; font-size: 90%}
.MathJax .MJX-monospace {font-family: monospace}
.MathJax .MJX-sans-serif {font-family: sans-serif}
#MathJax_Tooltip {background-color: InfoBackground; color: InfoText; border: 1px solid black; box-shadow: 2px 2px 5px #AAAAAA; -webkit-box-shadow: 2px 2px 5px #AAAAAA; -moz-box-shadow: 2px 2px 5px #AAAAAA; -khtml-box-shadow: 2px 2px 5px #AAAAAA; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true'); padding: 3px 4px; z-index: 401; position: absolute; left: 0; top: 0; width: auto; height: auto; display: none}
.MathJax {display: inline; font-style: normal; font-weight: normal; line-height: normal; font-size: 100%; font-size-adjust: none; text-indent: 0; text-align: left; text-transform: none; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; direction: ltr; max-width: none; max-height: none; min-width: 0; min-height: 0; border: 0; padding: 0; margin: 0}
.MathJax:focus, body :focus .MathJax {display: inline-table}
.MathJax.MathJax_FullWidth {text-align: center; display: table-cell!important; width: 10000em!important}
.MathJax img, .MathJax nobr, .MathJax a {border: 0; padding: 0; margin: 0; max-width: none; max-height: none; min-width: 0; min-height: 0; vertical-align: 0; line-height: normal; text-decoration: none}
img.MathJax_strut {border: 0!important; padding: 0!important; margin: 0!important; vertical-align: 0!important}
.MathJax span {display: inline; position: static; border: 0; padding: 0; margin: 0; vertical-align: 0; line-height: normal; text-decoration: none; box-sizing: content-box}
.MathJax nobr {white-space: nowrap!important}
.MathJax img {display: inline!important; float: none!important}
.MathJax * {transition: none; -webkit-transition: none; -moz-transition: none; -ms-transition: none; -o-transition: none}
.MathJax_Processing {visibility: hidden; position: fixed; width: 0; height: 0; overflow: hidden}
.MathJax_Processed {display: none!important}
.MathJax_test {font-style: normal; font-weight: normal; font-size: 100%; font-size-adjust: none; text-indent: 0; text-transform: none; letter-spacing: normal; word-spacing: normal; overflow: hidden; height: 1px}
.MathJax_test.mjx-test-display {display: table!important}
.MathJax_test.mjx-test-inline {display: inline!important; margin-right: -1px}
.MathJax_test.mjx-test-default {display: block!important; clear: both}
.MathJax_ex_box {display: inline-block!important; position: absolute; overflow: hidden; min-height: 0; max-height: none; padding: 0; border: 0; margin: 0; width: 1px; height: 60ex}
.MathJax_em_box {display: inline-block!important; position: absolute; overflow: hidden; min-height: 0; max-height: none; padding: 0; border: 0; margin: 0; width: 1px; height: 60em}
.mjx-test-inline .MathJax_left_box {display: inline-block; width: 0; float: left}
.mjx-test-inline .MathJax_right_box {display: inline-block; width: 0; float: right}
.mjx-test-display .MathJax_right_box {display: table-cell!important; width: 10000em!important; min-width: 0; max-width: none; padding: 0; border: 0; margin: 0}
.MathJax .MathJax_HitBox {cursor: text; background: white; opacity: 0; filter: alpha(opacity=0)}
.MathJax .MathJax_HitBox * {filter: none; opacity: 1; background: transparent}
#MathJax_Tooltip * {filter: none; opacity: 1; background: transparent}
@font-face {font-family: MathJax_Main; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Main-bold; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Bold.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Bold.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Main-italic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Main-Italic.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Main-Italic.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Math-italic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Math-Italic.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Math-Italic.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Caligraphic; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Caligraphic-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Caligraphic-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size1; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size1-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size1-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size2; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size2-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size2-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size3; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size3-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size3-Regular.otf?V=2.7.5') format('opentype')}
@font-face {font-family: MathJax_Size4; src: url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/woff/MathJax_Size4-Regular.woff?V=2.7.5') format('woff'), url('https://colab.research.google.com/static/mathjax/fonts/HTML-CSS/TeX/otf/MathJax_Size4-Regular.otf?V=2.7.5') format('opentype')}
.MathJax .noError {vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
</style><script async="async" type="text/javascript" src="./DataMining_Project3_HSM.ipynb - Colab_files/markdown.js.download"></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/api.js.download" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/api(1).js.download" nonce=""></script><style type="text/css" media="screen" class="monaco-colors">.codicon-add:before { content: '\ea60'; }
.codicon-plus:before { content: '\ea60'; }
.codicon-gist-new:before { content: '\ea60'; }
.codicon-repo-create:before { content: '\ea60'; }
.codicon-lightbulb:before { content: '\ea61'; }
.codicon-light-bulb:before { content: '\ea61'; }
.codicon-repo:before { content: '\ea62'; }
.codicon-repo-delete:before { content: '\ea62'; }
.codicon-gist-fork:before { content: '\ea63'; }
.codicon-repo-forked:before { content: '\ea63'; }
.codicon-git-pull-request:before { content: '\ea64'; }
.codicon-git-pull-request-abandoned:before { content: '\ea64'; }
.codicon-record-keys:before { content: '\ea65'; }
.codicon-keyboard:before { content: '\ea65'; }
.codicon-tag:before { content: '\ea66'; }
.codicon-tag-add:before { content: '\ea66'; }
.codicon-tag-remove:before { content: '\ea66'; }
.codicon-person:before { content: '\ea67'; }
.codicon-person-follow:before { content: '\ea67'; }
.codicon-person-outline:before { content: '\ea67'; }
.codicon-person-filled:before { content: '\ea67'; }
.codicon-git-branch:before { content: '\ea68'; }
.codicon-git-branch-create:before { content: '\ea68'; }
.codicon-git-branch-delete:before { content: '\ea68'; }
.codicon-source-control:before { content: '\ea68'; }
.codicon-mirror:before { content: '\ea69'; }
.codicon-mirror-public:before { content: '\ea69'; }
.codicon-star:before { content: '\ea6a'; }
.codicon-star-add:before { content: '\ea6a'; }
.codicon-star-delete:before { content: '\ea6a'; }
.codicon-star-empty:before { content: '\ea6a'; }
.codicon-comment:before { content: '\ea6b'; }
.codicon-comment-add:before { content: '\ea6b'; }
.codicon-alert:before { content: '\ea6c'; }
.codicon-warning:before { content: '\ea6c'; }
.codicon-search:before { content: '\ea6d'; }
.codicon-search-save:before { content: '\ea6d'; }
.codicon-log-out:before { content: '\ea6e'; }
.codicon-sign-out:before { content: '\ea6e'; }
.codicon-log-in:before { content: '\ea6f'; }
.codicon-sign-in:before { content: '\ea6f'; }
.codicon-eye:before { content: '\ea70'; }
.codicon-eye-unwatch:before { content: '\ea70'; }
.codicon-eye-watch:before { content: '\ea70'; }
.codicon-circle-filled:before { content: '\ea71'; }
.codicon-primitive-dot:before { content: '\ea71'; }
.codicon-close-dirty:before { content: '\ea71'; }
.codicon-debug-breakpoint:before { content: '\ea71'; }
.codicon-debug-breakpoint-disabled:before { content: '\ea71'; }
.codicon-debug-hint:before { content: '\ea71'; }
.codicon-primitive-square:before { content: '\ea72'; }
.codicon-edit:before { content: '\ea73'; }
.codicon-pencil:before { content: '\ea73'; }
.codicon-info:before { content: '\ea74'; }
.codicon-issue-opened:before { content: '\ea74'; }
.codicon-gist-private:before { content: '\ea75'; }
.codicon-git-fork-private:before { content: '\ea75'; }
.codicon-lock:before { content: '\ea75'; }
.codicon-mirror-private:before { content: '\ea75'; }
.codicon-close:before { content: '\ea76'; }
.codicon-remove-close:before { content: '\ea76'; }
.codicon-x:before { content: '\ea76'; }
.codicon-repo-sync:before { content: '\ea77'; }
.codicon-sync:before { content: '\ea77'; }
.codicon-clone:before { content: '\ea78'; }
.codicon-desktop-download:before { content: '\ea78'; }
.codicon-beaker:before { content: '\ea79'; }
.codicon-microscope:before { content: '\ea79'; }
.codicon-vm:before { content: '\ea7a'; }
.codicon-device-desktop:before { content: '\ea7a'; }
.codicon-file:before { content: '\ea7b'; }
.codicon-file-text:before { content: '\ea7b'; }
.codicon-more:before { content: '\ea7c'; }
.codicon-ellipsis:before { content: '\ea7c'; }
.codicon-kebab-horizontal:before { content: '\ea7c'; }
.codicon-mail-reply:before { content: '\ea7d'; }
.codicon-reply:before { content: '\ea7d'; }
.codicon-organization:before { content: '\ea7e'; }
.codicon-organization-filled:before { content: '\ea7e'; }
.codicon-organization-outline:before { content: '\ea7e'; }
.codicon-new-file:before { content: '\ea7f'; }
.codicon-file-add:before { content: '\ea7f'; }
.codicon-new-folder:before { content: '\ea80'; }
.codicon-file-directory-create:before { content: '\ea80'; }
.codicon-trash:before { content: '\ea81'; }
.codicon-trashcan:before { content: '\ea81'; }
.codicon-history:before { content: '\ea82'; }
.codicon-clock:before { content: '\ea82'; }
.codicon-folder:before { content: '\ea83'; }
.codicon-file-directory:before { content: '\ea83'; }
.codicon-symbol-folder:before { content: '\ea83'; }
.codicon-logo-github:before { content: '\ea84'; }
.codicon-mark-github:before { content: '\ea84'; }
.codicon-github:before { content: '\ea84'; }
.codicon-terminal:before { content: '\ea85'; }
.codicon-console:before { content: '\ea85'; }
.codicon-repl:before { content: '\ea85'; }
.codicon-zap:before { content: '\ea86'; }
.codicon-symbol-event:before { content: '\ea86'; }
.codicon-error:before { content: '\ea87'; }
.codicon-stop:before { content: '\ea87'; }
.codicon-variable:before { content: '\ea88'; }
.codicon-symbol-variable:before { content: '\ea88'; }
.codicon-array:before { content: '\ea8a'; }
.codicon-symbol-array:before { content: '\ea8a'; }
.codicon-symbol-module:before { content: '\ea8b'; }
.codicon-symbol-package:before { content: '\ea8b'; }
.codicon-symbol-namespace:before { content: '\ea8b'; }
.codicon-symbol-object:before { content: '\ea8b'; }
.codicon-symbol-method:before { content: '\ea8c'; }
.codicon-symbol-function:before { content: '\ea8c'; }
.codicon-symbol-constructor:before { content: '\ea8c'; }
.codicon-symbol-boolean:before { content: '\ea8f'; }
.codicon-symbol-null:before { content: '\ea8f'; }
.codicon-symbol-numeric:before { content: '\ea90'; }
.codicon-symbol-number:before { content: '\ea90'; }
.codicon-symbol-structure:before { content: '\ea91'; }
.codicon-symbol-struct:before { content: '\ea91'; }
.codicon-symbol-parameter:before { content: '\ea92'; }
.codicon-symbol-type-parameter:before { content: '\ea92'; }
.codicon-symbol-key:before { content: '\ea93'; }
.codicon-symbol-text:before { content: '\ea93'; }
.codicon-symbol-reference:before { content: '\ea94'; }
.codicon-go-to-file:before { content: '\ea94'; }
.codicon-symbol-enum:before { content: '\ea95'; }
.codicon-symbol-value:before { content: '\ea95'; }
.codicon-symbol-ruler:before { content: '\ea96'; }
.codicon-symbol-unit:before { content: '\ea96'; }
.codicon-activate-breakpoints:before { content: '\ea97'; }
.codicon-archive:before { content: '\ea98'; }
.codicon-arrow-both:before { content: '\ea99'; }
.codicon-arrow-down:before { content: '\ea9a'; }
.codicon-arrow-left:before { content: '\ea9b'; }
.codicon-arrow-right:before { content: '\ea9c'; }
.codicon-arrow-small-down:before { content: '\ea9d'; }
.codicon-arrow-small-left:before { content: '\ea9e'; }
.codicon-arrow-small-right:before { content: '\ea9f'; }
.codicon-arrow-small-up:before { content: '\eaa0'; }
.codicon-arrow-up:before { content: '\eaa1'; }
.codicon-bell:before { content: '\eaa2'; }
.codicon-bold:before { content: '\eaa3'; }
.codicon-book:before { content: '\eaa4'; }
.codicon-bookmark:before { content: '\eaa5'; }
.codicon-debug-breakpoint-conditional-unverified:before { content: '\eaa6'; }
.codicon-debug-breakpoint-conditional:before { content: '\eaa7'; }
.codicon-debug-breakpoint-conditional-disabled:before { content: '\eaa7'; }
.codicon-debug-breakpoint-data-unverified:before { content: '\eaa8'; }
.codicon-debug-breakpoint-data:before { content: '\eaa9'; }
.codicon-debug-breakpoint-data-disabled:before { content: '\eaa9'; }
.codicon-debug-breakpoint-log-unverified:before { content: '\eaaa'; }
.codicon-debug-breakpoint-log:before { content: '\eaab'; }
.codicon-debug-breakpoint-log-disabled:before { content: '\eaab'; }
.codicon-briefcase:before { content: '\eaac'; }
.codicon-broadcast:before { content: '\eaad'; }
.codicon-browser:before { content: '\eaae'; }
.codicon-bug:before { content: '\eaaf'; }
.codicon-calendar:before { content: '\eab0'; }
.codicon-case-sensitive:before { content: '\eab1'; }
.codicon-check:before { content: '\eab2'; }
.codicon-checklist:before { content: '\eab3'; }
.codicon-chevron-down:before { content: '\eab4'; }
.codicon-drop-down-button:before { content: '\eab4'; }
.codicon-chevron-left:before { content: '\eab5'; }
.codicon-chevron-right:before { content: '\eab6'; }
.codicon-chevron-up:before { content: '\eab7'; }
.codicon-chrome-close:before { content: '\eab8'; }
.codicon-chrome-maximize:before { content: '\eab9'; }
.codicon-chrome-minimize:before { content: '\eaba'; }
.codicon-chrome-restore:before { content: '\eabb'; }
.codicon-circle:before { content: '\eabc'; }
.codicon-circle-outline:before { content: '\eabc'; }
.codicon-debug-breakpoint-unverified:before { content: '\eabc'; }
.codicon-circle-slash:before { content: '\eabd'; }
.codicon-circuit-board:before { content: '\eabe'; }
.codicon-clear-all:before { content: '\eabf'; }
.codicon-clippy:before { content: '\eac0'; }
.codicon-close-all:before { content: '\eac1'; }
.codicon-cloud-download:before { content: '\eac2'; }
.codicon-cloud-upload:before { content: '\eac3'; }
.codicon-code:before { content: '\eac4'; }
.codicon-collapse-all:before { content: '\eac5'; }
.codicon-color-mode:before { content: '\eac6'; }
.codicon-comment-discussion:before { content: '\eac7'; }
.codicon-compare-changes:before { content: '\eafd'; }
.codicon-credit-card:before { content: '\eac9'; }
.codicon-dash:before { content: '\eacc'; }
.codicon-dashboard:before { content: '\eacd'; }
.codicon-database:before { content: '\eace'; }
.codicon-debug-continue:before { content: '\eacf'; }
.codicon-debug-disconnect:before { content: '\ead0'; }
.codicon-debug-pause:before { content: '\ead1'; }
.codicon-debug-restart:before { content: '\ead2'; }
.codicon-debug-start:before { content: '\ead3'; }
.codicon-debug-step-into:before { content: '\ead4'; }
.codicon-debug-step-out:before { content: '\ead5'; }
.codicon-debug-step-over:before { content: '\ead6'; }
.codicon-debug-stop:before { content: '\ead7'; }
.codicon-debug:before { content: '\ead8'; }
.codicon-device-camera-video:before { content: '\ead9'; }
.codicon-device-camera:before { content: '\eada'; }
.codicon-device-mobile:before { content: '\eadb'; }
.codicon-diff-added:before { content: '\eadc'; }
.codicon-diff-ignored:before { content: '\eadd'; }
.codicon-diff-modified:before { content: '\eade'; }
.codicon-diff-removed:before { content: '\eadf'; }
.codicon-diff-renamed:before { content: '\eae0'; }
.codicon-diff:before { content: '\eae1'; }
.codicon-discard:before { content: '\eae2'; }
.codicon-editor-layout:before { content: '\eae3'; }
.codicon-empty-window:before { content: '\eae4'; }
.codicon-exclude:before { content: '\eae5'; }
.codicon-extensions:before { content: '\eae6'; }
.codicon-eye-closed:before { content: '\eae7'; }
.codicon-file-binary:before { content: '\eae8'; }
.codicon-file-code:before { content: '\eae9'; }
.codicon-file-media:before { content: '\eaea'; }
.codicon-file-pdf:before { content: '\eaeb'; }
.codicon-file-submodule:before { content: '\eaec'; }
.codicon-file-symlink-directory:before { content: '\eaed'; }
.codicon-file-symlink-file:before { content: '\eaee'; }
.codicon-file-zip:before { content: '\eaef'; }
.codicon-files:before { content: '\eaf0'; }
.codicon-filter:before { content: '\eaf1'; }
.codicon-flame:before { content: '\eaf2'; }
.codicon-fold-down:before { content: '\eaf3'; }
.codicon-fold-up:before { content: '\eaf4'; }
.codicon-fold:before { content: '\eaf5'; }
.codicon-folder-active:before { content: '\eaf6'; }
.codicon-folder-opened:before { content: '\eaf7'; }
.codicon-gear:before { content: '\eaf8'; }
.codicon-gift:before { content: '\eaf9'; }
.codicon-gist-secret:before { content: '\eafa'; }
.codicon-gist:before { content: '\eafb'; }
.codicon-git-commit:before { content: '\eafc'; }
.codicon-git-compare:before { content: '\eafd'; }
.codicon-git-merge:before { content: '\eafe'; }
.codicon-github-action:before { content: '\eaff'; }
.codicon-github-alt:before { content: '\eb00'; }
.codicon-globe:before { content: '\eb01'; }
.codicon-grabber:before { content: '\eb02'; }
.codicon-graph:before { content: '\eb03'; }
.codicon-gripper:before { content: '\eb04'; }
.codicon-heart:before { content: '\eb05'; }
.codicon-home:before { content: '\eb06'; }
.codicon-horizontal-rule:before { content: '\eb07'; }
.codicon-hubot:before { content: '\eb08'; }
.codicon-inbox:before { content: '\eb09'; }
.codicon-issue-closed:before { content: '\eba4'; }
.codicon-issue-reopened:before { content: '\eb0b'; }
.codicon-issues:before { content: '\eb0c'; }
.codicon-italic:before { content: '\eb0d'; }
.codicon-jersey:before { content: '\eb0e'; }
.codicon-json:before { content: '\eb0f'; }
.codicon-bracket:before { content: '\eb0f'; }
.codicon-kebab-vertical:before { content: '\eb10'; }
.codicon-key:before { content: '\eb11'; }
.codicon-law:before { content: '\eb12'; }
.codicon-lightbulb-autofix:before { content: '\eb13'; }
.codicon-link-external:before { content: '\eb14'; }
.codicon-link:before { content: '\eb15'; }
.codicon-list-ordered:before { content: '\eb16'; }
.codicon-list-unordered:before { content: '\eb17'; }
.codicon-live-share:before { content: '\eb18'; }
.codicon-loading:before { content: '\eb19'; }
.codicon-location:before { content: '\eb1a'; }
.codicon-mail-read:before { content: '\eb1b'; }
.codicon-mail:before { content: '\eb1c'; }
.codicon-markdown:before { content: '\eb1d'; }
.codicon-megaphone:before { content: '\eb1e'; }
.codicon-mention:before { content: '\eb1f'; }
.codicon-milestone:before { content: '\eb20'; }
.codicon-mortar-board:before { content: '\eb21'; }
.codicon-move:before { content: '\eb22'; }
.codicon-multiple-windows:before { content: '\eb23'; }
.codicon-mute:before { content: '\eb24'; }
.codicon-no-newline:before { content: '\eb25'; }
.codicon-note:before { content: '\eb26'; }
.codicon-octoface:before { content: '\eb27'; }
.codicon-open-preview:before { content: '\eb28'; }
.codicon-package:before { content: '\eb29'; }
.codicon-paintcan:before { content: '\eb2a'; }
.codicon-pin:before { content: '\eb2b'; }
.codicon-play:before { content: '\eb2c'; }
.codicon-run:before { content: '\eb2c'; }
.codicon-plug:before { content: '\eb2d'; }
.codicon-preserve-case:before { content: '\eb2e'; }
.codicon-preview:before { content: '\eb2f'; }
.codicon-project:before { content: '\eb30'; }
.codicon-pulse:before { content: '\eb31'; }
.codicon-question:before { content: '\eb32'; }
.codicon-quote:before { content: '\eb33'; }
.codicon-radio-tower:before { content: '\eb34'; }
.codicon-reactions:before { content: '\eb35'; }
.codicon-references:before { content: '\eb36'; }
.codicon-refresh:before { content: '\eb37'; }
.codicon-regex:before { content: '\eb38'; }
.codicon-remote-explorer:before { content: '\eb39'; }
.codicon-remote:before { content: '\eb3a'; }
.codicon-remove:before { content: '\eb3b'; }
.codicon-replace-all:before { content: '\eb3c'; }
.codicon-replace:before { content: '\eb3d'; }
.codicon-repo-clone:before { content: '\eb3e'; }
.codicon-repo-force-push:before { content: '\eb3f'; }
.codicon-repo-pull:before { content: '\eb40'; }
.codicon-repo-push:before { content: '\eb41'; }
.codicon-report:before { content: '\eb42'; }
.codicon-request-changes:before { content: '\eb43'; }
.codicon-rocket:before { content: '\eb44'; }
.codicon-root-folder-opened:before { content: '\eb45'; }
.codicon-root-folder:before { content: '\eb46'; }
.codicon-rss:before { content: '\eb47'; }
.codicon-ruby:before { content: '\eb48'; }
.codicon-save-all:before { content: '\eb49'; }
.codicon-save-as:before { content: '\eb4a'; }
.codicon-save:before { content: '\eb4b'; }
.codicon-screen-full:before { content: '\eb4c'; }
.codicon-screen-normal:before { content: '\eb4d'; }
.codicon-search-stop:before { content: '\eb4e'; }
.codicon-server:before { content: '\eb50'; }
.codicon-settings-gear:before { content: '\eb51'; }
.codicon-settings:before { content: '\eb52'; }
.codicon-shield:before { content: '\eb53'; }
.codicon-smiley:before { content: '\eb54'; }
.codicon-sort-precedence:before { content: '\eb55'; }
.codicon-split-horizontal:before { content: '\eb56'; }
.codicon-split-vertical:before { content: '\eb57'; }
.codicon-squirrel:before { content: '\eb58'; }
.codicon-star-full:before { content: '\eb59'; }
.codicon-star-half:before { content: '\eb5a'; }
.codicon-symbol-class:before { content: '\eb5b'; }
.codicon-symbol-color:before { content: '\eb5c'; }
.codicon-symbol-customcolor:before { content: '\eb5c'; }
.codicon-symbol-constant:before { content: '\eb5d'; }
.codicon-symbol-enum-member:before { content: '\eb5e'; }
.codicon-symbol-field:before { content: '\eb5f'; }
.codicon-symbol-file:before { content: '\eb60'; }
.codicon-symbol-interface:before { content: '\eb61'; }
.codicon-symbol-keyword:before { content: '\eb62'; }
.codicon-symbol-misc:before { content: '\eb63'; }
.codicon-symbol-operator:before { content: '\eb64'; }
.codicon-symbol-property:before { content: '\eb65'; }
.codicon-wrench:before { content: '\eb65'; }
.codicon-wrench-subaction:before { content: '\eb65'; }
.codicon-symbol-snippet:before { content: '\eb66'; }
.codicon-tasklist:before { content: '\eb67'; }
.codicon-telescope:before { content: '\eb68'; }
.codicon-text-size:before { content: '\eb69'; }
.codicon-three-bars:before { content: '\eb6a'; }
.codicon-thumbsdown:before { content: '\eb6b'; }
.codicon-thumbsup:before { content: '\eb6c'; }
.codicon-tools:before { content: '\eb6d'; }
.codicon-triangle-down:before { content: '\eb6e'; }
.codicon-triangle-left:before { content: '\eb6f'; }
.codicon-triangle-right:before { content: '\eb70'; }
.codicon-triangle-up:before { content: '\eb71'; }
.codicon-twitter:before { content: '\eb72'; }
.codicon-unfold:before { content: '\eb73'; }
.codicon-unlock:before { content: '\eb74'; }
.codicon-unmute:before { content: '\eb75'; }
.codicon-unverified:before { content: '\eb76'; }
.codicon-verified:before { content: '\eb77'; }
.codicon-versions:before { content: '\eb78'; }
.codicon-vm-active:before { content: '\eb79'; }
.codicon-vm-outline:before { content: '\eb7a'; }
.codicon-vm-running:before { content: '\eb7b'; }
.codicon-watch:before { content: '\eb7c'; }
.codicon-whitespace:before { content: '\eb7d'; }
.codicon-whole-word:before { content: '\eb7e'; }
.codicon-window:before { content: '\eb7f'; }
.codicon-word-wrap:before { content: '\eb80'; }
.codicon-zoom-in:before { content: '\eb81'; }
.codicon-zoom-out:before { content: '\eb82'; }
.codicon-list-filter:before { content: '\eb83'; }
.codicon-list-flat:before { content: '\eb84'; }
.codicon-list-selection:before { content: '\eb85'; }
.codicon-selection:before { content: '\eb85'; }
.codicon-list-tree:before { content: '\eb86'; }
.codicon-debug-breakpoint-function-unverified:before { content: '\eb87'; }
.codicon-debug-breakpoint-function:before { content: '\eb88'; }
.codicon-debug-breakpoint-function-disabled:before { content: '\eb88'; }
.codicon-debug-stackframe-active:before { content: '\eb89'; }
.codicon-circle-small-filled:before { content: '\eb8a'; }
.codicon-debug-stackframe-dot:before { content: '\eb8a'; }
.codicon-debug-stackframe:before { content: '\eb8b'; }
.codicon-debug-stackframe-focused:before { content: '\eb8b'; }
.codicon-debug-breakpoint-unsupported:before { content: '\eb8c'; }
.codicon-symbol-string:before { content: '\eb8d'; }
.codicon-debug-reverse-continue:before { content: '\eb8e'; }
.codicon-debug-step-back:before { content: '\eb8f'; }
.codicon-debug-restart-frame:before { content: '\eb90'; }
.codicon-call-incoming:before { content: '\eb92'; }
.codicon-call-outgoing:before { content: '\eb93'; }
.codicon-menu:before { content: '\eb94'; }
.codicon-expand-all:before { content: '\eb95'; }
.codicon-feedback:before { content: '\eb96'; }
.codicon-group-by-ref-type:before { content: '\eb97'; }
.codicon-ungroup-by-ref-type:before { content: '\eb98'; }
.codicon-account:before { content: '\eb99'; }
.codicon-bell-dot:before { content: '\eb9a'; }
.codicon-debug-console:before { content: '\eb9b'; }
.codicon-library:before { content: '\eb9c'; }
.codicon-output:before { content: '\eb9d'; }
.codicon-run-all:before { content: '\eb9e'; }
.codicon-sync-ignored:before { content: '\eb9f'; }
.codicon-pinned:before { content: '\eba0'; }
.codicon-github-inverted:before { content: '\eba1'; }
.codicon-debug-alt:before { content: '\eb91'; }
.codicon-server-process:before { content: '\eba2'; }
.codicon-server-environment:before { content: '\eba3'; }
.codicon-pass:before { content: '\eba4'; }
.codicon-stop-circle:before { content: '\eba5'; }
.codicon-play-circle:before { content: '\eba6'; }
.codicon-record:before { content: '\eba7'; }
.codicon-debug-alt-small:before { content: '\eba8'; }
.codicon-vm-connect:before { content: '\eba9'; }
.codicon-cloud:before { content: '\ebaa'; }
.codicon-merge:before { content: '\ebab'; }
.codicon-export:before { content: '\ebac'; }
.codicon-graph-left:before { content: '\ebad'; }
.codicon-magnet:before { content: '\ebae'; }
.codicon-notebook:before { content: '\ebaf'; }
.codicon-redo:before { content: '\ebb0'; }
.codicon-check-all:before { content: '\ebb1'; }
.codicon-pinned-dirty:before { content: '\ebb2'; }
.codicon-pass-filled:before { content: '\ebb3'; }
.codicon-circle-large-filled:before { content: '\ebb4'; }
.codicon-circle-large:before { content: '\ebb5'; }
.codicon-circle-large-outline:before { content: '\ebb5'; }
.codicon-combine:before { content: '\ebb6'; }
.codicon-gather:before { content: '\ebb6'; }
.codicon-table:before { content: '\ebb7'; }
.codicon-variable-group:before { content: '\ebb8'; }
.codicon-type-hierarchy:before { content: '\ebb9'; }
.codicon-type-hierarchy-sub:before { content: '\ebba'; }
.codicon-type-hierarchy-super:before { content: '\ebbb'; }
.codicon-git-pull-request-create:before { content: '\ebbc'; }
.codicon-run-above:before { content: '\ebbd'; }
.codicon-run-below:before { content: '\ebbe'; }
.codicon-notebook-template:before { content: '\ebbf'; }
.codicon-debug-rerun:before { content: '\ebc0'; }
.codicon-workspace-trusted:before { content: '\ebc1'; }
.codicon-workspace-untrusted:before { content: '\ebc2'; }
.codicon-workspace-unspecified:before { content: '\ebc3'; }
.codicon-terminal-cmd:before { content: '\ebc4'; }
.codicon-terminal-debian:before { content: '\ebc5'; }
.codicon-terminal-linux:before { content: '\ebc6'; }
.codicon-terminal-powershell:before { content: '\ebc7'; }
.codicon-terminal-tmux:before { content: '\ebc8'; }
.codicon-terminal-ubuntu:before { content: '\ebc9'; }
.codicon-terminal-bash:before { content: '\ebca'; }
.codicon-arrow-swap:before { content: '\ebcb'; }
.codicon-copy:before { content: '\ebcc'; }
.codicon-person-add:before { content: '\ebcd'; }
.codicon-filter-filled:before { content: '\ebce'; }
.codicon-wand:before { content: '\ebcf'; }
.codicon-debug-line-by-line:before { content: '\ebd0'; }
.codicon-inspect:before { content: '\ebd1'; }
.codicon-layers:before { content: '\ebd2'; }
.codicon-layers-dot:before { content: '\ebd3'; }
.codicon-layers-active:before { content: '\ebd4'; }
.codicon-compass:before { content: '\ebd5'; }
.codicon-compass-dot:before { content: '\ebd6'; }
.codicon-compass-active:before { content: '\ebd7'; }
.codicon-azure:before { content: '\ebd8'; }
.codicon-issue-draft:before { content: '\ebd9'; }
.codicon-git-pull-request-closed:before { content: '\ebda'; }
.codicon-git-pull-request-draft:before { content: '\ebdb'; }
.codicon-debug-all:before { content: '\ebdc'; }
.codicon-debug-coverage:before { content: '\ebdd'; }
.codicon-run-errors:before { content: '\ebde'; }
.codicon-folder-library:before { content: '\ebdf'; }
.codicon-debug-continue-small:before { content: '\ebe0'; }
.codicon-beaker-stop:before { content: '\ebe1'; }
.codicon-graph-line:before { content: '\ebe2'; }
.codicon-graph-scatter:before { content: '\ebe3'; }
.codicon-pie-chart:before { content: '\ebe4'; }
.codicon-bracket-dot:before { content: '\ebe5'; }
.codicon-bracket-error:before { content: '\ebe6'; }
.codicon-lock-small:before { content: '\ebe7'; }
.codicon-azure-devops:before { content: '\ebe8'; }
.codicon-verified-filled:before { content: '\ebe9'; }
.codicon-newline:before { content: '\ebea'; }
.codicon-layout:before { content: '\ebeb'; }
.codicon-layout-activitybar-left:before { content: '\ebec'; }
.codicon-layout-activitybar-right:before { content: '\ebed'; }
.codicon-layout-panel-left:before { content: '\ebee'; }
.codicon-layout-panel-center:before { content: '\ebef'; }
.codicon-layout-panel-justify:before { content: '\ebf0'; }
.codicon-layout-panel-right:before { content: '\ebf1'; }
.codicon-layout-panel:before { content: '\ebf2'; }
.codicon-layout-sidebar-left:before { content: '\ebf3'; }
.codicon-layout-sidebar-right:before { content: '\ebf4'; }
.codicon-layout-statusbar:before { content: '\ebf5'; }
.codicon-layout-menubar:before { content: '\ebf6'; }
.codicon-layout-centered:before { content: '\ebf7'; }
.codicon-layout-sidebar-right-off:before { content: '\ec00'; }
.codicon-layout-panel-off:before { content: '\ec01'; }
.codicon-layout-sidebar-left-off:before { content: '\ec02'; }
.codicon-target:before { content: '\ebf8'; }
.codicon-indent:before { content: '\ebf9'; }
.codicon-record-small:before { content: '\ebfa'; }
.codicon-error-small:before { content: '\ebfb'; }
.codicon-arrow-circle-down:before { content: '\ebfc'; }
.codicon-arrow-circle-left:before { content: '\ebfd'; }
.codicon-arrow-circle-right:before { content: '\ebfe'; }
.codicon-arrow-circle-up:before { content: '\ebff'; }
.codicon-heart-filled:before { content: '\ec04'; }
.codicon-map:before { content: '\ec05'; }
.codicon-map-filled:before { content: '\ec06'; }
.codicon-circle-small:before { content: '\ec07'; }
.codicon-bell-slash:before { content: '\ec08'; }
.codicon-bell-slash-dot:before { content: '\ec09'; }
.codicon-comment-unresolved:before { content: '\ec0a'; }
.codicon-git-pull-request-go-to-changes:before { content: '\ec0b'; }
.codicon-git-pull-request-new-changes:before { content: '\ec0c'; }
.codicon-search-fuzzy:before { content: '\ec0d'; }
.codicon-comment-draft:before { content: '\ec0e'; }
.codicon-send:before { content: '\ec0f'; }
.codicon-sparkle:before { content: '\ec10'; }
.codicon-insert:before { content: '\ec11'; }
.codicon-dialog-error:before { content: '\ea87'; }
.codicon-dialog-warning:before { content: '\ea6c'; }
.codicon-dialog-info:before { content: '\ea74'; }
.codicon-dialog-close:before { content: '\ea76'; }
.codicon-tree-item-expanded:before { content: '\eab4'; }
.codicon-tree-filter-on-type-on:before { content: '\eb83'; }
.codicon-tree-filter-on-type-off:before { content: '\eb85'; }
.codicon-tree-filter-clear:before { content: '\ea76'; }
.codicon-tree-item-loading:before { content: '\eb19'; }
.codicon-menu-selection:before { content: '\eab2'; }
.codicon-menu-submenu:before { content: '\eab6'; }
.codicon-menubar-more:before { content: '\ea7c'; }
.codicon-scrollbar-button-left:before { content: '\eb6f'; }
.codicon-scrollbar-button-right:before { content: '\eb70'; }
.codicon-scrollbar-button-up:before { content: '\eb71'; }
.codicon-scrollbar-button-down:before { content: '\eb6e'; }
.codicon-toolbar-more:before { content: '\ea7c'; }
.codicon-quick-input-back:before { content: '\ea9b'; }
.codicon-widget-close:before { content: '\ea76'; }
.codicon-goto-previous-location:before { content: '\eaa1'; }
.codicon-goto-next-location:before { content: '\ea9a'; }
.codicon-diff-review-insert:before { content: '\ea60'; }
.codicon-diff-review-remove:before { content: '\eb3b'; }
.codicon-diff-review-close:before { content: '\ea76'; }
.codicon-parameter-hints-next:before { content: '\eab4'; }
.codicon-parameter-hints-previous:before { content: '\eab7'; }
.codicon-suggest-more-info:before { content: '\eab6'; }
.codicon-inline-suggestion-hints-next:before { content: '\eab6'; }
.codicon-inline-suggestion-hints-previous:before { content: '\eab5'; }
.codicon-diff-insert:before { content: '\ea60'; }
.codicon-diff-remove:before { content: '\eb3b'; }
.codicon-find-selection:before { content: '\eb85'; }
.codicon-find-collapsed:before { content: '\eab6'; }
.codicon-find-expanded:before { content: '\eab4'; }
.codicon-find-replace:before { content: '\eb3d'; }
.codicon-find-replace-all:before { content: '\eb3c'; }
.codicon-find-previous-match:before { content: '\eaa1'; }
.codicon-find-next-match:before { content: '\ea9a'; }
.codicon-folding-expanded:before { content: '\eab4'; }
.codicon-folding-collapsed:before { content: '\eab6'; }
.codicon-folding-manual-collapsed:before { content: '\eab6'; }
.codicon-folding-manual-expanded:before { content: '\eab4'; }
.codicon-marker-navigation-next:before { content: '\ea9a'; }
.codicon-marker-navigation-previous:before { content: '\eaa1'; }
.codicon-extensions-warning-message:before { content: '\ea6c'; }
.monaco-editor .inputarea.ime-input { background-color: #f7f7f7; }
.monaco-editor .view-overlays .current-line { border: 2px solid #eeeeee; }
.monaco-editor .margin-view-overlays .current-line-margin { border: 2px solid #eeeeee; }
.monaco-editor .bracket-indent-guide.lvl-0 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-1 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-2 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-3 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-4 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-5 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-6 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-7 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-8 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-9 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-10 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-11 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-12 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-13 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-14 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-15 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-16 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-17 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-18 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-19 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-20 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-21 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-22 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-23 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-24 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-25 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-26 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .bracket-indent-guide.lvl-27 { --guide-color: rgba(4, 49, 250, 0.3); --guide-color-active: #0431fa; }
.monaco-editor .bracket-indent-guide.lvl-28 { --guide-color: rgba(49, 147, 49, 0.3); --guide-color-active: #319331; }
.monaco-editor .bracket-indent-guide.lvl-29 { --guide-color: rgba(123, 56, 20, 0.3); --guide-color-active: #7b3814; }
.monaco-editor .vertical { box-shadow: 1px 0 0 0 var(--guide-color) inset; }
.monaco-editor .horizontal-top { border-top: 1px solid var(--guide-color); }
.monaco-editor .horizontal-bottom { border-bottom: 1px solid var(--guide-color); }
.monaco-editor .vertical.indent-active { box-shadow: 1px 0 0 0 var(--guide-color-active) inset; }
.monaco-editor .horizontal-top.indent-active { border-top: 1px solid var(--guide-color-active); }
.monaco-editor .horizontal-bottom.indent-active { border-bottom: 1px solid var(--guide-color-active); }
.monaco-editor .line-numbers.dimmed-line-number { color: rgba(153, 153, 153, 0.4); }
.monaco-editor .cursors-layer .cursor { background-color: #000000; border-color: #000000; color: #ffffff; }
.monaco-editor .unexpected-closing-bracket { color: rgba(255, 18, 18, 0.8); }
.monaco-editor .bracket-highlighting-0 { color: #0431fa; }
.monaco-editor .bracket-highlighting-1 { color: #319331; }
.monaco-editor .bracket-highlighting-2 { color: #7b3814; }
.monaco-editor .bracket-highlighting-3 { color: #0431fa; }
.monaco-editor .bracket-highlighting-4 { color: #319331; }
.monaco-editor .bracket-highlighting-5 { color: #7b3814; }
.monaco-editor .bracket-highlighting-6 { color: #0431fa; }
.monaco-editor .bracket-highlighting-7 { color: #319331; }
.monaco-editor .bracket-highlighting-8 { color: #7b3814; }
.monaco-editor .bracket-highlighting-9 { color: #0431fa; }
.monaco-editor .bracket-highlighting-10 { color: #319331; }
.monaco-editor .bracket-highlighting-11 { color: #7b3814; }
.monaco-editor .bracket-highlighting-12 { color: #0431fa; }
.monaco-editor .bracket-highlighting-13 { color: #319331; }
.monaco-editor .bracket-highlighting-14 { color: #7b3814; }
.monaco-editor .bracket-highlighting-15 { color: #0431fa; }
.monaco-editor .bracket-highlighting-16 { color: #319331; }
.monaco-editor .bracket-highlighting-17 { color: #7b3814; }
.monaco-editor .bracket-highlighting-18 { color: #0431fa; }
.monaco-editor .bracket-highlighting-19 { color: #319331; }
.monaco-editor .bracket-highlighting-20 { color: #7b3814; }
.monaco-editor .bracket-highlighting-21 { color: #0431fa; }
.monaco-editor .bracket-highlighting-22 { color: #319331; }
.monaco-editor .bracket-highlighting-23 { color: #7b3814; }
.monaco-editor .bracket-highlighting-24 { color: #0431fa; }
.monaco-editor .bracket-highlighting-25 { color: #319331; }
.monaco-editor .bracket-highlighting-26 { color: #7b3814; }
.monaco-editor .bracket-highlighting-27 { color: #0431fa; }
.monaco-editor .bracket-highlighting-28 { color: #319331; }
.monaco-editor .bracket-highlighting-29 { color: #7b3814; }
.monaco-editor .squiggly-error { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%23e51400'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-warning { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%23bf8803'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-info { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D'http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg'%20viewBox%3D'0%200%206%203'%20enable-background%3D'new%200%200%206%203'%20height%3D'3'%20width%3D'6'%3E%3Cg%20fill%3D'%231a85ff'%3E%3Cpolygon%20points%3D'5.5%2C0%202.5%2C3%201.1%2C3%204.1%2C0'%2F%3E%3Cpolygon%20points%3D'4%2C0%206%2C2%206%2C0.6%205.4%2C0'%2F%3E%3Cpolygon%20points%3D'0%2C2%201%2C3%202.4%2C3%200%2C0.6'%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") repeat-x bottom left; }
.monaco-editor .squiggly-hint { background: url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20height%3D%223%22%20width%3D%2212%22%3E%3Cg%20fill%3D%22%236c6c6c%22%3E%3Ccircle%20cx%3D%221%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3Ccircle%20cx%3D%225%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3Ccircle%20cx%3D%229%22%20cy%3D%221%22%20r%3D%221%22%2F%3E%3C%2Fg%3E%3C%2Fsvg%3E") no-repeat bottom left; }
.monaco-editor.showUnused .squiggly-inline-unnecessary { opacity: 0.467; }
.monaco-editor .selectionHighlight { background-color: rgba(173, 214, 255, 0.15); }

	.monaco-editor .diagonal-fill {
		background-image: linear-gradient(
			-45deg,
			rgba(34, 34, 34, 0.2) 12.5%,
			#0000 12.5%, #0000 50%,
			rgba(34, 34, 34, 0.2) 50%, rgba(34, 34, 34, 0.2) 62.5%,
			#0000 62.5%, #0000 100%
		);
		background-size: 8px 8px;
	}
	
.monaco-editor .findMatch { background-color: rgba(234, 92, 0, 0.33); }
.monaco-editor .currentFindMatch { background-color: #a8ac94; }
.monaco-editor .findScope { background-color: rgba(180, 180, 180, 0.3); }
.monaco-editor .find-widget { background-color: #f3f3f3; }
.monaco-editor .find-widget { box-shadow: 0 0 8px 2px rgba(0, 0, 0, 0.16); }
.monaco-editor .find-widget { color: #616161; }
.monaco-editor .find-widget.no-results .matchesCount { color: #a1260d; }
.monaco-editor .find-widget .monaco-sash { background-color: #c8c8c8; }

		.monaco-editor .find-widget .button:not(.disabled):hover,
		.monaco-editor .find-widget .codicon-find-selection:hover {
			background-color: rgba(184, 184, 184, 0.31) !important;
		}
	
.monaco-editor .find-widget .monaco-inputbox.synthetic-focus { outline-color: #0090f1; }
.monaco-editor .monaco-hover .hover-row:not(:first-child):not(:empty) { border-top: 1px solid rgba(200, 200, 200, 0.5); }
.monaco-editor .monaco-hover hr { border-top: 1px solid rgba(200, 200, 200, 0.5); }
.monaco-editor .monaco-hover hr { border-bottom: 0px solid rgba(200, 200, 200, 0.5); }
.monaco-editor { --vscode-foreground: #616161;
--vscode-disabledForeground: rgba(97, 97, 97, 0.5);
--vscode-errorForeground: #a1260d;
--vscode-descriptionForeground: #717171;
--vscode-icon-foreground: #424242;
--vscode-focusBorder: #0090f1;
--vscode-textSeparator-foreground: rgba(0, 0, 0, 0.18);
--vscode-textLink-foreground: #006ab1;
--vscode-textLink-activeForeground: #006ab1;
--vscode-textPreformat-foreground: #a31515;
--vscode-textBlockQuote-background: rgba(127, 127, 127, 0.1);
--vscode-textBlockQuote-border: rgba(0, 122, 204, 0.5);
--vscode-textCodeBlock-background: rgba(220, 220, 220, 0.4);
--vscode-widget-shadow: rgba(0, 0, 0, 0.16);
--vscode-input-background: #ffffff;
--vscode-input-foreground: #616161;
--vscode-inputOption-activeBorder: #007acc;
--vscode-inputOption-hoverBackground: rgba(184, 184, 184, 0.31);
--vscode-inputOption-activeBackground: rgba(0, 144, 241, 0.2);
--vscode-inputOption-activeForeground: #000000;
--vscode-input-placeholderForeground: rgba(97, 97, 97, 0.5);
--vscode-inputValidation-infoBackground: #d6ecf2;
--vscode-inputValidation-infoBorder: #007acc;
--vscode-inputValidation-warningBackground: #f6f5d2;
--vscode-inputValidation-warningBorder: #b89500;
--vscode-inputValidation-errorBackground: #f2dede;
--vscode-inputValidation-errorBorder: #be1100;
--vscode-dropdown-background: #ffffff;
--vscode-dropdown-foreground: #616161;
--vscode-dropdown-border: #cecece;
--vscode-button-foreground: #ffffff;
--vscode-button-separator: rgba(255, 255, 255, 0.4);
--vscode-button-background: #007acc;
--vscode-button-hoverBackground: #0062a3;
--vscode-button-secondaryForeground: #ffffff;
--vscode-button-secondaryBackground: #5f6a79;
--vscode-button-secondaryHoverBackground: #4c5561;
--vscode-badge-background: #c4c4c4;
--vscode-badge-foreground: #333333;
--vscode-scrollbar-shadow: #dddddd;
--vscode-scrollbarSlider-background: rgba(100, 100, 100, 0.4);
--vscode-scrollbarSlider-hoverBackground: rgba(100, 100, 100, 0.7);
--vscode-scrollbarSlider-activeBackground: rgba(0, 0, 0, 0.6);
--vscode-progressBar-background: #0e70c0;
--vscode-editorError-foreground: #e51400;
--vscode-editorWarning-foreground: #bf8803;
--vscode-editorInfo-foreground: #1a85ff;
--vscode-editorHint-foreground: #6c6c6c;
--vscode-sash-hoverBorder: #0090f1;
--vscode-editor-background: #f7f7f7;
--vscode-editor-foreground: #000000;
--vscode-editorStickyScroll-background: #f7f7f7;
--vscode-editorStickyScrollHover-background: #f0f0f0;
--vscode-editorWidget-background: #f3f3f3;
--vscode-editorWidget-foreground: #616161;
--vscode-editorWidget-border: #c8c8c8;
--vscode-quickInput-background: #f3f3f3;
--vscode-quickInput-foreground: #616161;
--vscode-quickInputTitle-background: rgba(0, 0, 0, 0.06);
--vscode-pickerGroup-foreground: #0066bf;
--vscode-pickerGroup-border: #cccedb;
--vscode-keybindingLabel-background: rgba(221, 221, 221, 0.4);
--vscode-keybindingLabel-foreground: #555555;
--vscode-keybindingLabel-border: rgba(204, 204, 204, 0.4);
--vscode-keybindingLabel-bottomBorder: rgba(187, 187, 187, 0.4);
--vscode-editor-selectionBackground: #add6ff;
--vscode-editor-inactiveSelectionBackground: #e5ebf1;
--vscode-editor-selectionHighlightBackground: rgba(173, 214, 255, 0.3);
--vscode-editor-findMatchBackground: #a8ac94;
--vscode-editor-findMatchHighlightBackground: rgba(234, 92, 0, 0.33);
--vscode-editor-findRangeHighlightBackground: rgba(180, 180, 180, 0.3);
--vscode-searchEditor-findMatchBackground: rgba(234, 92, 0, 0.22);
--vscode-search-resultsInfoForeground: #616161;
--vscode-editor-hoverHighlightBackground: rgba(173, 214, 255, 0.15);
--vscode-editorHoverWidget-background: #f3f3f3;
--vscode-editorHoverWidget-foreground: #616161;
--vscode-editorHoverWidget-border: #c8c8c8;
--vscode-editorHoverWidget-statusBarBackground: #e7e7e7;
--vscode-editorLink-activeForeground: #0000ff;
--vscode-editorInlayHint-foreground: #616161;
--vscode-editorInlayHint-background: rgba(196, 196, 196, 0.3);
--vscode-editorInlayHint-typeForeground: #616161;
--vscode-editorInlayHint-typeBackground: rgba(196, 196, 196, 0.3);
--vscode-editorInlayHint-parameterForeground: #616161;
--vscode-editorInlayHint-parameterBackground: rgba(196, 196, 196, 0.3);
--vscode-editorLightBulb-foreground: #ddb100;
--vscode-editorLightBulbAutoFix-foreground: #007acc;
--vscode-diffEditor-insertedTextBackground: rgba(155, 185, 85, 0.09);
--vscode-diffEditor-removedTextBackground: rgba(255, 0, 0, 0.03);
--vscode-diffEditor-insertedLineBackground: rgba(155, 185, 85, 0.09);
--vscode-diffEditor-removedLineBackground: rgba(255, 0, 0, 0.03);
--vscode-diffEditor-diagonalFill: rgba(34, 34, 34, 0.2);
--vscode-diffEditor-unchangedRegionBackground: #e4e4e4;
--vscode-diffEditor-unchangedRegionForeground: #4d4c4c;
--vscode-diffEditor-unchangedCodeBackground: rgba(184, 184, 184, 0.16);
--vscode-list-focusOutline: #0090f1;
--vscode-list-activeSelectionBackground: #d6ebff;
--vscode-list-activeSelectionForeground: #000000;
--vscode-list-inactiveSelectionBackground: #e4e6f1;
--vscode-list-hoverBackground: #f0f0f0;
--vscode-list-dropBackground: #d6ebff;
--vscode-list-highlightForeground: #0066bf;
--vscode-list-focusHighlightForeground: #0066bf;
--vscode-list-invalidItemForeground: #b89500;
--vscode-list-errorForeground: #b01011;
--vscode-list-warningForeground: #855f00;
--vscode-listFilterWidget-background: #f3f3f3;
--vscode-listFilterWidget-outline: rgba(0, 0, 0, 0);
--vscode-listFilterWidget-noMatchesOutline: #be1100;
--vscode-listFilterWidget-shadow: rgba(0, 0, 0, 0.16);
--vscode-list-filterMatchBackground: rgba(234, 92, 0, 0.33);
--vscode-tree-indentGuidesStroke: #a9a9a9;
--vscode-tree-inactiveIndentGuidesStroke: rgba(169, 169, 169, 0.4);
--vscode-tree-tableColumnsBorder: rgba(97, 97, 97, 0.13);
--vscode-tree-tableOddRowsBackground: rgba(97, 97, 97, 0.04);
--vscode-list-deemphasizedForeground: #8e8e90;
--vscode-checkbox-background: #ffffff;
--vscode-checkbox-selectBackground: #f3f3f3;
--vscode-checkbox-foreground: #616161;
--vscode-checkbox-border: #cecece;
--vscode-checkbox-selectBorder: #424242;
--vscode-quickInputList-focusForeground: #000000;
--vscode-quickInputList-focusBackground: #d6ebff;
--vscode-menu-foreground: #616161;
--vscode-menu-background: #ffffff;
--vscode-menu-selectionForeground: #000000;
--vscode-menu-selectionBackground: #d6ebff;
--vscode-menu-separatorBackground: #d4d4d4;
--vscode-toolbar-hoverBackground: rgba(184, 184, 184, 0.31);
--vscode-toolbar-activeBackground: rgba(166, 166, 166, 0.31);
--vscode-editor-snippetTabstopHighlightBackground: rgba(10, 50, 100, 0.2);
--vscode-editor-snippetFinalTabstopHighlightBorder: rgba(10, 50, 100, 0.5);
--vscode-breadcrumb-foreground: rgba(97, 97, 97, 0.8);
--vscode-breadcrumb-background: #f7f7f7;
--vscode-breadcrumb-focusForeground: #4e4e4e;
--vscode-breadcrumb-activeSelectionForeground: #4e4e4e;
--vscode-breadcrumbPicker-background: #f3f3f3;
--vscode-merge-currentHeaderBackground: rgba(64, 200, 174, 0.5);
--vscode-merge-currentContentBackground: rgba(64, 200, 174, 0.2);
--vscode-merge-incomingHeaderBackground: rgba(64, 166, 255, 0.5);
--vscode-merge-incomingContentBackground: rgba(64, 166, 255, 0.2);
--vscode-merge-commonHeaderBackground: rgba(96, 96, 96, 0.4);
--vscode-merge-commonContentBackground: rgba(96, 96, 96, 0.16);
--vscode-editorOverviewRuler-currentContentForeground: rgba(64, 200, 174, 0.5);
--vscode-editorOverviewRuler-incomingContentForeground: rgba(64, 166, 255, 0.5);
--vscode-editorOverviewRuler-commonContentForeground: rgba(96, 96, 96, 0.4);
--vscode-editorOverviewRuler-findMatchForeground: rgba(209, 134, 22, 0.49);
--vscode-editorOverviewRuler-selectionHighlightForeground: rgba(0, 0, 0, 0);
--vscode-minimap-findMatchHighlight: #d18616;
--vscode-minimap-selectionOccurrenceHighlight: #c9c9c9;
--vscode-minimap-selectionHighlight: #add6ff;
--vscode-minimap-errorHighlight: rgba(255, 18, 18, 0.7);
--vscode-minimap-warningHighlight: #bf8803;
--vscode-minimap-foregroundOpacity: #000000;
--vscode-minimapSlider-background: rgba(100, 100, 100, 0.2);
--vscode-minimapSlider-hoverBackground: rgba(100, 100, 100, 0.35);
--vscode-minimapSlider-activeBackground: rgba(0, 0, 0, 0.3);
--vscode-problemsErrorIcon-foreground: #e51400;
--vscode-problemsWarningIcon-foreground: #bf8803;
--vscode-problemsInfoIcon-foreground: #1a85ff;
--vscode-charts-foreground: #616161;
--vscode-charts-lines: rgba(97, 97, 97, 0.5);
--vscode-charts-red: #e51400;
--vscode-charts-blue: #1a85ff;
--vscode-charts-yellow: #bf8803;
--vscode-charts-orange: #d18616;
--vscode-charts-green: #388a34;
--vscode-charts-purple: #652d90;
--vscode-symbolIcon-arrayForeground: #616161;
--vscode-symbolIcon-booleanForeground: #616161;
--vscode-symbolIcon-classForeground: #d67e00;
--vscode-symbolIcon-colorForeground: #616161;
--vscode-symbolIcon-constantForeground: #616161;
--vscode-symbolIcon-constructorForeground: #652d90;
--vscode-symbolIcon-enumeratorForeground: #d67e00;
--vscode-symbolIcon-enumeratorMemberForeground: #007acc;
--vscode-symbolIcon-eventForeground: #d67e00;
--vscode-symbolIcon-fieldForeground: #007acc;
--vscode-symbolIcon-fileForeground: #616161;
--vscode-symbolIcon-folderForeground: #616161;
--vscode-symbolIcon-functionForeground: #652d90;
--vscode-symbolIcon-interfaceForeground: #007acc;
--vscode-symbolIcon-keyForeground: #616161;
--vscode-symbolIcon-keywordForeground: #616161;
--vscode-symbolIcon-methodForeground: #652d90;
--vscode-symbolIcon-moduleForeground: #616161;
--vscode-symbolIcon-namespaceForeground: #616161;
--vscode-symbolIcon-nullForeground: #616161;
--vscode-symbolIcon-numberForeground: #616161;
--vscode-symbolIcon-objectForeground: #616161;
--vscode-symbolIcon-operatorForeground: #616161;
--vscode-symbolIcon-packageForeground: #616161;
--vscode-symbolIcon-propertyForeground: #616161;
--vscode-symbolIcon-referenceForeground: #616161;
--vscode-symbolIcon-snippetForeground: #616161;
--vscode-symbolIcon-stringForeground: #616161;
--vscode-symbolIcon-structForeground: #616161;
--vscode-symbolIcon-textForeground: #616161;
--vscode-symbolIcon-typeParameterForeground: #616161;
--vscode-symbolIcon-unitForeground: #616161;
--vscode-symbolIcon-variableForeground: #007acc;
--vscode-editor-lineHighlightBorder: #eeeeee;
--vscode-editor-rangeHighlightBackground: rgba(253, 255, 0, 0.2);
--vscode-editor-symbolHighlightBackground: rgba(234, 92, 0, 0.33);
--vscode-editorCursor-foreground: #000000;
--vscode-editorWhitespace-foreground: rgba(51, 51, 51, 0.2);
--vscode-editorIndentGuide-background: #d3d3d3;
--vscode-editorIndentGuide-activeBackground: #939393;
--vscode-editorLineNumber-foreground: #999999;
--vscode-editorActiveLineNumber-foreground: #0b216f;
--vscode-editorLineNumber-activeForeground: #0b216f;
--vscode-editorRuler-foreground: #d3d3d3;
--vscode-editorCodeLens-foreground: #919191;
--vscode-editorBracketMatch-background: rgba(0, 100, 0, 0.1);
--vscode-editorBracketMatch-border: #b9b9b9;
--vscode-editorOverviewRuler-border: rgba(127, 127, 127, 0.3);
--vscode-editorGutter-background: #f7f7f7;
--vscode-editorUnnecessaryCode-opacity: rgba(0, 0, 0, 0.47);
--vscode-editorGhostText-foreground: rgba(0, 0, 0, 0.47);
--vscode-editorOverviewRuler-rangeHighlightForeground: rgba(0, 122, 204, 0.6);
--vscode-editorOverviewRuler-errorForeground: rgba(255, 18, 18, 0.7);
--vscode-editorOverviewRuler-warningForeground: #bf8803;
--vscode-editorOverviewRuler-infoForeground: #1a85ff;
--vscode-editorBracketHighlight-foreground1: #0431fa;
--vscode-editorBracketHighlight-foreground2: #319331;
--vscode-editorBracketHighlight-foreground3: #7b3814;
--vscode-editorBracketHighlight-foreground4: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-foreground5: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-foreground6: rgba(0, 0, 0, 0);
--vscode-editorBracketHighlight-unexpectedBracket-foreground: rgba(255, 18, 18, 0.8);
--vscode-editorBracketPairGuide-background1: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background2: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background3: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background4: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background5: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-background6: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground1: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground2: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground3: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground4: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground5: rgba(0, 0, 0, 0);
--vscode-editorBracketPairGuide-activeBackground6: rgba(0, 0, 0, 0);
--vscode-editorUnicodeHighlight-border: #cea33d;
--vscode-editorUnicodeHighlight-background: rgba(206, 163, 61, 0.08);
--vscode-editorOverviewRuler-bracketMatchForeground: #a0a0a0;
--vscode-editor-linkedEditingBackground: rgba(255, 0, 0, 0.3);
--vscode-editor-wordHighlightBackground: rgba(87, 87, 87, 0.25);
--vscode-editor-wordHighlightStrongBackground: #d6ebff;
--vscode-editor-wordHighlightTextBackground: rgba(173, 214, 255, 0.45);
--vscode-editorOverviewRuler-wordHighlightForeground: rgba(160, 160, 160, 0.8);
--vscode-editorOverviewRuler-wordHighlightStrongForeground: rgba(192, 160, 192, 0.8);
--vscode-editorOverviewRuler-wordHighlightTextForeground: rgba(0, 0, 0, 0);
--vscode-peekViewTitle-background: #f3f3f3;
--vscode-peekViewTitleLabel-foreground: #000000;
--vscode-peekViewTitleDescription-foreground: #616161;
--vscode-peekView-border: #1a85ff;
--vscode-peekViewResult-background: #f3f3f3;
--vscode-peekViewResult-lineForeground: #646465;
--vscode-peekViewResult-fileForeground: #1e1e1e;
--vscode-peekViewResult-selectionBackground: rgba(51, 153, 255, 0.2);
--vscode-peekViewResult-selectionForeground: #6c6c6c;
--vscode-peekViewEditor-background: #f2f8fc;
--vscode-peekViewEditorGutter-background: #f2f8fc;
--vscode-peekViewEditorStickyScroll-background: #f2f8fc;
--vscode-peekViewResult-matchHighlightBackground: rgba(234, 92, 0, 0.3);
--vscode-peekViewEditor-matchHighlightBackground: rgba(245, 216, 2, 0.87);
--vscode-editorMarkerNavigationError-background: #e51400;
--vscode-editorMarkerNavigationError-headerBackground: rgba(229, 20, 0, 0.1);
--vscode-editorMarkerNavigationWarning-background: #bf8803;
--vscode-editorMarkerNavigationWarning-headerBackground: rgba(191, 136, 3, 0.1);
--vscode-editorMarkerNavigationInfo-background: #1a85ff;
--vscode-editorMarkerNavigationInfo-headerBackground: rgba(26, 133, 255, 0.1);
--vscode-editorMarkerNavigation-background: #f7f7f7;
--vscode-editorHoverWidget-highlightForeground: #0066bf;
--vscode-editorSuggestWidget-background: #f3f3f3;
--vscode-editorSuggestWidget-border: #c8c8c8;
--vscode-editorSuggestWidget-foreground: #000000;
--vscode-editorSuggestWidget-selectedForeground: #000000;
--vscode-editorSuggestWidget-selectedBackground: #d6ebff;
--vscode-editorSuggestWidget-highlightForeground: #0066bf;
--vscode-editorSuggestWidget-focusHighlightForeground: #0066bf;
--vscode-editorSuggestWidgetStatus-foreground: rgba(0, 0, 0, 0.5);
--vscode-editor-foldBackground: rgba(173, 214, 255, 0.3);
--vscode-editorGutter-foldingControlForeground: #424242; }

.mtk1 { color: #000000; }
.mtk2 { color: #f7f7f7; }
.mtk3 { color: #808080; }
.mtk4 { color: #ff0000; }
.mtk5 { color: #0451a5; }
.mtk6 { color: #0000ff; }
.mtk7 { color: #098658; }
.mtk8 { color: #008000; }
.mtk9 { color: #dd0000; }
.mtk10 { color: #811f3f; }
.mtk11 { color: #e00000; }
.mtk12 { color: #116644; }
.mtk13 { color: #383838; }
.mtk14 { color: #257693; }
.mtk15 { color: #795e26; }
.mtk16 { color: #001080; }
.mtk17 { color: #cd3131; }
.mtk18 { color: #863b00; }
.mtk19 { color: #af00db; }
.mtk20 { color: #c43b3b; }
.mtk21 { color: #800000; }
.mtk22 { color: #3030c0; }
.mtk23 { color: #666666; }
.mtk24 { color: #778899; }
.mtk25 { color: #c700c7; }
.mtk26 { color: #a31515; }
.mtk27 { color: #4f76ac; }
.mtk28 { color: #008080; }
.mtk29 { color: #001188; }
.mtk30 { color: #4864aa; }
.mtki { font-style: italic; }
.mtkb { font-weight: bold; }
.mtku { text-decoration: underline; text-underline-position: under; }
.mtks { text-decoration: line-through; }
.mtks.mtku { text-decoration: underline line-through; text-underline-position: under; }</style></head><body class="" style="overscroll-behavior: contain;"><div style="visibility: hidden; overflow: hidden; position: absolute; top: 0px; height: 1px; width: auto; padding: 0px; border: 0px; margin: 0px; text-align: left; text-indent: 0px; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal;"><div id="MathJax_Hidden"></div></div><div id="MathJax_Message" style="display: none;"></div><div class="scripts"><script nonce="">window.performance.mark('external_scripts_start');</script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/gapi_loader.js.download" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/socketio_binary.js.download" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/analytics_binary.js.download" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/MathJax.js.download" nonce=""></script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/js_monaco_editor_vs_loader.js.download" nonce=""></script><script nonce="">window.performance.mark('external_scripts_end'); window.performance.measure('external_scripts', 'external_scripts_start', 'external_scripts_end'); window.performance.mark('colab_load_start');</script><script src="./DataMining_Project3_HSM.ipynb - Colab_files/external_binary.js.download" nonce=""></script><script nonce="">
          window.performance.mark('colab_load_end');
          window.performance.measure('colab_load', 'colab_load_start', 'colab_load_end');
        </script></div><colab-snackbar leading="" labeltext="" id="message-area" class="message-area"><template shadowrootmode="open"><!----><style>
        :host .mdc-snackbar__surface {
          background-color: var(--colab-snackbar-surface-color);
        }
      </style>
      <!--?lit$944599098$-->
      <div class="mdc-snackbar mdc-snackbar--leading">
        <div class="mdc-snackbar__surface">
          <!--?lit$944599098$-->
          <div class="mdc-snackbar__actions">
            <slot name="action"></slot>
            <slot name="dismiss"></slot>
          </div>
        </div>
      </div><!--?--></template>
      <md-icon-button class="close" slot="dismiss" title="Close" aria-label="Close" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button>
    </colab-snackbar><colab-snackbar leading="" labeltext="" id="message-area-secondary" class="message-area startup"><template shadowrootmode="open"><!----><style>
        :host .mdc-snackbar__surface {
          background-color: var(--colab-snackbar-surface-color);
        }
      </style>
      <!--?lit$944599098$-->
      <div class="mdc-snackbar mdc-snackbar--leading">
        <div class="mdc-snackbar__surface">
          <!--?lit$944599098$-->
          <div class="mdc-snackbar__actions">
            <slot name="action"></slot>
            <slot name="dismiss"></slot>
          </div>
        </div>
      </div><!--?--></template>
      <md-icon-button class="close" slot="dismiss" title="Close" aria-label="Close" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button>
    </colab-snackbar><div ng-non-bindable=""></div><div class="gb_r" ng-non-bindable=""><div class="gb_Hc"><div>Google Account</div><div class="gb_Hb">maryam j</div><div>maryaamjabbari@gmail.com</div></div></div><script nonce="">this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
var md;_.kd=function(a){var b=typeof a;return"object"==b&&null!=a||"function"==b};_.ld=class extends _.O{constructor(a){super(a)}};md=class extends _.Vc{};_.nd=function(a,b){if(b in a.i)return a.i[b];throw new md;};_.od=function(a){return _.nd(_.Sc.i(),a)};
}catch(e){_._DumpException(e)}
try{
/*

 SPDX-License-Identifier: Apache-2.0
*/
var ud,Dd,Fd;_.pd=function(a){if(null==a)return a;if("string"===typeof a){if(!a)return;a=+a}if("number"===typeof a)return Number.isFinite(a)?a|0:void 0};_.qd=function(a){const b=a.length;if(0<b){const c=Array(b);for(let d=0;d<b;d++)c[d]=a[d];return c}return[]};_.sd=function(a){if(a instanceof _.rd)return a.i;throw Error("D");};ud=function(a){return new td(b=>b.substr(0,a.length+1).toLowerCase()===a+":")};
_.wd=function(a,b=_.vd){if(a instanceof _.rd)return a;for(let c=0;c<b.length;++c){const d=b[c];if(d instanceof td&&d.Yg(a))return new _.rd(a)}};_.yd=function(a){if(xd.test(a))return a};_.zd=function(a){return a instanceof _.rd?_.sd(a):_.yd(a)};_.Ad=function(a,b){var c=Array.prototype.slice.call(arguments,1);return function(){var d=c.slice();d.push.apply(d,arguments);return a.apply(this,d)}};_.Bd=function(a,b,c){return void 0!==_.jb(a,b,c,!1)};_.Cd=function(a,b){return _.pd(_.pc(a,b))};
_.R=function(a,b){a=_.pc(a,b);return null==a?a:Number.isFinite(a)?a|0:void 0};_.S=function(a,b,c=0){return _.kb(_.Cd(a,b),c)};Dd=0;_.Ed=function(a){return Object.prototype.hasOwnProperty.call(a,_.xb)&&a[_.xb]||(a[_.xb]=++Dd)};Fd=function(a){return a};_.Gd=function(a){var b=null,c=_.r.trustedTypes;if(!c||!c.createPolicy)return b;try{b=c.createPolicy(a,{createHTML:Fd,createScript:Fd,createScriptURL:Fd})}catch(d){_.r.console&&_.r.console.error(d.message)}return b};
_.Hd=function(a,b){return 0==a.lastIndexOf(b,0)};_.Id=function(a,b){return Array.prototype.some.call(a,b,void 0)};try{(new self.OffscreenCanvas(0,0)).getContext("2d")}catch(a){};var Jd;_.Kd=function(){void 0===Jd&&(Jd=_.Gd("ogb-qtm#html"));return Jd};var Nd;_.Ld=class{constructor(a){this.i=a}toString(){return this.i+""}};_.Md=function(a){return a instanceof _.Ld&&a.constructor===_.Ld?a.i:"type_error:TrustedResourceUrl"};Nd={};_.Od=function(a){const b=_.Kd();a=b?b.createScriptURL(a):a;return new _.Ld(a,Nd)};_.rd=class{constructor(a){this.i=a}toString(){return this.i}};_.Pd=new _.rd("about:invalid#zClosurez");var td,xd;td=class{constructor(a){this.Yg=a}};_.vd=[ud("data"),ud("http"),ud("https"),ud("mailto"),ud("ftp"),new td(a=>/^[^:]*([/?#]|$)/.test(a))];xd=/^\s*(?!javascript:)(?:[\w+.-]+:|[^:/?#]*(?:[/?#]|$))/i;_.Qd={};_.Rd=class{constructor(a){this.i=a}toString(){return this.i.toString()}};_.Sd=new _.Rd("",_.Qd);_.Td=RegExp("^[-+,.\"'%_!#/ a-zA-Z0-9\\[\\]]+$");_.Ud=RegExp("\\b(url\\([ \t\n]*)('[ -&(-\\[\\]-~]*'|\"[ !#-\\[\\]-~]*\"|[!#-&*-\\[\\]-~]*)([ \t\n]*\\))","g");_.Vd=RegExp("\\b(calc|cubic-bezier|fit-content|hsl|hsla|linear-gradient|matrix|minmax|radial-gradient|repeat|rgb|rgba|(rotate|scale|translate)(X|Y|Z|3d)?|steps|var)\\([-+*/0-9a-zA-Z.%#\\[\\], ]+\\)","g");_.Wd={};_.Yd=function(a){return a instanceof _.Xd&&a.constructor===_.Xd?a.i:"type_error:SafeHtml"};_.Xd=class{constructor(a){this.i=a}toString(){return this.i.toString()}};_.Zd=new _.Xd(_.r.trustedTypes&&_.r.trustedTypes.emptyHTML||"",_.Wd);var ae;_.$d=function(a){let b=!1,c;return function(){b||(c=a(),b=!0);return c}}(function(){var a=document.createElement("div"),b=document.createElement("div");b.appendChild(document.createElement("div"));a.appendChild(b);b=a.firstChild.firstChild;a.innerHTML=_.Yd(_.Zd);return!b.parentElement});ae=/^[\w+/_-]+[=]{0,2}$/;
_.be=function(a){a=(a||_.r).document;return a.querySelector?(a=a.querySelector('style[nonce],link[rel="stylesheet"][nonce]'))&&(a=a.nonce||a.getAttribute("nonce"))&&ae.test(a)?a:"":""};_.ce=function(a,b){this.width=a;this.height=b};_.m=_.ce.prototype;_.m.aspectRatio=function(){return this.width/this.height};_.m.Gb=function(){return!(this.width*this.height)};_.m.ceil=function(){this.width=Math.ceil(this.width);this.height=Math.ceil(this.height);return this};_.m.floor=function(){this.width=Math.floor(this.width);this.height=Math.floor(this.height);return this};_.m.round=function(){this.width=Math.round(this.width);this.height=Math.round(this.height);return this};_.T=function(a,b){var c=b||document;if(c.getElementsByClassName)a=c.getElementsByClassName(a)[0];else{c=document;var d=b||c;a=d.querySelectorAll&&d.querySelector&&a?d.querySelector(a?"."+a:""):_.de(c,a,b)[0]||null}return a||null};
_.de=function(a,b,c){var d;a=c||a;if(a.querySelectorAll&&a.querySelector&&b)return a.querySelectorAll(b?"."+b:"");if(b&&a.getElementsByClassName){var e=a.getElementsByClassName(b);return e}e=a.getElementsByTagName("*");if(b){var f={};for(c=d=0;a=e[c];c++){var g=a.className;"function"==typeof g.split&&_.ta(g.split(/\s+/),b)&&(f[d++]=a)}f.length=d;return f}return e};_.fe=function(a){return _.ee(document,a)};
_.ee=function(a,b){b=String(b);"application/xhtml+xml"===a.contentType&&(b=b.toLowerCase());return a.createElement(b)};_.ge=function(a){for(var b;b=a.firstChild;)a.removeChild(b)};_.he=function(a){return 9==a.nodeType?a:a.ownerDocument||a.document};
}catch(e){_._DumpException(e)}
try{
_.Li=function(a){var b;let c;const d=null==(c=(b=(a.ownerDocument&&a.ownerDocument.defaultView||window).document).querySelector)?void 0:c.call(b,"script[nonce]");(b=d?d.nonce||d.getAttribute("nonce")||"":"")&&a.setAttribute("nonce",b)};_.Mi=function(a){if(!a)return null;a=_.G(a,4);var b;null===a||void 0===a?b=null:b=_.Od(a);return b};_.Ni=class extends _.O{constructor(a){super(a)}};_.Oi=function(a,b){return(b||document).getElementsByTagName(String(a))};
}catch(e){_._DumpException(e)}
try{
var Qi=function(a,b,c){a<b?Pi(a+1,b):_.Bc.log(Error("ca`"+a+"`"+b),{url:c})},Pi=function(a,b){if(Ri){const c=_.fe("SCRIPT");c.async=!0;c.type="text/javascript";c.charset="UTF-8";c.src=_.Md(Ri);_.Li(c);c.onerror=_.Ad(Qi,a,b,c.src);_.Oi("HEAD")[0].appendChild(c)}},Si=class extends _.O{constructor(a){super(a)}};var Ti=_.C(_.Mc,Si,17)||new Si,Ui,Ri=(Ui=_.C(Ti,_.Ni,1))?_.Mi(Ui):null,Vi,Wi=(Vi=_.C(Ti,_.Ni,2))?_.Mi(Vi):null,Xi=function(){Pi(1,2);if(Wi){const b=_.fe("LINK");b.setAttribute("type","text/css");b.rel="stylesheet";b.href=_.Md(Wi).toString();var a=_.be(b.ownerDocument&&b.ownerDocument.defaultView);a&&b.setAttribute("nonce",a);(a=_.be())&&b.setAttribute("nonce",a);_.Oi("HEAD")[0].appendChild(b)}};(function(){const a=_.Nc();if(_.F(a,18))Xi();else{const b=_.Cd(a,19)||0;window.addEventListener("load",()=>{window.setTimeout(Xi,b)})}})();
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script><div style="position: absolute; width: 0px; height: 0px; overflow: hidden; padding: 0px; border: 0px; margin: 0px;"><div id="MathJax_Font_Test" style="position: absolute; visibility: hidden; top: 0px; left: 0px; width: auto; min-width: 0px; max-width: none; padding: 0px; border: 0px; margin: 0px; white-space: nowrap; text-align: left; text-indent: 0px; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; font-size: 40px; font-weight: normal; font-style: normal; font-family: MathJax_Size1, monospace;"></div></div><iframe id="hfcr" src="./DataMining_Project3_HSM.ipynb - Colab_files/RotateCookiesPage.html" style="display: none;"></iframe><div class="notebook-vertical" style="position: relative;">
      <div class="top-floater"><div role="banner">
    <colab-header-skip-button><template shadowrootmode="open"><!----><a id="skiplink" class="skip-link" href="https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId#top-toolbar"><!--?lit$944599098$-->Skip to main content</a></template></colab-header-skip-button>
    <!--?lit$944599098$-->
    <!--?lit$944599098$-->
    <!--?lit$944599098$-->
          <div id="private-outputs-warning" class="header-warning private-outputs-warning hidden">
            <!--?lit$944599098$-->This notebook is open with private outputs. Outputs will not be saved. You can disable this in <a href="https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId#" id="private-outputs-notebook-info-link" command="notebook-settings" aria-describedby="private-outputs-notebook-info-link-tooltip">Notebook settings</a><colab-tooltip-trigger aria-hidden="true" for="private-outputs-notebook-info-link" id="private-outputs-notebook-info-link-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Open notebook settings</div><!----><!--?--></template>
        </colab-tooltip-trigger>.
          <mwc-icon-button class="close" icon="close" title="Close"><template shadowrootmode="open"><!----><button class="mdc-icon-button mdc-icon-button--display-flex" aria-label="Close"><!--?lit$944599098$-->
    <!--?lit$944599098$--><i class="material-icons"><!--?lit$944599098$-->close</i>
    <span><slot></slot></span>
  </button></template></mwc-icon-button></div>
        

    <div id="header" class="horizontal layout">
      <div id="header-background"><div></div></div>
      <div id="header-content">
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><div id="header-logo">
              <!--?lit$944599098$--> <!--?lit$944599098$--><a href="https://drive.google.com/drive/search?q=owner%3Ame%20(type%3Aapplication%2Fvnd.google.colaboratory%20%7C%7C%20type%3Aapplication%2Fvnd.google.colab)&amp;authuser=0" aria-label="View in Google Drive">
        <!--?lit$944599098$--><md-icon class="colab-large-icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$-->
      <g id="colab-logo">
        <path d="M4.54,9.46,2.19,7.1a6.93,6.93,0,0,0,0,9.79l2.36-2.36A3.59,3.59,0,0,1,4.54,9.46Z" style="fill:var(--colab-logo-dark)"></path>
        <path d="M2.19,7.1,4.54,9.46a3.59,3.59,0,0,1,5.08,0l1.71-2.93h0l-.1-.08h0A6.93,6.93,0,0,0,2.19,7.1Z" style="fill:var(--colab-logo-light)"></path>
        <path d="M11.34,17.46h0L9.62,14.54a3.59,3.59,0,0,1-5.08,0L2.19,16.9a6.93,6.93,0,0,0,9,.65l.11-.09" style="fill:var(--colab-logo-light)"></path>
        <path d="M12,7.1a6.93,6.93,0,0,0,0,9.79l2.36-2.36a3.59,3.59,0,1,1,5.08-5.08L21.81,7.1A6.93,6.93,0,0,0,12,7.1Z" style="fill:var(--colab-logo-light)"></path>
        <path d="M21.81,7.1,19.46,9.46a3.59,3.59,0,0,1-5.08,5.08L12,16.9A6.93,6.93,0,0,0,21.81,7.1Z" style="fill:var(--colab-logo-dark)"></path>
      </g></svg></md-icon>
      </a><!--?-->
            </div>
        <div id="header-doc-toolbar" class="flex">
          <div id="document-info">
            <!--?lit$944599098$--> <!--?lit$944599098$--><md-icon class="file-location-icon" id="file-type" aria-hidden="true" title="Notebook stored in Google Drive"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->
      <svg viewBox="0 0 192 192">
        <path d="M128.33,122l7.59,26.17l19.89,21.42c0,0,0,0,0,0v0c2.69-1.55,4.98-3.8,6.59-6.59l18.48-32 c1.61-2.78,2.41-5.89,2.41-9l-28.38-5.5L128.33,122z" fill="#EA4335"></path>
        <path d="M123.48,18.41c-2.69-1.55-5.78-2.41-9-2.41H77.53c-3.2,0-6.32,0.88-9,2.41l0,0l7.96,26.81l19.44,20.64 L96,66l0,0l19.58-20.89L123.48,18.41C123.48,18.41,123.48,18.41,123.48,18.41C123.48,18.41,123.48,18.41,123.48,18.41z" fill="#188038"></path>
        <path d="M63.67,122l-28.33-6.5L8.72,122c0,3.1,0.8,6.2,2.4,8.99L29.6,163c1.61,2.78,3.9,5.03,6.59,6.59 l19.59-20.18L63.67,122L63.67,122z" fill="#1967D2"></path>
        <path d="M155.47,69l-25.4-44c-1.61-2.79-3.9-5.04-6.59-6.59L96,66l32.33,56h54.95c0-3.11-0.8-6.21-2.41-9 L155.47,69z" fill="#FBBC04"></path><path d="M128.33,122H63.67l-27.48,47.59c2.69,1.55,5.78,2.41,9,2.41h101.61c3.22,0,6.31-0.86,9-2.41L128.33,122z" fill="#4285F4"></path>
        <path d="M96,66L68.53,18.41c-2.69,1.55-4.97,3.79-6.58,6.57l-50.83,88.05c-1.6,2.78-2.4,5.88-2.4,8.97h54.95L96,66 z" fill="#34A853"></path>
      </svg></md-icon>
    <input id="doc-name" class="doc-name" maxlength="259" autocomplete="off" aria-label="Notebook name" command="rename" style="width: 272.7px;" aria-describedby="doc-name-tooltip"><colab-tooltip-trigger aria-hidden="true" for="doc-name" id="doc-name-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Rename notebook</div><!----><!--?--></template>
        </colab-tooltip-trigger><colab-input-sizer aria-hidden="true" style="left: -1000%; position: absolute; font-family: &quot;Google Sans&quot;, Roboto, Noto, sans-serif; font-size: 18px; font-weight: 400; letter-spacing: normal; padding-left: 3px; padding-right: 4px; white-space: pre;">DataMining_Project3_HSM.ipynb_</colab-input-sizer>
            <!--?lit$944599098$-->
                  <div class="screenreader-only" id="star-status" aria-live="polite">Notebook unstarred</div>
                  <md-icon-button id="star-icon" command="toggle-star" aria-label="Star" role="presentation" aria-describedby="star-icon-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Star">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
                    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>star</md-icon>
                  </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="star-icon" id="star-icon-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Star notebook in Google Drive</div><!----><!--?--></template>
        </colab-tooltip-trigger>
                
          </div>
        <div class="menubar-wrapper"><div><!----><div id="top-menubar" class="goog-menubar format-lightborder" role="menubar" tabindex="0" style="user-select: none;"><!--?lit$944599098$--><div class="goog-menu-button goog-inline-block" id="file-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->File</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="edit-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->Edit</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="view-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->View</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="insert-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->Insert</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="runtime-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->Runtime</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="tools-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->Tools</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div><div class="goog-menu-button goog-inline-block" id="help-menu-button" role="button" aria-expanded="false" aria-haspopup="true" style="user-select: none;"><div class="goog-inline-block goog-menu-button-outer-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-inner-box" style="user-select: none;"><div class="goog-inline-block goog-menu-button-caption" style="user-select: none;"><!--?lit$944599098$-->Help</div><div class="goog-inline-block goog-menu-button-dropdown" style="user-select: none;">&nbsp;</div></div></div></div></div>
    <div id="colab-menu-cover" style="display: none;"> </div></div><!----><colab-last-saved-indicator aria-live="polite" aria-atomic="true" title=""><template shadowrootmode="open"><!----><button class=" save-message "><!--?lit$944599098$-->All changes saved</button></template></colab-last-saved-indicator></div></div>
        <div id="header-right">
          <!--?lit$944599098$-->
    <colab-collaborator-bar id="collaborator-bar"><template shadowrootmode="open"><!----> <div class="collaborator-bar">
      <!--?lit$944599098$-->
      <!--?lit$944599098$-->
    </div></template></colab-collaborator-bar>
  
          <!--?lit$944599098$--> <md-text-button id="comments" command="open-comments-thread" role="presentation" aria-describedby="comments-tooltip" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
                <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>comment</md-icon>
                <!--?lit$944599098$-->Comment
              </md-text-button><colab-tooltip-trigger aria-hidden="true" for="comments" id="comments-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Open comments pane</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <!--?lit$944599098$--> <md-text-button id="share-toolbar-button" command="share" role="presentation" aria-describedby="share-toolbar-button-tooltip" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
                <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->people</md-icon>
                <!--?lit$944599098$-->Share
              </md-text-button><colab-tooltip-trigger aria-hidden="true" for="share-toolbar-button" id="share-toolbar-button-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Share notebook</div><!----><!--?--></template>
        </colab-tooltip-trigger>
          <!--?lit$944599098$--> <md-icon-button id="settings-cog" command="preferences" title="Open settings" aria-label="Open settings" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open settings">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
                <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>settings</md-icon>
              </md-icon-button>
          <div class="header-onegoogle-container"><div class="onegoogle"><div class="gb_Ra gb_md gb_ib gb_2c" id="gb"><div class="gb_Dd gb_gb gb_rd" ng-non-bindable="" data-ogsr-up="" style="padding:0;height:auto;display:block"><div class="gb_Vd" style="display:block"><div class="gb_8c"></div><div class="gb_b gb_x gb_4f gb_K"><div class="gb_f gb_fb gb_4f gb_K"><a class="gb_d gb_Ia gb_K" aria-label="Google Account: maryam j  
(maryaamjabbari@gmail.com)" href="https://accounts.google.com/SignOutOptions?hl=en&amp;continue=https://colab.research.google.com/drive/1KfNEVY9UDb7tJa62q2GyppWfOgtRuVId&amp;ec=GBRAqQM" tabindex="0" role="button"><img class="gb_p gbii" src="./DataMining_Project3_HSM.ipynb - Colab_files/unnamed.png" srcset="https://lh3.google.com/u/0/ogw/AF2bZyhyjVUZv-NqSnUyO499Pqsu4cmMriJvl5c7jEWjm49pYQ=s32-c-mo 1x, https://lh3.google.com/u/0/ogw/AF2bZyhyjVUZv-NqSnUyO499Pqsu4cmMriJvl5c7jEWjm49pYQ=s64-c-mo 2x " alt="" aria-hidden="true" data-noaft=""></a></div></div></div><div style="overflow: hidden; position: absolute; top: 0px; visibility: hidden; width: 436px; z-index: 991; height: 0px; margin-top: 57px; right: 0px; margin-right: 4px;"></div></div></div><script nonce="">this.gbar_=this.gbar_||{};(function(_){var window=this;
try{
_.gd=function(a,b,c){if(!a.j)if(c instanceof Array)for(var d of c)_.gd(a,b,d);else{d=(0,_.y)(a.C,a,b);const e=a.v+c;a.v++;b.dataset.eqid=e;a.B[e]=d;b&&b.addEventListener?b.addEventListener(c,d,!1):b&&b.attachEvent?b.attachEvent("on"+c,d):a.o.log(Error("z`"+b))}};
}catch(e){_._DumpException(e)}
try{
_.hd=function(){if(!_.r.addEventListener||!Object.defineProperty)return!1;var a=!1,b=Object.defineProperty({},"passive",{get:function(){a=!0}});try{const c=()=>{};_.r.addEventListener("test",c,b);_.r.removeEventListener("test",c,b)}catch(c){}return a}();
}catch(e){_._DumpException(e)}
try{
var id=document.querySelector(".gb_k .gb_d"),jd=document.querySelector("#gb.gb_Zc");id&&!jd&&_.gd(_.Rc,id,"click");
}catch(e){_._DumpException(e)}
try{
_.jh=function(a){const b=[];let c=0;for(const d in a)b[c++]=a[d];return b};_.kh=function(a){if(a.v)return a.v;for(const b in a.i)if(a.i[b].qa()&&a.i[b].B())return a.i[b];return null};_.lh=function(a,b){a.i[b.K()]=b};var mh=new class extends _.P{constructor(){var a=_.Bc;super();this.B=a;this.v=null;this.o={};this.C={};this.i={};this.j=null}A(a){this.i[a]&&(_.kh(this)&&_.kh(this).K()==a||this.i[a].P(!0))}Xa(a){this.j=a;for(const b in this.i)this.i[b].qa()&&this.i[b].Xa(a)}oc(a){return a in this.i?this.i[a]:null}};_.Uc("dd",mh);
}catch(e){_._DumpException(e)}
try{
_.Ei=function(a,b){return _.K(a,36,b)};
}catch(e){_._DumpException(e)}
try{
var Fi=document.querySelector(".gb_b .gb_d"),Gi=document.querySelector("#gb.gb_Zc");Fi&&!Gi&&_.gd(_.Rc,Fi,"click");
}catch(e){_._DumpException(e)}
})(this.gbar_);
// Google Inc.
</script></div></div>
        </div>
      </div>
    </div>
  </div></div><div class="notebook-horizontal">
        <!--?lit$944599098$--><colab-left-pane role="complementary" aria-label="left pane"><!----><div class="colab-left-pane-nib layout vertical" role="toolbar" aria-orientation="vertical">
        <div class="left-pane-top"><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button toggle="" command="show-toc-pane" aria-label="Table of contents" title="Table of contents" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Table of contents" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->format_list_bulleted</md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button toggle="" command="find" aria-label="Find and replace" title="Find and replace" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Find and replace" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->search</md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button toggle="" command="show-variables" aria-label="Variables" title="Variables" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Variables" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$-->
      <path d="M4.51,9.44V6.08c0-1.34.37-1.85,1.6-2.17l.22-.06V3.13l-.27,0-.44,0a4.46,4.46,0,0,0-2.2.59,2.78,2.78,0,0,0-1,2.51V9.74c0,1.26-.26,1.61-1.49,2L0,12l.94.29c1.21.38,1.49.75,1.49,2v3.5a2.94,2.94,0,0,0,1,2.6,4.39,4.39,0,0,0,2.14.56l.46,0,.27,0v-.72l-.22-.06c-1.24-.32-1.6-.81-1.6-2.17V14.58c0-1.43-.3-2.13-1.25-2.57C4.2,11.57,4.51,10.87,4.51,9.44Z"></path>
      <path d="M23.06,11.71c-1.22-.36-1.49-.71-1.49-2l0-3.5a3,3,0,0,0-1-2.6,4.38,4.38,0,0,0-2.14-.56l-.46,0-.27,0v.72l.22.06c1.24.32,1.6.81,1.6,2.17V9.44c0,1.44.3,2.13,1.25,2.57-1,.44-1.25,1.14-1.25,2.57v3.36c0,1.34-.37,1.85-1.6,2.17l-.22.06v.72l.27,0,.44,0a4.47,4.47,0,0,0,2.2-.59,2.82,2.82,0,0,0,1-2.51V14.28c0-1.26.26-1.61,1.49-2L24,12Z"></path>
      <path d="M15.16,8.22a.88.88,0,0,1,.46.16,1.25,1.25,0,0,0,.69.2h0A1,1,0,0,0,17,8.23a1.06,1.06,0,0,0,.24-.8,1.1,1.1,0,0,0-1.15-1h0c-1,0-1.73.64-3,2.57l-.12-.51c-.28-1.36-.56-2-1.39-2h0A8,8,0,0,0,9,7.08l-.47.16.16.91L9.41,8a3.22,3.22,0,0,1,.73-.14c.34,0,.43,0,.71,1.2l.56,2.47L9.76,13.82a3.6,3.6,0,0,1-.8.88.9.9,0,0,1-.38-.13,1.83,1.83,0,0,0-.88-.28,1,1,0,0,0-1,1.06A1.15,1.15,0,0,0,8,16.53c.85,0,1.35-.35,2.24-1.55l1.49-2,.46,1.88c.23,1,.46,1.66,1.53,1.66s1.66-.75,2.81-2.53l.17-.26-.81-.48-.16.2-.25.34-.19.25c-.45.57-.62.73-.76.73s-.28-.4-.34-.63l-.67-2.83a4.2,4.2,0,0,1-.15-.79C13.84,9.78,14.74,8.22,15.16,8.22Z"></path></svg></md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button toggle="" command="open-user-secrets" aria-label="Secrets" title="Secrets" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Secrets" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->vpn_key</md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button toggle="" command="show-files" aria-label="Files" title="Files" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Files" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->folder</md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div></div>
        <div class="left-pane-bottom"><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button command="snippets" aria-label="Code snippets" title="Code snippets" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code snippets">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->code</md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div><!----><div class="left-pane-button">
        <!--?lit$944599098$--><md-icon-button command="show-command-palette" aria-label="Command palette" title="Command palette" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Command palette">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$-->
      <path d="M21,3H3A2,2,0,0,0,1,5V17a2,2,0,0,0,2,2H21a2,2,0,0,0,2-2V5A2,2,0,0,0,21,3Zm0,2V17H3V5"></path>
      <rect x="5" y="12" width="11" height="2"></rect>
      <rect x="5" y="8" width="11" height="2"></rect>
      <rect x="17" y="8" width="2" height="2"></rect>
      <rect x="17" y="12" width="2" height="2"></rect></svg></md-icon>
        </md-icon-button> <!--?lit$944599098$-->
      </div></div>
      </div></colab-left-pane>
        <div class="layout vertical grow">
          <colab-notebook-toolbar id="top-toolbar" class="horizontal layout center noshrink"><!----> <!--?lit$944599098$-->
          <colab-toolbar-button command="insert-cell-below" icon="add" id="toolbar-add-code"><template shadowrootmode="open"><!----><md-text-button id="button" aria-disabled="false" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
        <!--?lit$944599098$--><md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->add</md-icon>
        <span class="button-content"><slot></slot></span>
        <!--?lit$944599098$--><span class="screenreader-only"><!--?lit$944599098$-->Insert code cell below <!--?lit$944599098$-->Ctrl+M B</span>
      </md-text-button>
      <!--?lit$944599098$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="tooltip" message="Insert code cell below" shortcut="Ctrl+M B"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Insert code cell below</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
            <!--?lit$944599098$-->Code
          </colab-toolbar-button>
          <colab-toolbar-button command="add-text" icon="add" id="toolbar-add-text"><template shadowrootmode="open"><!----><md-text-button id="button" aria-disabled="false" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
        <!--?lit$944599098$--><md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->add</md-icon>
        <span class="button-content"><slot></slot></span>
        <!--?lit$944599098$--><span class="screenreader-only"><!--?lit$944599098$-->Add text cell <!--?lit$944599098$--></span>
      </md-text-button>
      <!--?lit$944599098$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="tooltip" message="Add text cell" shortcut=""><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Add text cell</div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
            <!--?lit$944599098$-->Text
          </colab-toolbar-button>
          <!--?lit$944599098$-->
        
    <!--?lit$944599098$-->
    <!--?lit$944599098$-->
    <!--?lit$944599098$-->
    <!--?lit$944599098$--> <span class="collapsed-options">
          <colab-last-saved-indicator aria-live="polite" aria-atomic="true" title=""><template shadowrootmode="open"><!----><button class=" save-message "><!--?lit$944599098$-->All changes saved</button></template></colab-last-saved-indicator>
        </span>

    <span class="flex"></span>
    <!--?lit$944599098$--><colab-connect-warning-button><template shadowrootmode="open"><!----><!--?lit$944599098$--><!--?--><!--?--></template></colab-connect-warning-button>
    <!--?lit$944599098$--><!--?lit$944599098$--><colab-connect-button><template shadowrootmode="open"><!----> <!--?lit$944599098$--><!--?-->
      <colab-toolbar-button id="connect" tooltipid="colab-connect-tooltip" tooltiptext="Connect to a new runtime

          "><template shadowrootmode="open"><!----><md-text-button id="button" aria-disabled="false" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
        <!--?lit$944599098$-->
        <span class="button-content"><slot></slot></span>
        <!--?lit$944599098$--><span class="screenreader-only"><!--?lit$944599098$-->Connect to a new runtime

           <!--?lit$944599098$--></span>
      </md-text-button>
      <!--?lit$944599098$--> <colab-tooltip-trigger for="button" aria-hidden="true" id="colab-connect-tooltip" message="Connect to a new runtime

          " shortcut=""><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Connect to a new runtime</div><!----><!----><div><!--?lit$944599098$--></div><!----><!----><div><!--?lit$944599098$-->          </div><!----><!--?--></template>
          </colab-tooltip-trigger><!--?--></template>
        <!--?lit$944599098$-->Connect
      </colab-toolbar-button>
      <!--?lit$944599098$--> <md-icon-button id="connect-dropdown" aria-label="Additional connection options" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Additional connection options">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>arrow_drop_down</md-icon>
      </md-icon-button>
      <colab-tooltip-trigger for="connect-dropdown" id="connect-dropdown-tooltip" aria-hidden="true" message="Additional connection options"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Additional connection options</div><!----><!--?--></template>
      </colab-tooltip-trigger><!--?--></template></colab-connect-button><!--?-->
    <!--?lit$944599098$-->
    <!--?lit$944599098$-->
    <span class="collapsed-options">
      <!--?lit$944599098$--><span class="colab-separator"></span>
      <!--?lit$944599098$--> <md-icon-button command="share" title="Share notebook" aria-label="Share notebook" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Share notebook">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
            <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->people</md-icon>
          </md-icon-button><md-icon-button command="preferences" aria-label="Open settings" title="Open settings" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open settings">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>settings</md-icon>
      </md-icon-button>
    </span>
    <span class="colab-separator"></span>
    <!--?lit$944599098$--><md-icon-button toggle="" command="toggle-header" id="toggle-header-button" aria-label="Toggle header visibility" role="presentation" aria-describedby="toggle-header-button-tooltip" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Toggle header visibility" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>expand_less</md-icon>
    <md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>expand_more</md-icon>
  </md-icon-button><colab-tooltip-trigger aria-hidden="true" for="toggle-header-button" id="toggle-header-button-tooltip"><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----><div><!--?lit$944599098$-->Toggle header visibility</div><!----><!--?--></template>
        </colab-tooltip-trigger><!--?--></colab-notebook-toolbar><colab-tab-layout-container class="layout horizontal grow flexible-tabs"><!----> <div class="layout horizontal tab-pane-parent">
      <!--?lit$944599098$--> <div class="layout vertical tab-pane-parent">
      <!--?lit$944599098$--><colab-tab-pane class="layout vertical grow no-header focused" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template><md-primary-tab noink="" title="" aria-labelledby="tab-title-y77Sqykx8qco" class="selected-tab" tabindex="0" md-tab="" active=""><template shadowrootmode="open"><!----><div class="button" role="presentation">
      <md-focus-ring part="focus-ring" inward="" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-elevation part="elevation" aria-hidden="true"><template shadowrootmode="open"><!----><span class="shadow"></span></template></md-elevation>
      <md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <div role="presentation" class="content  has-label stacked ">
        <slot name="icon"></slot>
        <slot></slot>
        <!--?lit$944599098$--><div class="indicator"></div>
      </div>
      <!--?lit$944599098$-->
    </div></template>
          <div class="colab-tab-header">
            <span class="colab-tab-title" id="tab-title-y77Sqykx8qco"><!--?lit$944599098$--><!--?lit$944599098$-->Notebook<!--?--></span>
            <!--?lit$944599098$-->
          </div>
        </md-primary-tab></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$944599098$--> <md-icon-button title="Show more" aria-label="Show more" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show more">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> <colab-tab class="layout vertical grow notebook-tab-content selected-tab"><!----> <div class="overflow-flexbox-workaround">
      <colab-shaded-scroller ignore-dom-changes="" tabindex="-1" role="main" class="notebook-container" aria-label="Notebook">
        <div class="notebook-scrolling-horizontal-container">
          <div class="notebook-scrolling-horizontal">
            <div class="notebook-content-background">
              <!--?lit$944599098$-->
              <div class="notebook-content ">
                <!--?lit$944599098$--><div class="add-cell">
      <hr>
    </div>
                <div class="notebook-cell-list"><div class="cell code icon-scrolling" id="cell-wqiVDGR55Wfk" tabindex="-1" role="region" aria-label="Cell 0: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab" data-lang="notebook-python"><span><span class="mtk6">!</span><span class="mtk1">pip&nbsp;install&nbsp;langdetect</span></span><br><span><span class="mtk6">!</span><span class="mtk1">pip&nbsp;install&nbsp;scispacy</span></span><br><span><span class="mtk6">!</span><span class="mtk1">pip&nbsp;install&nbsp;https://s3-us-west-</span><span class="mtk7">2.</span><span class="mtk1">amazonaws.com/ai2-s2-scispacy/releases/v0</span><span class="mtk7">.5.4</span><span class="mtk1">/en_core_sci_lg-</span><span class="mtk7">0.5.4</span><span class="mtk1">.tar.gz</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 0 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-hF_lqFaDUMGY" tabindex="-1" role="region" aria-label="Cell 1: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab" data-lang="notebook-python"><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;numpy&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;np</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Plotting&nbsp;and&nbsp;visualization</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;matplotlib.pyplot&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;plt</span></span><br><span><span class="mtk1">plt.style.use(</span><span class="mtk26">'ggplot'</span><span class="mtk1">)</span></span><br><span><span class="mtk6">%config&nbsp;</span><span class="mtk1">InlineBackend.figure_formats&nbsp;=&nbsp;[</span><span class="mtk26">'svg'</span><span class="mtk1">]</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;seaborn&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;sns</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Used&nbsp;to&nbsp;draw&nbsp;a&nbsp;progress&nbsp;bar&nbsp;for&nbsp;longer&nbsp;method&nbsp;ca</span><span class="mtk8">lls</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;tqdm&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;tqdm</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Used&nbsp;to&nbsp;detect&nbsp;language&nbsp;used&nbsp;in&nbsp;each&nbsp;document</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;langdetect&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;detect</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;langdetect&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;DetectorFactory</span></span><br><span><span class="mtk1">DetectorFactory.seed&nbsp;=&nbsp;</span><span class="mtk12">0</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Pre-trained&nbsp;natural&nbsp;language&nbsp;processing&nbsp;pipeline</span><span class="mtk8">&nbsp;for&nbsp;biomedical&nbsp;use</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;spacy</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;spacy.lang.en.stop_words&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;STOP_WORDS</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;en_core_sci_lg</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Used&nbsp;to&nbsp;import&nbsp;list&nbsp;of&nbsp;punctuations</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;string</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Feature&nbsp;extraction&nbsp;(text&nbsp;vectorizers)</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.feature_extraction.text&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;TfidfVectorizer</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.feature_extraction.text&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;CountVectorizer</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Dimensionality&nbsp;reduction</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.decomposition&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;PCA</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.manifold&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;TSNE</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Clustering&nbsp;and&nbsp;evaluation</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.cluster&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;KMeans</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;metrics</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;scipy.spatial.distance&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;cdist</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Topic&nbsp;modeling</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.decomposition&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;LatentDirichletAllocation</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 1 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-KihLPswAcgvn" tabindex="-1" role="region" aria-label="Cell 2: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 5.807s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk6">!</span><span class="mtk1">gdown&nbsp;</span><span class="mtk7">15E8</span><span class="mtk1">FLX0C-</span><span class="mtk7">6</span><span class="mtk1">qpK-lDBEQJXw00Lsdcvjae</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 2 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 5.807s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>Downloading...
From (original): <a rel="nofollow" target="_blank" href="https://drive.google.com/uc?id=15E8FLX0C-6qpK-lDBEQJXw00Lsdcvjae">https://drive.google.com/uc?id=15E8FLX0C-6qpK-lDBEQJXw00Lsdcvjae</a>
From (redirected): <a rel="nofollow" target="_blank" href="https://drive.google.com/uc?id=15E8FLX0C-6qpK-lDBEQJXw00Lsdcvjae&amp;confirm=t&amp;uuid=1da5c918-f025-4c9d-b4ca-668473d323a6">https://drive.google.com/uc?id=15E8FLX0C-6qpK-lDBEQJXw00Lsdcvjae&amp;confirm=t&amp;uuid=1da5c918-f025-4c9d-b4ca-668473d323a6</a>
To: /content/10k_df.csv
100% 341M/341M [00:03&lt;00:00, 86.5MB/s]
</pre></div></div><div></div></colab-static-output-renderer></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell text" id="cell-mY9evTyRQA82" tabindex="-1" role="region" aria-label="Cell 3: Text cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><!----> <div class="toolbar-root"></div>
      <div class="editor-container horizontal">
        <div class="editor-root"></div>
        <div class="text-top-div">
          <div class="markdown"><span><p>!gdown 15E8FLX0C-6qpK-lDBEQJXw00Lsdcvjae</p>
</span></div>
        </div>
      </div>

      <div class="section-header" style="display: none;">
        <colab-run-button role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
        <div class="section-header-container" title="click to expand">↳ 0 cells hidden</div>
      </div></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-mG_ng9hsUMGc" tabindex="-1" role="region" aria-label="Cell 4: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df_10k&nbsp;=&nbsp;pd.read_csv(</span><span class="mtk26">'10k_df.csv'</span><span class="mtk1">)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 4 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-CppfUdF3Zyp8" tabindex="-1" role="region" aria-label="Cell 5: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df_10k.fillna(value=</span><span class="mtk26">"&nbsp;"</span><span class="mtk1">,inplace=</span><span class="mtk6">True</span><span class="mtk1">)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 5 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-ehfaa_-eUMGd" tabindex="-1" role="region" aria-label="Cell 6: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df&nbsp;=&nbsp;df_10k.sample(</span><span class="mtk12">1500</span><span class="mtk1">,&nbsp;random_state=</span><span class="mtk12">400</span><span class="mtk1">)</span></span><br><span><span class="mtk19">del</span><span class="mtk1">&nbsp;df_10k</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 6 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-IOYhxehocv0S" tabindex="-1" role="region" aria-label="Cell 7: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.046s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df.shape</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 7 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.046s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="execute_result output_text"><pre>(1500, 8)</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-Bft2mKhUdtUT" tabindex="-1" role="region" aria-label="Cell 8: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 64.515s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="8" data-mode-id="notebook-python" style="height: 333px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs" role="code" data-uri="inmemory://model/17" style="width: 1411px; height: 333px;"><div data-mprt="3" class="overflow-guard" style="width: 1411px; height: 333px;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 333px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 333px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 333px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1405px; height: 333px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 333px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1405px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1405px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1405px; height: 333px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Part&nbsp;1:</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;langdetect&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;detect,&nbsp;DetectorFactory</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;langdetect.lang_detect_exception&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;LangDetectException</span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">detect_language</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk16">text</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">:</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk19">try</span><span class="mtk1">:</span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;detect</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">text</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk19">except</span><span class="mtk1">&nbsp;LangDetectException:</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;</span><span class="mtk26">'unknown'</span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'language'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'body_text'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">.apply</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">detect_language</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span class="mtk1">df&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'language'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">&nbsp;==&nbsp;</span><span class="mtk26">'en'</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span class="mtk1">df.drop</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'language'</span><span class="mtk1">,&nbsp;axis=</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;inplace=</span><span class="mtk6">True</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">df.shape</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute; width: 1391px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1391px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="416" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 333px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 333px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 333px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1411px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 1411px; height: 1px;"></textarea><div style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;" class="monaco-editor-background textAreaCover"></div><div data-mprt="4" class="overlayWidgets" style="width: 1411px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 333px;"><div class="minimap-shadow-hidden" style="height: 333px;"></div><canvas width="0" height="416" style="position: absolute; left: 0px; width: 0px; height: 333px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="416" style="position: absolute; left: 0px; width: 0px; height: 333px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 8 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 64.515s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>&lt;ipython-input-17-fb85518531d7&gt;:15: SettingWithCopyWarning: 
A value is trying to be set on a copy of a slice from a DataFrame

See the caveats in the documentation: <a rel="nofollow" target="_blank" href="https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy">https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy</a>
  df.drop('language', axis=1, inplace=True)
</pre></div><div class="execute_result output_text"><pre>(1441, 8)</pre></div></div><div></div></colab-static-output-renderer></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-EEVTLXxFD9hC" tabindex="-1" role="region" aria-label="Cell 9: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1049.82s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Part&nbsp;2</span></span><br><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;spacy</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Parser</span></span><br><span><span class="mtk1">parser&nbsp;=&nbsp;en_core_sci_lg.load(disable=[</span><span class="mtk26">"tagger"</span><span class="mtk1">,&nbsp;</span><span class="mtk26">"ner"</span><span class="mtk1">])</span></span><br><span><span class="mtk1">parser.max_length&nbsp;=&nbsp;</span><span class="mtk12">2000000</span></span><br><span><span></span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">tokenize_text</span><span class="mtk1">(</span><span class="mtk16">text</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;doc&nbsp;=&nbsp;parser(text)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;[token.text&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;token&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;doc]</span></span><br><span><span></span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'tokens'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'body_text'</span><span class="mtk1">].apply(tokenize_text)</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 9 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1049.82s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>/usr/local/lib/python3.10/dist-packages/spacy/language.py:2195: FutureWarning: Possible set union at position 6328
  deserializers["tokenizer"] = lambda p: self.tokenizer.from_disk(  # type: ignore[union-attr]
/usr/local/lib/python3.10/dist-packages/spacy/pipeline/lemmatizer.py:211: UserWarning: [W108] The rule-based lemmatizer did not find POS annotation for one or more tokens. Check that your pipeline includes components that assign token.pos, typically 'tagger'+'attribute_ruler' or 'morphologizer'.
  warnings.warn(Warnings.W108)
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-AWL3iZ4_m2Go" tabindex="-1" role="region" aria-label="Cell 10: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.031s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df.shape</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 10 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.031s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="execute_result output_text"><pre>(1441, 9)</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-XIKnact1m3kS" tabindex="-1" role="region" aria-label="Cell 11: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1.083s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 11 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1.083s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div style=""><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe.html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-EVBoX_pDgeUI" tabindex="-1" role="region" aria-label="Cell 12: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 67.037s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Part&nbsp;3(stem)</span></span><br><span><span></span></span><br><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.stem&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;SnowballStemmer</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;nltk</span></span><br><span><span></span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'punkt'</span><span class="mtk1">)&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Download&nbsp;necessary&nbsp;resources&nbsp;for&nbsp;NLTK</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;SnowballStemmer&nbsp;for&nbsp;English</span></span><br><span><span class="mtk1">stemmer&nbsp;=&nbsp;SnowballStemmer(</span><span class="mtk26">"english"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Function&nbsp;to&nbsp;perform&nbsp;stemming&nbsp;on&nbsp;a&nbsp;text</span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">stem_text</span><span class="mtk1">(</span><span class="mtk16">words</span><span class="mtk1">):</span></span><br><span><span></span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Stem&nbsp;each&nbsp;word&nbsp;in&nbsp;the&nbsp;list&nbsp;of&nbsp;words</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;stemmed_words&nbsp;=&nbsp;[stemmer.stem(word)&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;word&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;words]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Join&nbsp;the&nbsp;stemmed&nbsp;words&nbsp;back&nbsp;into&nbsp;a&nbsp;single&nbsp;string</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;stemmed_text&nbsp;=&nbsp;</span><span class="mtk26">'&nbsp;'</span><span class="mtk1">.join(stemmed_words)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;stemmed_text</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Assuming&nbsp;'df'&nbsp;is&nbsp;your&nbsp;DataFrame&nbsp;with&nbsp;the&nbsp;text&nbsp;da</span><span class="mtk8">ta&nbsp;in&nbsp;the&nbsp;'body_text'&nbsp;column</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Apply&nbsp;stem_text&nbsp;function&nbsp;to&nbsp;stem&nbsp;the&nbsp;text&nbsp;in&nbsp;the</span><span class="mtk8">&nbsp;'body_text'&nbsp;column</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'stemmed_text'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'tokens'</span><span class="mtk1">].apply(stem_text)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Now&nbsp;the&nbsp;'body_text'&nbsp;column&nbsp;has&nbsp;been</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 12 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 67.037s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>[nltk_data] Downloading package punkt to /root/nltk_data...
[nltk_data]   Unzipping tokenizers/punkt.zip.
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-c5W3VhUgcegD" tabindex="-1" role="region" aria-label="Cell 13: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 167.156s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Part&nbsp;3(lem)</span></span><br><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.stem&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;SnowballStemmer</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.stem&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;WordNetLemmatizer</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;nltk</span></span><br><span><span></span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'punkt'</span><span class="mtk1">)&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Download&nbsp;necessary&nbsp;resources&nbsp;for&nbsp;NLTK</span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'wordnet'</span><span class="mtk1">)&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Download&nbsp;WordNet&nbsp;for&nbsp;lemmatization</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;SnowballStemmer&nbsp;for&nbsp;English</span></span><br><span><span class="mtk1">stemmer&nbsp;=&nbsp;SnowballStemmer(</span><span class="mtk26">"english"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;WordNetLemmatizer</span></span><br><span><span class="mtk1">lemmatizer&nbsp;=&nbsp;WordNetLemmatizer()</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Function&nbsp;to&nbsp;perform&nbsp;stemming&nbsp;and&nbsp;lemmatization&nbsp;o</span><span class="mtk8">n&nbsp;a&nbsp;text</span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">stem_and_lemmatize_text</span><span class="mtk1">(</span><span class="mtk16">words</span><span class="mtk1">):</span></span><br><span><span></span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Stem&nbsp;each&nbsp;word&nbsp;in&nbsp;the&nbsp;list&nbsp;of&nbsp;words</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;stemmed_words&nbsp;=&nbsp;[stemmer.stem(word)&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;word&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;words]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Lemmatize&nbsp;each&nbsp;word&nbsp;in&nbsp;the&nbsp;list&nbsp;of&nbsp;words</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;lemmatized_words&nbsp;=&nbsp;[lemmatizer.lemmatize(word)</span><span class="mtk1">&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;word&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;stemmed_words]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Join&nbsp;the&nbsp;lemmatized&nbsp;words&nbsp;back&nbsp;into&nbsp;a&nbsp;single&nbsp;str</span><span class="mtk8">ing</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;lemmatized_text&nbsp;=&nbsp;</span><span class="mtk26">'&nbsp;'</span><span class="mtk1">.join(lemmatized_words)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;lemmatized_text</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Assuming&nbsp;'df'&nbsp;is&nbsp;your&nbsp;DataFrame&nbsp;with&nbsp;the&nbsp;text&nbsp;da</span><span class="mtk8">ta&nbsp;in&nbsp;the&nbsp;'body_text'&nbsp;column</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Apply&nbsp;stem_and_lemmatize_text&nbsp;function&nbsp;to&nbsp;stem&nbsp;a</span><span class="mtk8">nd&nbsp;lemmatize&nbsp;the&nbsp;text&nbsp;in&nbsp;the&nbsp;'body_text'&nbsp;column</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'stemmed_and_lemmatized_text'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'stemmed_text'</span><span class="mtk1">].apply(stem_and_lemmatize_text)</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 13 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 167.156s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>[nltk_data] Downloading package punkt to /root/nltk_data...
[nltk_data]   Package punkt is already up-to-date!
[nltk_data] Downloading package wordnet to /root/nltk_data...
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-1DUFoBkOnsGw" tabindex="-1" role="region" aria-label="Cell 14: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.035s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df.shape</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 14 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.035s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="execute_result output_text"><pre>(1441, 11)</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-DBKlJ3wYnujW" tabindex="-1" role="region" aria-label="Cell 15: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 2.151s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 15 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 2.151s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(1).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-JUjAEQFEnzvr" tabindex="-1" role="region" aria-label="Cell 16: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Part&nbsp;4</span></span><br><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;nltk</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.corpus&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;stopwords</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.tokenize&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;word_tokenize</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.stem&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;SnowballStemmer</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;re</span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'punkt'</span><span class="mtk1">)</span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'stopwords'</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;SnowballStemmer&nbsp;for&nbsp;English</span></span><br><span><span class="mtk1">stemmer&nbsp;=&nbsp;SnowballStemmer(</span><span class="mtk26">"english"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Function&nbsp;to&nbsp;remove&nbsp;stopwords&nbsp;from&nbsp;a&nbsp;text</span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">remove_stopwords</span><span class="mtk1">(</span><span class="mtk16">text</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Tokenize&nbsp;the&nbsp;text&nbsp;into&nbsp;words</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;words&nbsp;=&nbsp;word_tokenize(text)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Remove&nbsp;stopwords&nbsp;from&nbsp;the&nbsp;list&nbsp;of&nbsp;words</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;filtered_words&nbsp;=&nbsp;[word&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;word&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;words&nbsp;</span><span class="mtk19">if</span><span class="mtk1">&nbsp;word.lower()&nbsp;</span><span class="mtk6">not</span><span class="mtk1">&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;stopwords.words(</span><span class="mtk26">'english'</span><span class="mtk1">)]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Join&nbsp;the&nbsp;filtered&nbsp;words&nbsp;back&nbsp;into&nbsp;a&nbsp;single&nbsp;strin</span><span class="mtk8">g</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;filtered_text&nbsp;=&nbsp;</span><span class="mtk26">'&nbsp;'</span><span class="mtk1">.join(filtered_words)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;filtered_text</span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">remove_numbers_and_punctuation</span><span class="mtk1">(</span><span class="mtk16">text</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;re.sub(r</span><span class="mtk26">'\d+|[^\w\s]'</span><span class="mtk1">,&nbsp;</span><span class="mtk26">''</span><span class="mtk1">,&nbsp;text)</span></span><br><span><span></span></span><br><span><span></span></span><br><span><span></span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">remove_short_words</span><span class="mtk1">(</span><span class="mtk16">text</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Create&nbsp;a&nbsp;regular&nbsp;expression&nbsp;pattern&nbsp;to&nbsp;match&nbsp;wor</span><span class="mtk8">ds&nbsp;with&nbsp;length&nbsp;smaller&nbsp;than&nbsp;2</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;pattern&nbsp;=&nbsp;r</span><span class="mtk26">'\b\w{2}\b'</span></span><br><span><span></span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Use&nbsp;re.sub()&nbsp;to&nbsp;replace&nbsp;the&nbsp;matched&nbsp;short&nbsp;words&nbsp;</span><span class="mtk8">with&nbsp;an&nbsp;empty&nbsp;string</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;re.sub(pattern,&nbsp;</span><span class="mtk26">''</span><span class="mtk1">,&nbsp;text)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Assuming&nbsp;'df'&nbsp;is&nbsp;your&nbsp;DataFrame&nbsp;with&nbsp;the&nbsp;text&nbsp;da</span><span class="mtk8">ta&nbsp;in&nbsp;the&nbsp;'stemmed_text'&nbsp;column</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Apply&nbsp;remove_stopwords&nbsp;function&nbsp;to&nbsp;remove&nbsp;stopwo</span><span class="mtk8">rds&nbsp;from&nbsp;the&nbsp;'stemmed_text'&nbsp;column</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'stemmed_text'</span><span class="mtk1">].apply(remove_numbers_and_punctuation)</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">]=df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">].apply(remove_short_words)</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">].apply(remove_stopwords)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Now&nbsp;the&nbsp;'stemmed_text'&nbsp;column&nbsp;has&nbsp;been&nbsp;processed</span><span class="mtk8">&nbsp;to&nbsp;remove&nbsp;stopwords&nbsp;and&nbsp;stored&nbsp;in&nbsp;the&nbsp;'processed_</span><span class="mtk8">text'&nbsp;column</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 16 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>[nltk_data] Downloading package punkt to /root/nltk_data...
[nltk_data]   Package punkt is already up-to-date!
[nltk_data] Downloading package stopwords to /root/nltk_data...
[nltk_data]   Unzipping corpora/stopwords.zip.
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-OROAlB5NodJ5" tabindex="-1" role="region" aria-label="Cell 17: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 17 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(2).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-O8LY73UForGm" tabindex="-1" role="region" aria-label="Cell 18: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Part&nbsp;5:</span></span><br><span><span></span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;pandas&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;pd</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;nltk</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.corpus&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;stopwords</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.tokenize&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;word_tokenize</span></span><br><span><span class="mtk19">from</span><span class="mtk1">&nbsp;nltk.stem&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;SnowballStemmer</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;string</span></span><br><span><span></span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'punkt'</span><span class="mtk1">)</span></span><br><span><span class="mtk1">nltk.download(</span><span class="mtk26">'stopwords'</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;SnowballStemmer&nbsp;for&nbsp;English</span></span><br><span><span class="mtk1">stemmer&nbsp;=&nbsp;SnowballStemmer(</span><span class="mtk26">"english"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">remove_punctuation</span><span class="mtk1">(</span><span class="mtk16">text</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Define&nbsp;a&nbsp;set&nbsp;of&nbsp;punctuation&nbsp;marks</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;punctuation_set&nbsp;=&nbsp;</span><span class="mtk14">set</span><span class="mtk1">(string.punctuation)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Remove&nbsp;punctuation&nbsp;marks&nbsp;from&nbsp;the&nbsp;text</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;text_no_punctuation&nbsp;=&nbsp;</span><span class="mtk26">''</span><span class="mtk1">.join(char&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;char&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;text&nbsp;</span><span class="mtk19">if</span><span class="mtk1">&nbsp;char&nbsp;</span><span class="mtk6">not</span><span class="mtk1">&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;punctuation_set&nbsp;</span><span class="mtk6">and</span><span class="mtk1">&nbsp;</span><span class="mtk6">not</span><span class="mtk1">&nbsp;char.isdigit())</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;text_no_punctuation</span></span><br><span><span></span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Assuming&nbsp;'df'&nbsp;is&nbsp;your&nbsp;DataFrame&nbsp;with&nbsp;the&nbsp;text&nbsp;da</span><span class="mtk8">ta&nbsp;in&nbsp;the&nbsp;'processed_text'&nbsp;column</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Apply&nbsp;remove_punctuation&nbsp;function&nbsp;to&nbsp;remove&nbsp;punc</span><span class="mtk8">tuation&nbsp;marks&nbsp;from&nbsp;the&nbsp;'processed_text'&nbsp;column</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'clean_text'</span><span class="mtk1">]&nbsp;=&nbsp;df[</span><span class="mtk26">'processed_text'</span><span class="mtk1">].apply(remove_punctuation)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Now&nbsp;the&nbsp;'processed_text'&nbsp;column&nbsp;has&nbsp;been&nbsp;process</span><span class="mtk8">ed&nbsp;to&nbsp;remove&nbsp;punctuation&nbsp;marks&nbsp;and&nbsp;stored&nbsp;in&nbsp;the&nbsp;'</span><span class="mtk8">clean_text'&nbsp;column</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 18 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>[nltk_data] Downloading package punkt to /root/nltk_data...
[nltk_data]   Package punkt is already up-to-date!
[nltk_data] Downloading package stopwords to /root/nltk_data...
[nltk_data]   Package stopwords is already up-to-date!
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-X3YNVTZEo6gj" tabindex="-1" role="region" aria-label="Cell 19: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 19 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(3).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-KDBjKgPNrRaQ" tabindex="-1" role="region" aria-label="Cell 20: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df.drop(</span><span class="mtk26">'tokens'</span><span class="mtk1">,&nbsp;axis=</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;inplace=</span><span class="mtk6">True</span><span class="mtk1">)</span></span><br><span><span class="mtk1">df.drop(</span><span class="mtk26">'stemmed_text'</span><span class="mtk1">,&nbsp;axis=</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;inplace=</span><span class="mtk6">True</span><span class="mtk1">)</span></span><br><span><span class="mtk1">df.drop(</span><span class="mtk26">'processed_text'</span><span class="mtk1">,&nbsp;axis=</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;inplace=</span><span class="mtk6">True</span><span class="mtk1">)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 20 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-R03Cpw6SrlgN" tabindex="-1" role="region" aria-label="Cell 21: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 21 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(4).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-bnzpP2cW7Q2z" tabindex="-1" role="region" aria-label="Cell 22: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.feature_extraction.text&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;TfidfVectorizer</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;TfidfVectorizer&nbsp;with&nbsp;maximum&nbsp;of&nbsp;4096&nbsp;</span><span class="mtk8">features</span></span><br><span><span class="mtk1">tfidf_vectorizer&nbsp;=&nbsp;TfidfVectorizer(max_features=</span><span class="mtk12">4096</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Fit&nbsp;and&nbsp;transform&nbsp;the&nbsp;preprocessed&nbsp;text&nbsp;data&nbsp;to&nbsp;</span><span class="mtk8">obtain&nbsp;TF-IDF&nbsp;features</span></span><br><span><span class="mtk1">tfidf_features&nbsp;=&nbsp;tfidf_vectorizer.fit_transform(df</span><span class="mtk1">[</span><span class="mtk26">'clean_text'</span><span class="mtk1">])</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Convert&nbsp;TF-IDF&nbsp;features&nbsp;to&nbsp;a&nbsp;dense&nbsp;matrix</span></span><br><span><span class="mtk1">tfidf_features_dense&nbsp;=&nbsp;tfidf_features.toarray()</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Convert&nbsp;the&nbsp;dense&nbsp;matrix&nbsp;to&nbsp;DataFrame</span></span><br><span><span class="mtk1">tfidf_df&nbsp;=&nbsp;pd.DataFrame(tfidf_features_dense,&nbsp;colu</span><span class="mtk1">mns=tfidf_vectorizer.get_feature_names_out())</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Now&nbsp;tfidf_df&nbsp;contains&nbsp;TF-IDF&nbsp;features&nbsp;for&nbsp;each&nbsp;d</span><span class="mtk8">ocument</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 22 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-bOR-uIYssGcd" tabindex="-1" role="region" aria-label="Cell 23: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">tfidf_df.shape</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 23 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="execute_result output_text"><pre>(1441, 4096)</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-7nTtZzUzsTK-" tabindex="-1" role="region" aria-label="Cell 24: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">tfidf_df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 24 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 423px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(5).html" class="" style="height: 423px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <div class="add-cell-buttons">
        <md-outlined-button class="add-code add-button" aria-label="Add code cell
Ctrl+M B" title="Add code cell
Ctrl+M B" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add code cell
Ctrl+M B">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Code
        </md-outlined-button>
        <md-outlined-button class="add-text add-button" aria-label="Add text cell" title="Add text cell" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$--><div class="outline"></div>
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button" aria-label="Add text cell">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>add</md-icon>
          <!--?lit$944599098$-->Text
        </md-outlined-button>
        <!--?lit$944599098$-->
      </div><hr>
    </div></div><div class="cell code icon-scrolling" id="cell-Nn7maPOiEen9" tabindex="-1" role="region" aria-label="Cell 25: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="25" data-mode-id="notebook-python" style="height: 485px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs" role="code" data-uri="inmemory://model/36" style="width: 1411px; height: 485px;"><div data-mprt="3" class="overflow-guard" style="width: 1411px; height: 485px;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 485px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 485px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 485px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1405px; height: 485px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 485px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1405px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1405px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 485px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1405px; height: 485px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.decomposition&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;PCA</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Initialize&nbsp;PCA&nbsp;with&nbsp;n_components=None&nbsp;to&nbsp;keep&nbsp;al</span><span class="mtk8">l&nbsp;principal&nbsp;components</span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk1">pca&nbsp;=&nbsp;PCA</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">n_components=</span><span class="mtk6">None</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Fit&nbsp;PCA&nbsp;to&nbsp;TF-IDF&nbsp;features</span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk1">pca.fit</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_dense</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Calculate&nbsp;the&nbsp;cumulative&nbsp;sum&nbsp;of&nbsp;explained&nbsp;varian</span><span class="mtk8">ce&nbsp;ratio</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">cumulative_variance_ratio&nbsp;=&nbsp;pca.explained_variance</span><span class="mtk1">_ratio_.cumsum</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Determine&nbsp;the&nbsp;number&nbsp;of&nbsp;components&nbsp;required&nbsp;to&nbsp;p</span><span class="mtk8">reserve&nbsp;95%&nbsp;of&nbsp;variance</span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">n_components&nbsp;=&nbsp;</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">cumulative_variance_ratio&nbsp;&lt;=&nbsp;</span><span class="mtk12">0.95</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">.</span><span class="mtk15">sum</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Initialize&nbsp;PCA&nbsp;with&nbsp;the&nbsp;determined&nbsp;number&nbsp;of&nbsp;com</span><span class="mtk8">ponents</span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk1">pca&nbsp;=&nbsp;PCA</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">n_components=n_components</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:323px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Fit&nbsp;PCA&nbsp;again&nbsp;to&nbsp;TF-IDF&nbsp;features</span></span></div><div style="top:342px;height:19px;" class="view-line"><span><span class="mtk1">pca.fit</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_dense</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:361px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:380px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Transform&nbsp;the&nbsp;TF-IDF&nbsp;features&nbsp;to&nbsp;the&nbsp;reduced&nbsp;dim</span><span class="mtk8">ensionality</span></span></div><div style="top:399px;height:19px;" class="view-line"><span><span class="mtk1">tfidf_features_reduced&nbsp;=&nbsp;pca.transform</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_dense</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:418px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:437px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Now&nbsp;tfidf_features_reduced&nbsp;contains&nbsp;TF-IDF&nbsp;featu</span><span class="mtk8">res&nbsp;reduced&nbsp;with&nbsp;PCA&nbsp;while&nbsp;preserving&nbsp;95%&nbsp;of&nbsp;varia</span><span class="mtk8">nce</span></span></div><div style="top:456px;height:19px;" class="view-line"><span><span></span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute; width: 1391px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1391px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="606" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 485px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 485px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 485px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1411px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 1411px; height: 1px;"></textarea><div style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;" class="monaco-editor-background textAreaCover"></div><div data-mprt="4" class="overlayWidgets" style="width: 1411px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 485px;"><div class="minimap-shadow-hidden" style="height: 485px;"></div><canvas width="0" height="606" style="position: absolute; left: 0px; width: 0px; height: 485px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="606" style="position: absolute; left: 0px; width: 0px; height: 485px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 931.26px; max-height: 250px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 25 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-z7M8w-uK7f5U" tabindex="-1" role="region" aria-label="Cell 26: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">tfidf_features_reduced.shape</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 26 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="execute_result output_text"><pre>(1441, 963)</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-YBbS0xDQImlm" tabindex="-1" role="region" aria-label="Cell 27: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">tfidf_features_reduced=pd.DataFrame(tfidf_features</span><span class="mtk1">_reduced)</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 27 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-lQlpgvjtPCtV" tabindex="-1" role="region" aria-label="Cell 28: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed at unknown time" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">tfidf_features_reduced</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 28 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed at unknown time"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div class="outputview" style="height: 443px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(6).html" class="" style="height: 443px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-yllwsZlaJKCD" tabindex="-1" role="region" aria-label="Cell 29: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 62.501s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="34" data-mode-id="notebook-python" style="height: 523px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs" role="code" data-uri="inmemory://model/41" style="width: 1411px; height: 523px;"><div data-mprt="3" class="overflow-guard" style="width: 1411px; height: 523px;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 523px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 523px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 523px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1405px; height: 523px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 523px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1405px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1405px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 523px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1405px; height: 523px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.cluster&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;KMeans</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span class="mtk19">import</span><span class="mtk1">&nbsp;matplotlib.pyplot&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;plt</span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Assuming&nbsp;you&nbsp;have&nbsp;already&nbsp;computed&nbsp;tfidf_feature</span><span class="mtk8">s_reduced&nbsp;and&nbsp;have&nbsp;a&nbsp;DataFrame&nbsp;'df'&nbsp;containing&nbsp;you</span><span class="mtk8">r&nbsp;data</span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Apply&nbsp;K-Means&nbsp;clustering&nbsp;with&nbsp;Elbow&nbsp;Method</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span class="mtk1">distortions&nbsp;=&nbsp;</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">max_clusters&nbsp;=&nbsp;</span><span class="mtk12">30</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Maximum&nbsp;number&nbsp;of&nbsp;clusters&nbsp;to&nbsp;consider</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span class="mtk19">for</span><span class="mtk1">&nbsp;i&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;</span><span class="mtk15">range</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;max_clusters&nbsp;+&nbsp;</span><span class="mtk12">1</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">:</span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;kmeans&nbsp;=&nbsp;KMeans</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">n_clusters=i,&nbsp;random_state=</span><span class="mtk12">400</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;kmeans.fit</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_reduced</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;distortions.append</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">kmeans.inertia_</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Plot&nbsp;Elbow&nbsp;Method&nbsp;curve</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk12">10</span><span class="mtk1">,&nbsp;</span><span class="mtk12">6</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:323px;height:19px;" class="view-line"><span><span class="mtk1">plt.plot</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk15">range</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;max_clusters&nbsp;+&nbsp;</span><span class="mtk12">1</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,&nbsp;distortions,&nbsp;marker=</span><span class="mtk26">'o'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:342px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'Elbow&nbsp;Method&nbsp;for&nbsp;Optimal&nbsp;K'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:361px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'Number&nbsp;of&nbsp;Clusters'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:380px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'Distortion'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:399px;height:19px;" class="view-line"><span><span class="mtk1">plt.xticks</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk15">range</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;max_clusters&nbsp;+&nbsp;</span><span class="mtk12">1</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:418px;height:19px;" class="view-line"><span><span class="mtk1">plt.grid</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk6">True</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:437px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:456px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:475px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:494px;height:19px;" class="view-line"><span><span></span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute; width: 1391px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1391px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="653" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 523px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 523px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 523px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1411px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 1411px; height: 1px;"></textarea><div style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;" class="monaco-editor-background textAreaCover"></div><div data-mprt="4" class="overlayWidgets" style="width: 1411px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 523px;"><div class="minimap-shadow-hidden" style="height: 523px;"></div><canvas width="0" height="653" style="position: absolute; left: 0px; width: 0px; height: 523px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="653" style="position: absolute; left: 0px; width: 0px; height: 523px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 931.26px; max-height: 250px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 29 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 62.501s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div style=""><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(7).html" class="" style="height: 1000px;"></iframe></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-690d_Stee3rZ" tabindex="-1" role="region" aria-label="Cell 30: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 3.801s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk8">#&nbsp;Choose&nbsp;the&nbsp;optimal&nbsp;number&nbsp;of&nbsp;clusters&nbsp;based&nbsp;on&nbsp;t</span><span class="mtk8">he&nbsp;Elbow&nbsp;Method</span></span><br><span><span class="mtk1">optimal_k&nbsp;=&nbsp;</span><span class="mtk12">16</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Assuming&nbsp;the&nbsp;optimal&nbsp;number&nbsp;of&nbsp;clusters&nbsp;is&nbsp;5&nbsp;bas</span><span class="mtk8">ed&nbsp;on&nbsp;the&nbsp;Elbow&nbsp;Method</span></span><br><span><span class="mtk8">#&nbsp;Apply&nbsp;K-Means&nbsp;clustering&nbsp;with&nbsp;the&nbsp;optimal&nbsp;number</span><span class="mtk8">&nbsp;of&nbsp;clusters</span></span><br><span><span class="mtk1">kmeans&nbsp;=&nbsp;KMeans(n_clusters=optimal_k,&nbsp;random_state</span><span class="mtk1">=</span><span class="mtk12">42</span><span class="mtk1">)</span></span><br><span><span class="mtk1">kmeans.fit(tfidf_features_reduced)</span></span><br><span><span class="mtk8">#&nbsp;Get&nbsp;the&nbsp;cluster&nbsp;labels</span></span><br><span><span class="mtk1">cluster_labels&nbsp;=&nbsp;kmeans.labels_</span></span><br><span><span class="mtk8">#&nbsp;Add&nbsp;cluster&nbsp;labels&nbsp;to&nbsp;the&nbsp;DataFrame</span></span><br><span><span class="mtk1">df[</span><span class="mtk26">'cluster'</span><span class="mtk1">]&nbsp;=&nbsp;cluster_labels</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 30 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 3.801s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>/usr/local/lib/python3.10/dist-packages/sklearn/cluster/_kmeans.py:870: FutureWarning: The default value of `n_init` will change from 10 to 'auto' in 1.4. Set the value of `n_init` explicitly to suppress the warning
  warnings.warn(
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-4M3G8sJFghvp" tabindex="-1" role="region" aria-label="Cell 31: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.525s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.metrics&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;silhouette_score,&nbsp;davies_bouldin_score</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Silhouette&nbsp;Score</span></span><br><span><span class="mtk1">silhouette&nbsp;=&nbsp;silhouette_score(tfidf_features_reduc</span><span class="mtk1">ed,&nbsp;cluster_labels)</span></span><br><span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Silhouette&nbsp;Score:&nbsp;</span><span class="mtk1">{silhouette}</span><span class="mtk26">"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Davies-Bouldin&nbsp;Index</span></span><br><span><span class="mtk1">davies_bouldin&nbsp;=&nbsp;davies_bouldin_score(tfidf_featur</span><span class="mtk1">es_reduced,&nbsp;cluster_labels)</span></span><br><span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Davies-Bouldin&nbsp;Index:&nbsp;</span><span class="mtk1">{davies_bouldin}</span><span class="mtk26">"</span><span class="mtk1">)</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 31 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.525s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>Silhouette Score: 0.026219904154234835
Davies-Bouldin Index: 4.9101509932479885
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-1cHMpnjfYHu-" tabindex="-1" role="region" aria-label="Cell 32: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.cluster&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;DBSCAN</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;DBSCAN&nbsp;with&nbsp;parameters</span></span><br><span><span class="mtk1">dbscan&nbsp;=&nbsp;DBSCAN(eps=</span><span class="mtk12">1</span><span class="mtk1">,&nbsp;min_samples=</span><span class="mtk12">10</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Fit&nbsp;DBSCAN&nbsp;to&nbsp;TF-IDF&nbsp;features</span></span><br><span><span class="mtk1">dbscan.fit(tfidf_features_reduced)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Get&nbsp;the&nbsp;cluster&nbsp;labels</span></span><br><span><span class="mtk1">cluster_labels_1&nbsp;=&nbsp;dbscan.labels_</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Add&nbsp;cluster&nbsp;labels&nbsp;to&nbsp;the&nbsp;DataFrame</span></span><br><span><span class="mtk8">#&nbsp;df['DB_cluster']&nbsp;=&nbsp;cluster_labels_1</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 32 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-crIEVfbbYlbn" tabindex="-1" role="region" aria-label="Cell 33: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.395s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.metrics&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;silhouette_score,&nbsp;davies_bouldin_score</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Silhouette&nbsp;Score</span></span><br><span><span class="mtk1">silhouette&nbsp;=&nbsp;silhouette_score(tfidf_features_reduc</span><span class="mtk1">ed,&nbsp;cluster_labels_1)</span></span><br><span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Silhouette&nbsp;Score:&nbsp;</span><span class="mtk1">{silhouette}</span><span class="mtk26">"</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Davies-Bouldin&nbsp;Index</span></span><br><span><span class="mtk1">davies_bouldin&nbsp;=&nbsp;davies_bouldin_score(tfidf_featur</span><span class="mtk1">es_reduced,&nbsp;cluster_labels_1)</span></span><br><span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Davies-Bouldin&nbsp;Index:&nbsp;</span><span class="mtk1">{davies_bouldin}</span><span class="mtk26">"</span><span class="mtk1">)</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 33 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 0.395s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>Silhouette Score: -0.008425072491723059
Davies-Bouldin Index: 5.2424066400924705
</pre></div></div><div></div></colab-static-output-renderer></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-liPOnsWC74j3" tabindex="-1" role="region" aria-label="Cell 34: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 3.156s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk1">df</span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 34 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 3.156s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div style=""><div class="outputview" style="height: 1000px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(8).html" class="" style="height: 1000px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling focused" id="cell-ZMLknF7HJ1qH" tabindex="-1" role="region" aria-label="Cell 35: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"><colab-cell-toolbar><template shadowrootmode="open"><!----><!--?lit$944599098$--><!----> <md-icon-button class="colab-icon" title="Move cell up
Ctrl+M K" aria-label="Move cell up
Ctrl+M K" command="move-cell-up" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Move cell up
Ctrl+M K">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->arrow_upward</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Move cell down
Ctrl+M J" aria-label="Move cell down
Ctrl+M J" command="move-cell-down" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Move cell down
Ctrl+M J">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->arrow_downward</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Copy link to cell" aria-label="Copy link to cell" command="copy-link-to-cell" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Copy link to cell">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->link</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Add a comment
Ctrl+Alt+M" aria-label="Add a comment
Ctrl+Alt+M" command="add-comment" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Add a comment
Ctrl+Alt+M">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->comment</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Open editor settings" aria-label="Open editor settings" command="editor-preferences" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Open editor settings">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->settings</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Edit" aria-label="Edit" command="toggle-edit-markdown" toggle="" role="presentation" style="display: none;" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Edit" aria-pressed="false">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->edit</md-icon>
          <!--?lit$944599098$--><md-icon slot="selected" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->edit_off</md-icon>
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Mirror cell in tab" aria-label="Mirror cell in tab" command="mirror-cell-in-tab" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Mirror cell in tab">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$-->
      <g id="mirror-cell">
        <path d="M4,21V7H2V21a2,2,0,0,0,2,2H18V21Z"></path>
        <path d="M6,13v2H8.6L5,18.6,6.4,20,10,16.4V19h2V13Z"></path>
        <path d="M19,1H8A2,2,0,0,0,6,3v8H8V3H19V17H14v2h5a2,2,0,0,0,2-2V3A2,2,0,0,0,19,1Z"></path>
      </g></svg></md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!----> <md-icon-button class="colab-icon" title="Delete cell
Ctrl+M D" aria-label="Delete cell
Ctrl+M D" command="delete-cell-or-selection" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Delete cell
Ctrl+M D">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface"></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
          <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->delete</md-icon>
          <!--?lit$944599098$-->
        </md-icon-button><!----><!--?lit$944599098$--><md-icon-button title="More cell actions" aria-label="More cell actions" class="colab-icon cell-toolbar-more" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="More cell actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_vert</md-icon>
    </md-icon-button><!--?--></template></colab-cell-toolbar></div><div class="main-content" elevation="2"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 17.3s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale focused">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="41" data-mode-id="notebook-python" style="height: 428px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs" role="code" data-uri="inmemory://model/48" style="width: 1411px; height: 428px;"><div data-mprt="3" class="overflow-guard" style="width: 1411px; height: 428px;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 428px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 428px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 428px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1405px; height: 428px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 428px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1405px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1405px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 428px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1405px; height: 428px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.manifold&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;TSNE</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span class="mtk19">import</span><span class="mtk1">&nbsp;seaborn&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;sns</span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Apply&nbsp;t-SNE&nbsp;to&nbsp;reduce&nbsp;the&nbsp;dimensionality&nbsp;of&nbsp;TF-I</span><span class="mtk8">DF&nbsp;features&nbsp;to&nbsp;2D</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span class="mtk1">tsne&nbsp;=&nbsp;TSNE</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">n_components=</span><span class="mtk12">2</span><span class="mtk1">,&nbsp;random_state=</span><span class="mtk12">42</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span class="mtk1">tfidf_features_2d&nbsp;=&nbsp;tsne.fit_transform</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_dense</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Convert&nbsp;the&nbsp;2D&nbsp;features&nbsp;to&nbsp;DataFrame</span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">tfidf_features_2d_df&nbsp;=&nbsp;pd.DataFrame</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">tfidf_features_2d,&nbsp;columns=</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1">,&nbsp;</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">&nbsp;=&nbsp;tfidf_features_2d_df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">&nbsp;=&nbsp;tfidf_features_2d_df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Add&nbsp;cluster&nbsp;labels&nbsp;to&nbsp;the&nbsp;DataFrame</span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">tfidf_features_2d_df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'cluster'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">&nbsp;=&nbsp;cluster_labels</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span class="mtk8">#&nbsp;Plot&nbsp;the&nbsp;scatterplot&nbsp;with&nbsp;different&nbsp;colors&nbsp;for&nbsp;d</span><span class="mtk8">ifferent&nbsp;clusters</span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk1">plt.figure</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">figsize=</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk12">10</span><span class="mtk1">,&nbsp;</span><span class="mtk12">6</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">sns.scatterplot</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">x=</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1">,&nbsp;y=</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1">,&nbsp;hue=</span><span class="mtk26">'cluster'</span><span class="mtk1">,&nbsp;data=tfidf_features_2d_df,&nbsp;palette=</span><span class="mtk26">'viridis'</span><span class="mtk1">,&nbsp;legend=</span><span class="mtk26">'full'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:323px;height:19px;" class="view-line"><span><span class="mtk1">plt.title</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'t-SNE&nbsp;Visualization&nbsp;of&nbsp;TF-IDF&nbsp;Features&nbsp;with&nbsp;Clust</span><span class="mtk26">er&nbsp;Labels'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:342px;height:19px;" class="view-line"><span><span class="mtk1">plt.xlabel</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:361px;height:19px;" class="view-line"><span><span class="mtk1">plt.ylabel</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:380px;height:19px;" class="view-line"><span><span class="mtk1">plt.legend</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">title=</span><span class="mtk26">'Cluster'</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:399px;height:19px;" class="view-line"><span><span class="mtk1">plt.show</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute; width: 1391px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1391px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="535" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 428px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 428px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 428px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1411px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 1411px; height: 1px;"></textarea><div style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;" class="monaco-editor-background textAreaCover"></div><div data-mprt="4" class="overlayWidgets" style="width: 1411px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 428px;"><div class="minimap-shadow-hidden" style="height: 428px;"></div><canvas width="0" height="535" style="position: absolute; left: 0px; width: 0px; height: 428px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="535" style="position: absolute; left: 0px; width: 0px; height: 428px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 931.26px; max-height: 250px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 35 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 17.3s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div style=""><div class="outputview" style="height: 550px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(9).html" class="" style="height: 550px;"></iframe></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-By4_qAM_C_p0" tabindex="-1" role="region" aria-label="Cell 36: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 14.579s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span class="mtk19">from</span><span class="mtk1">&nbsp;sklearn.decomposition&nbsp;</span><span class="mtk19">import</span><span class="mtk1">&nbsp;LatentDirichletAllocation</span></span><br><span><span class="mtk19">import</span><span class="mtk1">&nbsp;numpy&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;np</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Number&nbsp;of&nbsp;topics&nbsp;to&nbsp;extract&nbsp;(can&nbsp;be&nbsp;adjusted)</span></span><br><span><span class="mtk1">num_topics&nbsp;=&nbsp;</span><span class="mtk12">5</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Initialize&nbsp;LDA&nbsp;model</span></span><br><span><span class="mtk1">lda&nbsp;=&nbsp;LatentDirichletAllocation(n_components=num_t</span><span class="mtk1">opics,&nbsp;random_state=</span><span class="mtk12">42</span><span class="mtk1">)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Fit&nbsp;LDA&nbsp;model&nbsp;to&nbsp;TF-IDF&nbsp;features</span></span><br><span><span class="mtk1">lda.fit(tfidf_features_dense)</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Get&nbsp;the&nbsp;top&nbsp;words&nbsp;for&nbsp;each&nbsp;topic</span></span><br><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">get_top_words</span><span class="mtk1">(</span><span class="mtk16">lda_model</span><span class="mtk1">,&nbsp;</span><span class="mtk16">feature_names</span><span class="mtk1">,&nbsp;</span><span class="mtk16">num_words</span><span class="mtk1">=</span><span class="mtk12">10</span><span class="mtk1">):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;top_words&nbsp;=&nbsp;[]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;topic_weights&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;lda_model.components_:</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;top_word_indices&nbsp;=&nbsp;topic_weights.argsort()</span><span class="mtk1">[-num_words:][::</span><span class="mtk12">-1</span><span class="mtk1">]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;top_words.append([feature_names[i]&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;i&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;top_word_indices])</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">return</span><span class="mtk1">&nbsp;top_words</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Get&nbsp;feature&nbsp;names&nbsp;from&nbsp;TfidfVectorizer</span></span><br><span><span class="mtk1">feature_names&nbsp;=&nbsp;tfidf_vectorizer.get_feature_names</span><span class="mtk1">_out()</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Print&nbsp;top&nbsp;words&nbsp;for&nbsp;each&nbsp;topic&nbsp;in&nbsp;each&nbsp;cluster</span></span><br><span><span class="mtk19">for</span><span class="mtk1">&nbsp;cluster_id&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;</span><span class="mtk15">range</span><span class="mtk1">(optimal_k):&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;assuming&nbsp;optimal_k&nbsp;is&nbsp;the&nbsp;number&nbsp;of&nbsp;clusters</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Cluster&nbsp;</span><span class="mtk1">{cluster_id&nbsp;+&nbsp;</span><span class="mtk12">1</span><span class="mtk1">}</span><span class="mtk26">:"</span><span class="mtk1">)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;cluster_tfidf_features&nbsp;=&nbsp;tfidf_features_dense[</span><span class="mtk1">df[</span><span class="mtk26">'cluster'</span><span class="mtk1">]&nbsp;==&nbsp;cluster_id]</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;lda.fit(cluster_tfidf_features)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;top_words&nbsp;=&nbsp;get_top_words(lda,&nbsp;feature_names)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;i,&nbsp;words&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;</span><span class="mtk15">enumerate</span><span class="mtk1">(top_words):</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk15">print</span><span class="mtk1">(</span><span class="mtk6">f</span><span class="mtk26">"Topic&nbsp;</span><span class="mtk1">{i&nbsp;+&nbsp;</span><span class="mtk12">1</span><span class="mtk1">}</span><span class="mtk26">:&nbsp;</span><span class="mtk1">{</span><span class="mtk26">',&nbsp;'</span><span class="mtk1">.join(words)}</span><span class="mtk26">"</span><span class="mtk1">)</span></span><br><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk15">print</span><span class="mtk1">()</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 36 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 14.579s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div><div><colab-static-output-renderer tabindex="0" role="group"><div><div class="stream output_text"><pre>Cluster 1:
Topic 1: tcid, mef, passeng, ntr, plasmid, spin, roch, covari, qpcr, sas
Topic 2: tcid, mef, passeng, ntr, plasmid, spin, roch, covari, qpcr, sas
Topic 3: children, virus, infect, influenza, rsv, respiratori, patient, pneumonia, studi, case
Topic 4: tcid, mef, passeng, ntr, plasmid, spin, roch, covari, qpcr, sas
Topic 5: tcid, mef, passeng, ntr, plasmid, spin, roch, covari, qpcr, sas

Cluster 2:
Topic 1: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 2: lncrnas, cis, utr, noncod, rnas, outdoor, neighbor, nest, enforc, pol
Topic 3: cell, mice, express, immun, respons, activ, infect, ace, lung, cytokin
Topic 4: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 5: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo

Cluster 3:
Topic 1: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 2: sirna, pdcov, knockdown, rnai, silenc, appendix, mainland, los, stream, organell
Topic 3: sequenc, genom, virus, use, rna, sampl, gene, assay, primer, strain
Topic 4: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 5: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag

Cluster 4:
Topic 1: trauma, ago, occasion, pancreat, ecolog, attenu, decontamin, bacteriophag, inocul, deform
Topic 2: trauma, ago, occasion, pancreat, ecolog, attenu, decontamin, bacteriophag, inocul, deform
Topic 3: trauma, ago, occasion, pancreat, ecolog, attenu, decontamin, bacteriophag, inocul, deform
Topic 4: trauma, ago, occasion, pancreat, ecolog, attenu, decontamin, bacteriophag, inocul, deform
Topic 5: preprint, medrxiv, licens, authorfund, covid, perpetu, holder, copyright, grant, patient

Cluster 5:
Topic 1: hcwes, oac, huvec, icp, ifitm, sia, oacetyl, bcov, mucus, heparin
Topic 2: huvec, oac, hcwes, icp, curat, oacetyl, ifitm, vap, confus, french
Topic 3: huvec, oac, hcwes, icp, curat, oacetyl, ifitm, vap, confus, french
Topic 4: huvec, oac, hcwes, icp, curat, oacetyl, ifitm, vap, confus, french
Topic 5: cell, virus, infect, protein, viral, replic, nsp, rna, use, activ

Cluster 6:
Topic 1: adam, fipv, hsct, readi, hai, cotton, ncov, ndv, neighborhood, prematur
Topic 2: protein, cell, sarscov, peptid, epitop, bind, sequenc, use, express, vaccin
Topic 3: adam, fipv, hsct, readi, hai, cotton, ncov, ndv, neighborhood, prematur
Topic 4: adam, fipv, hsct, readi, hai, cotton, ncov, ndv, neighborhood, prematur
Topic 5: adam, fipv, hsct, readi, hai, cotton, ncov, ndv, neighborhood, prematur

Cluster 7:
Topic 1: formula, locus, null, unstabl, circular, chamber, nonlinear, assign, mismatch, geometr
Topic 2: diseas, health, human, infect, virus, anim, pathogen, outbreak, emerg, popul
Topic 3: formula, locus, null, unstabl, circular, chamber, nonlinear, assign, mismatch, geometr
Topic 4: formula, locus, null, unstabl, circular, chamber, nonlinear, assign, mismatch, geometr
Topic 5: formula, locus, null, unstabl, circular, chamber, nonlinear, assign, mismatch, geometr

Cluster 8:
Topic 1: string, overlap, algorithm, row, bound, compress, length, comput, lower, border
Topic 2: markov, intervent, merscov, state, seir, simul, equat, index, step, korea
Topic 3: languag, theorem, let, proof, stochast, finit, slide, geometr, model, equat
Topic 4: fraction, root, equat, stabil, theorem, system, condit, satisfi, equilibrium, model
Topic 5: string, code, problem, symbol, embed, complex, algorithm, solut, dataset, use

Cluster 9:
Topic 1: astrovirus, profit, atg, macaqu, tcid, camel, dispar, doi, infer, genbank
Topic 2: astrovirus, profit, atg, macaqu, tcid, camel, dispar, doi, infer, genbank
Topic 3: patient, infect, pneumonia, studi, day, therapi, clinic, use, treatment, diseas
Topic 4: astrovirus, profit, atg, macaqu, tcid, camel, dispar, doi, infer, genbank
Topic 5: astrovirus, profit, atg, macaqu, tcid, camel, dispar, doi, infer, genbank

Cluster 10:
Topic 1: ventil, hospitalis, dilat, downstream, inpati, exit, zhang, sent, frame, ineffect
Topic 2: ventil, hospitalis, dilat, downstream, inpati, exit, zhang, sent, frame, ineffect
Topic 3: model, infect, network, case, epidem, estim, number, node, data, paramet
Topic 4: ventil, hospitalis, dilat, downstream, inpati, exit, zhang, sent, frame, ineffect
Topic 5: ventil, hospitalis, dilat, downstream, inpati, exit, zhang, sent, frame, ineffect

Cluster 11:
Topic 1: albeit, huang, code, singapor, recal, causal, press, clade, workplac, frozen
Topic 2: covid, patient, sarscov, case, infect, hospit, treatment, diseas, clinic, symptom
Topic 3: albeit, huang, code, singapor, recal, causal, press, clade, workplac, frozen
Topic 4: albeit, huang, code, singapor, recal, causal, press, clade, workplac, frozen
Topic 5: albeit, huang, code, singapor, recal, causal, press, clade, workplac, frozen

Cluster 12:
Topic 1: coloni, odd, drop, immunoassay, regress, belong, relationship, statist, random, composit
Topic 2: calv, herd, calf, milk, rotavirus, cow, sampl, diarrhea, vaccin, dairi
Topic 3: coloni, odd, drop, immunoassay, regress, belong, relationship, statist, random, composit
Topic 4: coloni, odd, drop, immunoassay, regress, belong, relationship, statist, random, composit
Topic 5: coloni, odd, drop, immunoassay, regress, belong, relationship, statist, random, composit

Cluster 13:
Topic 1: deplet, hospitalis, faecal, nurs, ifnγ, nos, speed, pbmc, home, messag
Topic 2: cat, felin, fip, dog, fiv, infect, fcov, fecv, diseas, fipv
Topic 3: deplet, hospitalis, faecal, ifnγ, nurs, nos, speed, pbmc, home, messag
Topic 4: deplet, hospitalis, faecal, nurs, ifnγ, nos, speed, pbmc, home, messag
Topic 5: deplet, hospitalis, faecal, ifnγ, nurs, nos, speed, pbmc, home, messag

Cluster 14:
Topic 1: bst, hpiv, evg, cvb, pomegran, eifα, torovirus, ectodomain, btamir, cpe
Topic 2: rvi, dmi, circrna, arl, tcdc, atrh, lozeng, alibaba, izn, legitimaci
Topic 3: studi, use, infect, virus, sampl, group, result, patient, cell, differ
Topic 4: apelin, vasopressin, psa, fsfs, unusu, curcumin, tbk, plp, replic, anim
Topic 5: btv, aminopeptidas, aptam, hfold, isr, ece, bile, rtqpcr, oligomer, blast

Cluster 15:
Topic 1: consensus, biosystem, alanin, serin, crisi, physician, shorten, comment, metastasi, letter
Topic 2: compound, activ, use, inhibitor, reaction, cell, drug, extract, solvent, product
Topic 3: consensus, biosystem, alanin, serin, crisi, physician, shorten, comment, metastasi, letter
Topic 4: consensus, biosystem, alanin, serin, crisi, physician, shorten, comment, metastasi, letter
Topic 5: consensus, biosystem, alanin, serin, crisi, physician, shorten, comment, metastasi, letter

Cluster 16:
Topic 1: patient, health, care, covid, staff, hospit, nurs, healthcar, pandem, medic
Topic 2: difficil, bmi, nos, thermo, constitu, portion, sea, chloroquin, maximum, arrhythmia
Topic 3: difficil, bmi, nos, thermo, constitu, portion, sea, chloroquin, maximum, arrhythmia
Topic 4: difficil, bmi, nos, thermo, constitu, portion, sea, chloroquin, maximum, arrhythmia
Topic 5: difficil, bmi, nos, thermo, constitu, portion, sea, chloroquin, maximum, arrhythmia

</pre></div></div><div></div></colab-static-output-renderer></div></div><div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-FboibFCYLKAW" tabindex="-1" role="region" aria-label="Cell 37: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><div class="editor flex monaco" data-keybinding-context="50" data-mode-id="notebook-python" style="height: 1796px; --vscode-editorCodeLens-lineHeight: 16px; --vscode-editorCodeLens-fontSize: 12px; --vscode-editorCodeLens-fontFeatureSettings: &quot;liga&quot; off, &quot;calt&quot; off;"><div class="monaco-editor no-user-select  showUnused showDeprecated vs" role="code" data-uri="inmemory://model/53" style="width: 1411px; height: 1796px;"><div data-mprt="3" class="overflow-guard" style="width: 1411px; height: 1796px;"><div class="margin" role="presentation" aria-hidden="true" style="position: absolute; contain: strict; will-change: unset; top: 0px; height: 1796px; width: 6px;"><div class="glyph-margin" style="left: 0px; width: 0px; height: 1796px;"></div><div class="margin-view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="margin-view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 6px; height: 1796px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line current-line-margin-both" style="width:6px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div><div style="position:absolute;top:513px;width:100%;height:19px;"></div><div style="position:absolute;top:532px;width:100%;height:19px;"></div><div style="position:absolute;top:551px;width:100%;height:19px;"></div><div style="position:absolute;top:570px;width:100%;height:19px;"></div><div style="position:absolute;top:589px;width:100%;height:19px;"></div><div style="position:absolute;top:608px;width:100%;height:19px;"></div><div style="position:absolute;top:627px;width:100%;height:19px;"></div><div style="position:absolute;top:646px;width:100%;height:19px;"></div><div style="position:absolute;top:665px;width:100%;height:19px;"></div><div style="position:absolute;top:684px;width:100%;height:19px;"></div><div style="position:absolute;top:703px;width:100%;height:19px;"></div><div style="position:absolute;top:722px;width:100%;height:19px;"></div><div style="position:absolute;top:741px;width:100%;height:19px;"></div><div style="position:absolute;top:760px;width:100%;height:19px;"></div><div style="position:absolute;top:779px;width:100%;height:19px;"></div><div style="position:absolute;top:798px;width:100%;height:19px;"></div><div style="position:absolute;top:817px;width:100%;height:19px;"></div><div style="position:absolute;top:836px;width:100%;height:19px;"></div><div style="position:absolute;top:855px;width:100%;height:19px;"></div><div style="position:absolute;top:874px;width:100%;height:19px;"></div><div style="position:absolute;top:893px;width:100%;height:19px;"></div><div style="position:absolute;top:912px;width:100%;height:19px;"></div><div style="position:absolute;top:931px;width:100%;height:19px;"></div><div style="position:absolute;top:950px;width:100%;height:19px;"></div><div style="position:absolute;top:969px;width:100%;height:19px;"></div><div style="position:absolute;top:988px;width:100%;height:19px;"></div><div style="position:absolute;top:1007px;width:100%;height:19px;"></div><div style="position:absolute;top:1026px;width:100%;height:19px;"></div><div style="position:absolute;top:1045px;width:100%;height:19px;"></div><div style="position:absolute;top:1064px;width:100%;height:19px;"></div><div style="position:absolute;top:1083px;width:100%;height:19px;"></div><div style="position:absolute;top:1102px;width:100%;height:19px;"></div><div style="position:absolute;top:1121px;width:100%;height:19px;"></div><div style="position:absolute;top:1140px;width:100%;height:19px;"></div><div style="position:absolute;top:1159px;width:100%;height:19px;"></div><div style="position:absolute;top:1178px;width:100%;height:19px;"></div><div style="position:absolute;top:1197px;width:100%;height:19px;"></div><div style="position:absolute;top:1216px;width:100%;height:19px;"></div><div style="position:absolute;top:1235px;width:100%;height:19px;"></div><div style="position:absolute;top:1254px;width:100%;height:19px;"></div><div style="position:absolute;top:1273px;width:100%;height:19px;"></div><div style="position:absolute;top:1292px;width:100%;height:19px;"></div><div style="position:absolute;top:1311px;width:100%;height:19px;"></div><div style="position:absolute;top:1330px;width:100%;height:19px;"></div><div style="position:absolute;top:1349px;width:100%;height:19px;"></div><div style="position:absolute;top:1368px;width:100%;height:19px;"></div><div style="position:absolute;top:1387px;width:100%;height:19px;"></div><div style="position:absolute;top:1406px;width:100%;height:19px;"></div><div style="position:absolute;top:1425px;width:100%;height:19px;"></div><div style="position:absolute;top:1444px;width:100%;height:19px;"></div><div style="position:absolute;top:1463px;width:100%;height:19px;"></div><div style="position:absolute;top:1482px;width:100%;height:19px;"></div><div style="position:absolute;top:1501px;width:100%;height:19px;"></div><div style="position:absolute;top:1520px;width:100%;height:19px;"></div><div style="position:absolute;top:1539px;width:100%;height:19px;"></div><div style="position:absolute;top:1558px;width:100%;height:19px;"></div><div style="position:absolute;top:1577px;width:100%;height:19px;"></div><div style="position:absolute;top:1596px;width:100%;height:19px;"></div><div style="position:absolute;top:1615px;width:100%;height:19px;"></div><div style="position:absolute;top:1634px;width:100%;height:19px;"></div><div style="position:absolute;top:1653px;width:100%;height:19px;"></div><div style="position:absolute;top:1672px;width:100%;height:19px;"></div><div style="position:absolute;top:1691px;width:100%;height:19px;"></div><div style="position:absolute;top:1710px;width:100%;height:19px;"></div><div style="position:absolute;top:1729px;width:100%;height:19px;"></div><div style="position:absolute;top:1748px;width:100%;height:19px;"></div><div style="position:absolute;top:1767px;width:100%;height:19px;"></div></div><div class="glyph-margin-widgets" style="position: absolute; top: 0px;"></div></div><div class="monaco-scrollable-element editor-scrollable vs" role="presentation" data-mprt="5" style="position: absolute; overflow: hidden; left: 6px; width: 1405px; height: 1796px;"><div class="lines-content monaco-editor-background" style="position: absolute; overflow: hidden; width: 1e+06px; height: 1796px; contain: strict; will-change: unset; top: 0px; left: 0px;"><div class="view-overlays" role="presentation" aria-hidden="true" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; height: 0px; width: 1405px;"><div style="position:absolute;top:0px;width:100%;height:19px;"><div class="current-line" style="width:1405px; height:19px;"></div></div><div style="position:absolute;top:19px;width:100%;height:19px;"></div><div style="position:absolute;top:38px;width:100%;height:19px;"></div><div style="position:absolute;top:57px;width:100%;height:19px;"></div><div style="position:absolute;top:76px;width:100%;height:19px;"></div><div style="position:absolute;top:95px;width:100%;height:19px;"></div><div style="position:absolute;top:114px;width:100%;height:19px;"></div><div style="position:absolute;top:133px;width:100%;height:19px;"></div><div style="position:absolute;top:152px;width:100%;height:19px;"></div><div style="position:absolute;top:171px;width:100%;height:19px;"></div><div style="position:absolute;top:190px;width:100%;height:19px;"></div><div style="position:absolute;top:209px;width:100%;height:19px;"></div><div style="position:absolute;top:228px;width:100%;height:19px;"></div><div style="position:absolute;top:247px;width:100%;height:19px;"></div><div style="position:absolute;top:266px;width:100%;height:19px;"></div><div style="position:absolute;top:285px;width:100%;height:19px;"></div><div style="position:absolute;top:304px;width:100%;height:19px;"></div><div style="position:absolute;top:323px;width:100%;height:19px;"></div><div style="position:absolute;top:342px;width:100%;height:19px;"></div><div style="position:absolute;top:361px;width:100%;height:19px;"></div><div style="position:absolute;top:380px;width:100%;height:19px;"></div><div style="position:absolute;top:399px;width:100%;height:19px;"></div><div style="position:absolute;top:418px;width:100%;height:19px;"></div><div style="position:absolute;top:437px;width:100%;height:19px;"></div><div style="position:absolute;top:456px;width:100%;height:19px;"></div><div style="position:absolute;top:475px;width:100%;height:19px;"></div><div style="position:absolute;top:494px;width:100%;height:19px;"></div><div style="position:absolute;top:513px;width:100%;height:19px;"></div><div style="position:absolute;top:532px;width:100%;height:19px;"></div><div style="position:absolute;top:551px;width:100%;height:19px;"></div><div style="position:absolute;top:570px;width:100%;height:19px;"></div><div style="position:absolute;top:589px;width:100%;height:19px;"></div><div style="position:absolute;top:608px;width:100%;height:19px;"></div><div style="position:absolute;top:627px;width:100%;height:19px;"></div><div style="position:absolute;top:646px;width:100%;height:19px;"></div><div style="position:absolute;top:665px;width:100%;height:19px;"></div><div style="position:absolute;top:684px;width:100%;height:19px;"></div><div style="position:absolute;top:703px;width:100%;height:19px;"></div><div style="position:absolute;top:722px;width:100%;height:19px;"></div><div style="position:absolute;top:741px;width:100%;height:19px;"></div><div style="position:absolute;top:760px;width:100%;height:19px;"></div><div style="position:absolute;top:779px;width:100%;height:19px;"></div><div style="position:absolute;top:798px;width:100%;height:19px;"></div><div style="position:absolute;top:817px;width:100%;height:19px;"></div><div style="position:absolute;top:836px;width:100%;height:19px;"></div><div style="position:absolute;top:855px;width:100%;height:19px;"></div><div style="position:absolute;top:874px;width:100%;height:19px;"></div><div style="position:absolute;top:893px;width:100%;height:19px;"></div><div style="position:absolute;top:912px;width:100%;height:19px;"></div><div style="position:absolute;top:931px;width:100%;height:19px;"></div><div style="position:absolute;top:950px;width:100%;height:19px;"></div><div style="position:absolute;top:969px;width:100%;height:19px;"></div><div style="position:absolute;top:988px;width:100%;height:19px;"></div><div style="position:absolute;top:1007px;width:100%;height:19px;"></div><div style="position:absolute;top:1026px;width:100%;height:19px;"></div><div style="position:absolute;top:1045px;width:100%;height:19px;"></div><div style="position:absolute;top:1064px;width:100%;height:19px;"></div><div style="position:absolute;top:1083px;width:100%;height:19px;"></div><div style="position:absolute;top:1102px;width:100%;height:19px;"></div><div style="position:absolute;top:1121px;width:100%;height:19px;"></div><div style="position:absolute;top:1140px;width:100%;height:19px;"></div><div style="position:absolute;top:1159px;width:100%;height:19px;"></div><div style="position:absolute;top:1178px;width:100%;height:19px;"></div><div style="position:absolute;top:1197px;width:100%;height:19px;"></div><div style="position:absolute;top:1216px;width:100%;height:19px;"></div><div style="position:absolute;top:1235px;width:100%;height:19px;"></div><div style="position:absolute;top:1254px;width:100%;height:19px;"></div><div style="position:absolute;top:1273px;width:100%;height:19px;"></div><div style="position:absolute;top:1292px;width:100%;height:19px;"></div><div style="position:absolute;top:1311px;width:100%;height:19px;"></div><div style="position:absolute;top:1330px;width:100%;height:19px;"></div><div style="position:absolute;top:1349px;width:100%;height:19px;"></div><div style="position:absolute;top:1368px;width:100%;height:19px;"></div><div style="position:absolute;top:1387px;width:100%;height:19px;"></div><div style="position:absolute;top:1406px;width:100%;height:19px;"></div><div style="position:absolute;top:1425px;width:100%;height:19px;"></div><div style="position:absolute;top:1444px;width:100%;height:19px;"></div><div style="position:absolute;top:1463px;width:100%;height:19px;"></div><div style="position:absolute;top:1482px;width:100%;height:19px;"></div><div style="position:absolute;top:1501px;width:100%;height:19px;"></div><div style="position:absolute;top:1520px;width:100%;height:19px;"></div><div style="position:absolute;top:1539px;width:100%;height:19px;"></div><div style="position:absolute;top:1558px;width:100%;height:19px;"></div><div style="position:absolute;top:1577px;width:100%;height:19px;"></div><div style="position:absolute;top:1596px;width:100%;height:19px;"></div><div style="position:absolute;top:1615px;width:100%;height:19px;"></div><div style="position:absolute;top:1634px;width:100%;height:19px;"></div><div style="position:absolute;top:1653px;width:100%;height:19px;"></div><div style="position:absolute;top:1672px;width:100%;height:19px;"></div><div style="position:absolute;top:1691px;width:100%;height:19px;"></div><div style="position:absolute;top:1710px;width:100%;height:19px;"></div><div style="position:absolute;top:1729px;width:100%;height:19px;"></div><div style="position:absolute;top:1748px;width:100%;height:19px;"></div><div style="position:absolute;top:1767px;width:100%;height:19px;"></div></div><div role="presentation" aria-hidden="true" class="view-rulers"><div class="view-ruler" style="width: 2px; height: 1796px; left: 615.938px;"></div></div><div class="view-zones" role="presentation" aria-hidden="true" style="position: absolute;"></div><div class="view-lines monaco-mouse-cursor-text" role="presentation" aria-hidden="true" data-mprt="7" style="position: absolute; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; width: 1405px; height: 1796px;"><div style="top:0px;height:19px;" class="view-line"><span><span class="mtk19">import</span><span class="mtk1">&nbsp;plotly.express&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;px</span></span></div><div style="top:19px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:38px;height:19px;" class="view-line"><span><span class="mtk6">def</span><span class="mtk1">&nbsp;</span><span class="mtk15">interactive_plot</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk16">df</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">:</span></span></div><div style="top:57px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;clusters&nbsp;=&nbsp;</span><span class="mtk15">sorted</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'cluster'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">.unique</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:76px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:95px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Generate&nbsp;distinct&nbsp;colors&nbsp;for&nbsp;each&nbsp;cluster&nbsp;using&nbsp;</span><span class="mtk8">Plotly's&nbsp;colors</span></span></div><div style="top:114px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;colors&nbsp;=&nbsp;px.colors.qualitative.Plotly</span></span></div><div style="top:133px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:152px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Create&nbsp;a&nbsp;scatter&nbsp;plot&nbsp;for&nbsp;each&nbsp;cluster&nbsp;with&nbsp;a&nbsp;un</span><span class="mtk8">ique&nbsp;color</span></span></div><div style="top:171px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;data&nbsp;=&nbsp;</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:190px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;i,&nbsp;cluster&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;</span><span class="mtk15">enumerate</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">clusters</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">:</span></span></div><div style="top:209px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cluster_data&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1">df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'cluster'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">&nbsp;==&nbsp;cluster</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:228px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;scatter&nbsp;=&nbsp;go.Scatter</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:247px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;x=cluster_data</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:266px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y=cluster_data</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:285px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mode=</span><span class="mtk26">'markers'</span><span class="mtk1">,</span></span></div><div style="top:304px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name=</span><span class="mtk6">f</span><span class="mtk26">'Cluster&nbsp;</span><span class="mtk1 bracket-highlighting-1">{</span><span class="mtk1">cluster</span><span class="mtk1 bracket-highlighting-1">}</span><span class="mtk26">'</span><span class="mtk1">,</span></span></div><div style="top:323px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;text=cluster_data</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'title'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:342px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hoverinfo=</span><span class="mtk26">'text'</span><span class="mtk1">,</span></span></div><div style="top:361px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;marker=</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1">size=</span><span class="mtk12">10</span><span class="mtk1">,&nbsp;color=colors</span><span class="mtk1 bracket-highlighting-2">[</span><span class="mtk1">i&nbsp;%&nbsp;</span><span class="mtk15">len</span><span class="mtk1 bracket-highlighting-3">(</span><span class="mtk1">colors</span><span class="mtk1 bracket-highlighting-3">)</span><span class="mtk1 bracket-highlighting-2">]</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Assign&nbsp;a&nbsp;unique&nbsp;color</span></span></div><div style="top:380px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;visible=</span><span class="mtk6">False</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Initially,&nbsp;make&nbsp;all&nbsp;traces&nbsp;invisible</span></span></div><div style="top:399px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:418px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;data.append</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">scatter</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:437px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:456px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Add&nbsp;a&nbsp;scatter&nbsp;plot&nbsp;for&nbsp;all&nbsp;clusters&nbsp;with&nbsp;differe</span><span class="mtk8">nt&nbsp;colors</span></span></div><div style="top:475px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;scatter_all&nbsp;=&nbsp;go.Scatter</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:494px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;x=df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:513px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y=df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:532px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mode=</span><span class="mtk26">'markers'</span><span class="mtk1">,</span></span></div><div style="top:551px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name=</span><span class="mtk26">'All&nbsp;Clusters'</span><span class="mtk1">,</span></span></div><div style="top:570px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;text=df</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk26">'title'</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:589px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hoverinfo=</span><span class="mtk26">'text'</span><span class="mtk1">,</span></span></div><div style="top:608px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;marker=</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1">size=</span><span class="mtk12">10</span><span class="mtk1">,&nbsp;color=df</span><span class="mtk1 bracket-highlighting-2">[</span><span class="mtk26">'cluster'</span><span class="mtk1 bracket-highlighting-2">]</span><span class="mtk1">.</span><span class="mtk15">map</span><span class="mtk1 bracket-highlighting-2">(</span><span class="mtk6">lambda</span><span class="mtk1">&nbsp;x:&nbsp;colors</span><span class="mtk1 bracket-highlighting-3">[</span><span class="mtk1">x&nbsp;%&nbsp;</span><span class="mtk15">len</span><span class="mtk1 bracket-highlighting-4">(</span><span class="mtk1">colors</span><span class="mtk1 bracket-highlighting-4">)</span><span class="mtk1 bracket-highlighting-3">]</span><span class="mtk1 bracket-highlighting-2">)</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Assign&nbsp;colors&nbsp;by&nbsp;cluster</span></span></div><div style="top:627px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;visible=</span><span class="mtk6">True</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Initially,&nbsp;show&nbsp;all&nbsp;clusters</span></span></div><div style="top:646px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:665px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;data.append</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">scatter_all</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:684px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:703px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;x_min&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">.</span><span class="mtk15">min</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:722px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;x_max&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-one'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">.</span><span class="mtk15">max</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:741px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;y_min&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">.</span><span class="mtk15">min</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:760px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;y_max&nbsp;=&nbsp;df</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'tsne-2d-two'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">.</span><span class="mtk15">max</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:779px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:798px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Initialize&nbsp;the&nbsp;figure</span></span></div><div style="top:817px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;fig&nbsp;=&nbsp;go.Figure</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">data=data</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:836px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:855px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Ensure&nbsp;square&nbsp;aspect&nbsp;ratio</span></span></div><div style="top:874px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;fig.update_layout</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:893px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;title=</span><span class="mtk26">'Cluster&nbsp;Visualization'</span><span class="mtk1">,</span></span></div><div style="top:912px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;xaxis=</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1">title=</span><span class="mtk26">'t-SNE&nbsp;1'</span><span class="mtk1">,&nbsp;range=</span><span class="mtk1 bracket-highlighting-2">[</span><span class="mtk1">x_min,&nbsp;x_max</span><span class="mtk1 bracket-highlighting-2">]</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Ensure&nbsp;x&nbsp;and&nbsp;y&nbsp;axes&nbsp;are&nbsp;equal</span></span></div><div style="top:931px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;yaxis=</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1">title=</span><span class="mtk26">'t-SNE&nbsp;2'</span><span class="mtk1">,&nbsp;range=</span><span class="mtk1 bracket-highlighting-2">[</span><span class="mtk1">y_min,&nbsp;y_max</span><span class="mtk1 bracket-highlighting-2">]</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,</span></span></div><div style="top:950px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;width=</span><span class="mtk12">1000</span><span class="mtk1">,</span></span></div><div style="top:969px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;height=</span><span class="mtk12">700</span><span class="mtk1">&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Ensure&nbsp;the&nbsp;figure&nbsp;is&nbsp;square-shaped</span></span></div><div style="top:988px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1007px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1026px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Add&nbsp;hover&nbsp;functionality</span></span></div><div style="top:1045px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;fig.update_traces</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:1064px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hoverinfo=</span><span class="mtk26">'text'</span><span class="mtk1">,</span></span></div><div style="top:1083px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;marker=</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span><span class="mtk1">opacity=</span><span class="mtk12">0.7</span><span class="mtk1">,&nbsp;size=</span><span class="mtk12">8</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1">,</span></span></div><div style="top:1102px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1121px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1140px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Add&nbsp;interactive&nbsp;slider&nbsp;for&nbsp;cluster&nbsp;selection</span></span></div><div style="top:1159px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;steps&nbsp;=&nbsp;</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:1178px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk19">for</span><span class="mtk1">&nbsp;i,&nbsp;cluster&nbsp;</span><span class="mtk6">in</span><span class="mtk1">&nbsp;</span><span class="mtk15">enumerate</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">clusters</span><span class="mtk1 bracket-highlighting-0">)</span><span class="mtk1">:</span></span></div><div style="top:1197px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;step&nbsp;=&nbsp;</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:1216px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;method=</span><span class="mtk26">'update'</span><span class="mtk1">,</span></span></div><div style="top:1235px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;args=</span><span class="mtk1 bracket-highlighting-1">[</span><span class="mtk1 bracket-highlighting-2">{</span><span class="mtk26">'visible'</span><span class="mtk1">:&nbsp;</span><span class="mtk1 bracket-highlighting-3">[</span><span class="mtk6">False</span><span class="mtk1 bracket-highlighting-3">]</span><span class="mtk1">&nbsp;*&nbsp;</span><span class="mtk15">len</span><span class="mtk1 bracket-highlighting-3">(</span><span class="mtk1">clusters</span><span class="mtk1 bracket-highlighting-3">)</span><span class="mtk1">&nbsp;+&nbsp;</span><span class="mtk1 bracket-highlighting-3">[</span><span class="mtk6">False</span><span class="mtk1 bracket-highlighting-3">]</span><span class="mtk1 bracket-highlighting-2">}</span><span class="mtk1">,&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Hide&nbsp;all&nbsp;clusters</span></span></div><div style="top:1254px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-2">{</span><span class="mtk26">'title'</span><span class="mtk1">:&nbsp;</span><span class="mtk6">f</span><span class="mtk26">'Cluster&nbsp;</span><span class="mtk1 bracket-highlighting-3">{</span><span class="mtk1">cluster</span><span class="mtk1 bracket-highlighting-3">}</span><span class="mtk26">'</span><span class="mtk1 bracket-highlighting-2">}</span><span class="mtk1 bracket-highlighting-1">]</span><span class="mtk1">,</span></span></div><div style="top:1273px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;label=</span><span class="mtk6">f</span><span class="mtk26">'Cluster&nbsp;</span><span class="mtk1 bracket-highlighting-1">{</span><span class="mtk1">cluster</span><span class="mtk1 bracket-highlighting-1">}</span><span class="mtk26">'</span></span></div><div style="top:1292px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1311px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Only&nbsp;make&nbsp;the&nbsp;current&nbsp;cluster&nbsp;visible</span></span></div><div style="top:1330px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;step</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'args'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk12">0</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk26">'visible'</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk1">i</span><span class="mtk1 bracket-highlighting-0">]</span><span class="mtk1">&nbsp;=&nbsp;</span><span class="mtk6">True</span></span></div><div style="top:1349px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;steps.append</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1">step</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1368px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1387px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Add&nbsp;final&nbsp;step&nbsp;for&nbsp;all&nbsp;clusters</span></span></div><div style="top:1406px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;steps.append</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span></span></div><div style="top:1425px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;method=</span><span class="mtk26">'update'</span><span class="mtk1">,</span></span></div><div style="top:1444px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;args=</span><span class="mtk1 bracket-highlighting-2">[</span><span class="mtk1 bracket-highlighting-3">{</span><span class="mtk26">'visible'</span><span class="mtk1">:&nbsp;</span><span class="mtk1 bracket-highlighting-4">[</span><span class="mtk6">False</span><span class="mtk1 bracket-highlighting-4">]</span><span class="mtk1">&nbsp;*&nbsp;</span><span class="mtk15">len</span><span class="mtk1 bracket-highlighting-4">(</span><span class="mtk1">clusters</span><span class="mtk1 bracket-highlighting-4">)</span><span class="mtk1">&nbsp;+&nbsp;</span><span class="mtk1 bracket-highlighting-4">[</span><span class="mtk6">True</span><span class="mtk1 bracket-highlighting-4">]</span><span class="mtk1 bracket-highlighting-3">}</span><span class="mtk1">,&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Only&nbsp;show&nbsp;the&nbsp;'all&nbsp;clusters'&nbsp;trace</span></span></div><div style="top:1463px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-3">{</span><span class="mtk26">'title'</span><span class="mtk1">:&nbsp;</span><span class="mtk26">'All&nbsp;Clusters'</span><span class="mtk1 bracket-highlighting-3">}</span><span class="mtk1 bracket-highlighting-2">]</span><span class="mtk1">,</span></span></div><div style="top:1482px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;label=</span><span class="mtk26">'All&nbsp;Clusters'</span></span></div><div style="top:1501px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1520px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1539px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;sliders&nbsp;=&nbsp;</span><span class="mtk1 bracket-highlighting-0">[</span><span class="mtk14">dict</span><span class="mtk1 bracket-highlighting-1">(</span></span></div><div style="top:1558px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;active=</span><span class="mtk15">len</span><span class="mtk1 bracket-highlighting-2">(</span><span class="mtk1">steps</span><span class="mtk1 bracket-highlighting-2">)</span><span class="mtk1">&nbsp;-&nbsp;</span><span class="mtk12">1</span><span class="mtk1">,</span></span></div><div style="top:1577px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;currentvalue=</span><span class="mtk1 bracket-highlighting-2">{</span><span class="mtk26">"prefix"</span><span class="mtk1">:&nbsp;</span><span class="mtk26">"Cluster:&nbsp;"</span><span class="mtk1 bracket-highlighting-2">}</span><span class="mtk1">,</span></span></div><div style="top:1596px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pad=</span><span class="mtk1 bracket-highlighting-2">{</span><span class="mtk26">"t"</span><span class="mtk1">:&nbsp;</span><span class="mtk12">50</span><span class="mtk1 bracket-highlighting-2">}</span><span class="mtk1">,</span></span></div><div style="top:1615px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;steps=steps</span></span></div><div style="top:1634px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-1">)</span><span class="mtk1 bracket-highlighting-0">]</span></span></div><div style="top:1653px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1672px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;fig.update_layout</span><span class="mtk1 bracket-highlighting-0">(</span></span></div><div style="top:1691px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sliders=sliders</span></span></div><div style="top:1710px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk1 bracket-highlighting-0">)</span></span></div><div style="top:1729px;height:19px;" class="view-line"><span><span></span></span></div><div style="top:1748px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="mtk8">#&nbsp;Display&nbsp;the&nbsp;plot</span></span></div><div style="top:1767px;height:19px;" class="view-line"><span><span class="mtk1">&nbsp;&nbsp;&nbsp;&nbsp;fig.show</span><span class="mtk1 bracket-highlighting-0">(</span><span class="mtk1 bracket-highlighting-0">)</span></span></div></div><div data-mprt="1" class="contentWidgets" style="position: absolute; top: 0px;"></div><div role="presentation" aria-hidden="true" class="cursors-layer cursor-line-style cursor-solid"><div class="cursor monaco-mouse-cursor-text " style="height: 19px; top: 0px; left: 0px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; display: block; visibility: hidden; padding-left: 0px; width: 1.6px;"></div></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute; width: 1391px; height: 10px; left: 0px; bottom: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; width: 1391px;"></div></div><canvas class="decorationsOverviewRuler" aria-hidden="true" width="17" height="2245" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; top: 0px; right: 0px; width: 14px; height: 1796px; will-change: unset; display: block;"></canvas><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute; width: 14px; height: 1796px; right: 0px; top: 0px;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 14px; transform: translate3d(0px, 0px, 0px); contain: strict; will-change: unset; height: 1796px;"></div></div></div><div role="presentation" aria-hidden="true" style="width: 1411px;"></div><textarea data-mprt="6" class="inputarea monaco-mouse-cursor-text" wrap="on" autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" aria-label="Editor content;Press Alt+F1 for Accessibility Options." tabindex="0" role="textbox" aria-roledescription="editor" aria-multiline="true" aria-haspopup="false" aria-autocomplete="both" style="tab-size: 15.3984px; font-family: monospace, Consolas, &quot;Courier New&quot;, monospace; font-weight: normal; font-size: 14px; font-feature-settings: &quot;liga&quot; 0, &quot;calt&quot; 0; font-variation-settings: normal; line-height: 19px; letter-spacing: 0px; top: 0px; left: 6px; width: 1411px; height: 1px;"></textarea><div style="position: absolute; top: 0px; left: 0px; width: 0px; height: 0px;" class="monaco-editor-background textAreaCover"></div><div data-mprt="4" class="overlayWidgets" style="width: 1411px;"></div><div data-mprt="8" class="minimap slider-mouseover" role="presentation" aria-hidden="true" style="position: absolute; left: 0px; width: 0px; height: 1796px;"><div class="minimap-shadow-hidden" style="height: 1796px;"></div><canvas width="0" height="2245" style="position: absolute; left: 0px; width: 0px; height: 1796px;"></canvas><canvas class="minimap-decorations-layer" width="0" height="2245" style="position: absolute; left: 0px; width: 0px; height: 1796px;"></canvas><div class="minimap-slider" style="position: absolute; transform: translate3d(0px, 0px, 0px); contain: strict; width: 0px; will-change: unset;"><div class="minimap-slider-horizontal" style="position: absolute; width: 0px; height: 0px;"></div></div></div><div role="presentation" aria-hidden="true" class="blockDecorations-container"></div></div><div data-mprt="2" class="overflowingContentWidgets" style="display: none;"><div widgetid="editor.contrib.resizableContentHoverWidget" style="position: fixed; height: 10px; width: 10px; z-index: 50; display: none; visibility: hidden; max-width: 1536px;"><div class="monaco-sash vertical" style="left: 8px;"></div><div class="monaco-sash vertical" style="left: -2px;"></div><div class="monaco-sash orthogonal-edge-north horizontal" style="top: -2px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-sash orthogonal-edge-south horizontal" style="top: 8px;"><div class="orthogonal-drag-handle start"></div><div class="orthogonal-drag-handle end"></div></div><div class="monaco-hover hidden" tabindex="0" role="tooltip"><div class="monaco-scrollable-element " role="presentation" style="position: relative; overflow: hidden;"><div class="monaco-hover-content" style="overflow: hidden; font-size: 14px; line-height: 1.35714; max-width: 931.26px; max-height: 449px;"></div><div role="presentation" aria-hidden="true" class="invisible scrollbar horizontal" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; height: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div role="presentation" aria-hidden="true" class="invisible scrollbar vertical" style="position: absolute;"><div class="slider" style="position: absolute; top: 0px; left: 0px; width: 10px; transform: translate3d(0px, 0px, 0px); contain: strict;"></div></div><div class="shadow"></div><div class="shadow"></div><div class="shadow"></div></div></div></div></div><div class=".in-cell-overflowing"><div widgetid="editor.contrib.quickInputWidget" style="position: absolute; top: 0px; right: 50%;"></div></div></div></div></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 37 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> <div><div></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code code-has-output icon-scrolling" id="cell-NNzHwU5M8uf2" tabindex="-1" role="region" aria-label="Cell 38: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1.244s" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class="cell-execution stale">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab colab" data-lang="notebook-python"><span><span class="mtk19">import</span><span class="mtk1">&nbsp;plotly.graph_objs&nbsp;</span><span class="mtk19">as</span><span class="mtk1">&nbsp;go</span></span><br><span><span></span></span><br><span><span class="mtk8">#&nbsp;Assuming&nbsp;you&nbsp;have&nbsp;a&nbsp;DataFrame&nbsp;'df'&nbsp;containing&nbsp;yo</span><span class="mtk8">ur&nbsp;data,&nbsp;and&nbsp;it&nbsp;has&nbsp;columns&nbsp;'tsne-2d-one',&nbsp;'tsne-2</span><span class="mtk8">d-two',&nbsp;'y',&nbsp;and&nbsp;'title'</span></span><br><span><span class="mtk1">tfidf_features_2d_df[</span><span class="mtk26">'title'</span><span class="mtk1">]=df[</span><span class="mtk26">'title'</span><span class="mtk1">]</span></span><br><span><span class="mtk8">#&nbsp;Call&nbsp;the&nbsp;interactive_plot&nbsp;function&nbsp;with&nbsp;your&nbsp;Dat</span><span class="mtk8">aFrame&nbsp;as&nbsp;input</span></span><br><span><span class="mtk1">interactive_plot(tfidf_features_2d_df)</span></span><br><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 38 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content">
          <div class="output-info"><colab-output-info title="Clear output

executed by maryam j
Wednesday, June 5, 2024 (3 days ago)
executed in 1.244s"><template shadowrootmode="open"><!----><md-icon-button title="Code cell output actions" aria-label="Code cell output actions" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Code cell output actions">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$--><svg viewBox="0 0 24 24"><!--?lit$944599098$--><path d="m15.9 3.07c-4.32 0.0742-8.64-0.0355-13 0.0568-1.37 0.307-1.74 2.1-1.41 3.26 0.469 0.606 1.86 0.384 1.66-0.525 0.0448-0.329-0.183-0.93 0.354-0.766h13.3v1.53h1.71c0.0709-1.13 0.141-2.62-0.968-3.3-0.511-0.264-1.11-0.252-1.67-0.259zm2.94 6.84v4.87c1.62-1.62 3.24-3.24 4.87-4.87h-4.87zm0 0h-1.71v3.43l1.57 1.57c0.32-1.65 0.0556-3.34 0.135-5zm-1.71 3.43v-3.43h-3.43c1.14 1.14 2.29 2.29 3.43 3.43zm1.4 4.27h-1.71v1.48h-13.6v-1.48h-1.71c-0.0473 1.15-0.16 2.72 1.09 3.29 1.47 0.506 3.02 0.0265 4.53 0.192 3.34-0.0051 6.68 0.0336 10-0.0245 1.49-0.366 1.56-2.22 1.42-3.45zm-10.1-1.12c-0.398-0.483-0.796-0.967-1.19-1.45 0.59-0.683 1.18-1.37 1.77-2.05h-8.67v-2h8.67c-0.59-0.683-1.18-1.37-1.77-2.05 0.398-0.483 0.796-0.967 1.19-1.45 1.28 1.5 2.56 3 3.84 4.5-1.28 1.5-2.56 3-3.84 4.5z"></path></svg></md-icon>
      </md-icon-button></template></colab-output-info></div>
          <div class="output-iframe-container">
            <div class="output-iframe-sizer"> <div style=""><div class="outputview" style="height: 717px;"><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(10).html" class="" style="height: 717px;"></iframe></div></div></div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div><div class="cell code icon-scrolling" id="cell-qu2zDG3D8wQe" tabindex="-1" role="region" aria-label="Cell 39: Code cell: " style=""><div class="cell-tag-editor sticky"></div><div class="cell-toolbar sticky"></div><div class="main-content" elevation="0"><div class="cell-contents"><div class="cell-mask"></div><span class="imported-info-area"></span><div class="codecell-input-output">
      <div class="inputarea horizontal layout code">
        <div class="cell-gutter">
          <!-- Bounding range for vertical scrolling of icons -->
          <div class="cell-execution-container">
            <colab-run-button title="Run cell (Ctrl+Enter)
cell has not been executed in this session" role="button" aria-label="Run cell"><template shadowrootmode="open"><!----> <div class=" cell-execution stale ">
      <div class="execution-count"><!--?lit$944599098$-->[ ]</div>
      <div class="cell-execution-indicator"> <!--?lit$944599098$-->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
  <!--?lit$944599098$-->
  <mask id="playSymbolMask">
    <rect width="100%" height="100%" fill="white"></rect>
    <polygon points="10,8 17,12 10,16" fill="black"></polygon>
  </mask>
  <circle cx="12" cy="12" r="7.8" mask="url(#playSymbolMask)" id="filledCircle"></circle>
</svg> </div>
      <!--?lit$944599098$--><!--?-->
    </div></template></colab-run-button>
          </div>
        </div>
      <div class="editor flex lazy-editor" style=""><pre class="lazy-virtualized" style="font-size: 14px; line-height: 19px;"><pre class="lazy-gutter"></pre><pre class="monaco-colorized colab colab colab" data-lang="notebook-python"><span><span></span></span><br></pre><colab-read-only-cell-placeholder style="display: none;"><template shadowrootmode="open"><!----><div><!--?lit$944599098$-->Start coding or <span tabindex="0" role="button" class="link">generate</span> with AI.</div></template></colab-read-only-cell-placeholder></pre></div><colab-form class="formview vertical layout flex"><div class="widget-area vertical layout"></div></colab-form></div>
    <div class="output" aria-label="Cell 39 output" role="region"><!----> <div class="output-header"> </div>
        <div class="output-content" hidden="">
          <div class="output-info"> </div>
          <div class="output-iframe-container" hidden="">
            <div class="output-iframe-sizer"> </div>
          </div>
        </div></div></div><colab-cell-next-steps><template shadowrootmode="open"><!----></template></colab-cell-next-steps></div></div><div class="add-cell">
      <hr>
    </div></div></div>
              </div>
            </div>
          <div class="sidebar" style="display: none;"></div></div>
          <!--?lit$944599098$--> <div class="footer-links">
      <a target="_blank" href="https://colab.research.google.com/signup?utm_source=footer&amp;utm_medium=link&amp;utm_campaign=footer_links">
        <!--?lit$944599098$-->Colab paid products
      </a>
      -
      <a href="https://colab.research.google.com/cancel-subscription" target="_blank">
        <!--?lit$944599098$-->Cancel contracts here
      </a>
    </div>
        </div>
      </colab-shaded-scroller>
      <div class="notebook-scroll-shadow" style="box-shadow: rgba(0, 0, 0, 0.15) 0px 4px 4px -2px inset;"></div>
    </div></colab-tab></div>
  </div></colab-tab-pane>
      <colab-resizer style="height: 33.3%" class="sn-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$944599098$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$944599098$--> <md-icon-button title="Show more" aria-label="Show more" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show more">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      </colab-resizer>
    </div>
      <colab-resizer style="width: 37%" class="we-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$944599098$--> <div class="layout vertical tab-pane-parent">
      <!--?lit$944599098$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$944599098$--> <md-icon-button title="Show more" aria-label="Show more" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show more">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      <colab-resizer style="height: 33.3%" class="sn-resize no-tabs"><div class="resizer-thumb"></div>
        <!--?lit$944599098$--><colab-tab-pane class="layout vertical grow no-tabs" align="horizontal"><!----> <div class="layout vertical grow">
    <div class="tab-pane-header layout horizontal noshrink">
      <md-tabs><template shadowrootmode="open"><!---->
      <div class="tabs">
        <slot></slot>
      </div>
      <md-divider part="divider"><template shadowrootmode="open"><!----></template></md-divider>
    </template></md-tabs>
      <div class="layout grow"></div>
      <!--?lit$944599098$--> <md-icon-button title="Show more" aria-label="Show more" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Show more">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
    <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>more_horiz</md-icon>
  </md-icon-button>
    </div>
    <div class="layout vertical grow tab-pane-container"> </div>
  </div></colab-tab-pane>
      </colab-resizer>
    </div>
      </colab-resizer>
    </div></colab-tab-layout-container>
        </div>
        <div class="proxies"><div><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(11).html" style="width: 1px; height: 1px; position: absolute; top: -100px;"></iframe></div><div><colab-dom-lifecycle-events style="display: none;"></colab-dom-lifecycle-events><iframe allow="accelerometer; autoplay; gyroscope; magnetometer; xr-spatial-tracking; clipboard-write; camera; microphone; serial; usb" sandbox="allow-downloads allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-modals allow-popups-to-escape-sandbox" src="./DataMining_Project3_HSM.ipynb - Colab_files/outputframe(12).html" style="width: 1px; height: 1px; position: absolute; top: -100px;"></iframe></div></div>
      <colab-file-viewer-manager></colab-file-viewer-manager></div>
    <colab-status-bar role="region" aria-label="Runtime status bar" style="min-height: inherit;"><template shadowrootmode="open"><!----> <!--?lit$944599098$--><div class="frames"></div>
      <md-icon-button class="visible-on-closed" title="Runtime disconnected" aria-label="Runtime disconnected" disabled="" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Runtime disconnected" disabled="">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple disabled="" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon filled="" class="visible-on-closed" status="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template><!--?lit$944599098$-->fiber_manual_record</md-icon>
      </md-icon-button>
      <md-icon-button title="Close" aria-label="Close" role="presentation" value=""><template shadowrootmode="open" shadowrootdelegatesfocus><!----><button id="button" class="icon-button  standard " aria-label="Close">
        <!--?lit$944599098$--><md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
        <!--?lit$944599098$--><md-ripple aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
        <!--?lit$944599098$--><span class="icon"><slot></slot></span>
        <!--?lit$944599098$-->
        <!--?lit$944599098$--><span class="touch"></span>
        <!--?lit$944599098$-->
  </button></template>
        <md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>close</md-icon>
      </md-icon-button></template></colab-status-bar></div><div class="goog-menu" id="file-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="locate-in-drive" class="goog-menuitem " role="menuitem" id=":2" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Locate in Drive<!--?lit$944599098$--></div></div><div command="open-in-playground" class="goog-menuitem " role="menuitem" id=":3" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Open in playground mode<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":4" style="user-select: none;"></div><div command="new" class="goog-menuitem " role="menuitem" id=":5" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->New notebook<!--?lit$944599098$--></div></div><div command="open" class="goog-menuitem " role="menuitem" id=":6" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Open notebook<!--?lit$944599098$--></div></div><div command="import-notebook" class="goog-menuitem " role="menuitem" id=":7" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Upload notebook<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":8" style="user-select: none;"></div><div command="rename" class="goog-menuitem " role="menuitem" id=":9" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Rename<!--?lit$944599098$--></div></div><div command="move-notebook" class="goog-menuitem " role="menuitem" id=":a" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Move<!--?lit$944599098$--></div></div><div command="trash" class="goog-menuitem " role="menuitem" id=":b" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Move to trash<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":c" style="user-select: none;"></div><div command="clone" class="goog-menuitem " role="menuitem" id=":d" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save a copy in Drive<!--?lit$944599098$--></div></div><div command="copy-to-gist" class="goog-menuitem " role="menuitem" id=":e" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save a copy as a GitHub Gist<!--?lit$944599098$--></div></div><div command="copy-to-github" class="goog-menuitem " role="menuitem" id=":f" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save a copy in GitHub<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":g" style="user-select: none;"></div><div command="save" class="goog-menuitem " role="menuitem" id=":h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save<!--?lit$944599098$--></div></div><div command="save-and-checkpoint" class="goog-menuitem " role="menuitem" id=":i" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save and pin revision<!--?lit$944599098$--></div></div><div command="show-history" class="goog-menuitem " role="menuitem" id=":j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Revision history<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":k" style="user-select: none;"></div><div class="goog-submenu goog-menuitem" id="download-submenu-menu-button" role="menuitem" aria-haspopup="true" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;">
      <!--?lit$944599098$-->Download
    <span class="goog-submenu-arrow" style="user-select: none;">►</span></div></div><div command="print" class="goog-menuitem " role="menuitem" id=":o" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Print<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="download-submenu-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="download-ipynb" class="goog-menuitem " role="menuitem" id=":m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Download .ipynb<!--?lit$944599098$--></div></div><div command="download-python" class="goog-menuitem " role="menuitem" id=":n" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Download .py<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="edit-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="undo" class="goog-menuitem " role="menuitem" id=":q" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Undo<!--?lit$944599098$--></div></div><div command="redo" class="goog-menuitem " role="menuitem" id=":r" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Redo<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":s" style="user-select: none;"></div><div command="select-all" class="goog-menuitem " role="menuitem" id=":t" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Select all cells<!--?lit$944599098$--></div></div><div command="cut" class="goog-menuitem " role="menuitem" id=":u" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Cut cell or selection<!--?lit$944599098$--></div></div><div command="copy" class="goog-menuitem " role="menuitem" id=":v" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Copy cell or selection<!--?lit$944599098$--></div></div><div command="paste" class="goog-menuitem " role="menuitem" id=":w" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Paste<!--?lit$944599098$--></div></div><div command="delete-cell-or-selection" class="goog-menuitem " role="menuitem" id=":x" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Delete selected cells<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":y" style="user-select: none;"></div><div command="find" class="goog-menuitem " role="menuitem" id=":z" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Find and replace<!--?lit$944599098$--></div></div><div command="find-next" class="goog-menuitem " role="menuitem" id=":10" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Find next<!--?lit$944599098$--></div></div><div command="find-previous" class="goog-menuitem " role="menuitem" id=":11" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Find previous<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":12" style="user-select: none;"></div><div command="notebook-settings" class="goog-menuitem " role="menuitem" id=":13" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Notebook settings<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":14" style="user-select: none;"></div><div command="clear-outputs" class="goog-menuitem " role="menuitem" id=":15" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Clear all outputs<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="view-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="show-toc-pane" class="goog-menuitem goog-option" role="menuitemcheckbox" aria-checked="false" id=":17" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><div class="goog-menuitem-checkbox" style="user-select: none;"><!----><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>check</md-icon> </div><!--?lit$944599098$-->Table of contents<!--?lit$944599098$--></div></div><div command="show-fileinfo" class="goog-menuitem " role="menuitem" id=":18" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Notebook info<!--?lit$944599098$--></div></div><div command="show-executedcode" class="goog-menuitem " role="menuitem" id=":19" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Executed code history<!--?lit$944599098$--></div></div><div command="toggle-comments-visibility" class="goog-menuitem goog-option" role="menuitemcheckbox" aria-checked="false" id=":1a" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><div class="goog-menuitem-checkbox" style="user-select: none;"><!----><md-icon aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>check</md-icon> </div><!--?lit$944599098$-->Comments sidebar<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1b" style="user-select: none;"></div><div command="collapse-sections" class="goog-menuitem " role="menuitem" id=":1c" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Collapse sections<!--?lit$944599098$--></div></div><div command="expand-sections" class="goog-menuitem " role="menuitem" id=":1d" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Expand sections<!--?lit$944599098$--></div></div><div command="save-section-layout" class="goog-menuitem " role="menuitem" id=":1e" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Save collapsed section layout<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1f" style="user-select: none;"></div><div command="hide-code" class="goog-menuitem " role="menuitem" id=":1g" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Show/hide code<!--?lit$944599098$--></div></div><div command="toggle-output" class="goog-menuitem " role="menuitem" id=":1h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Show/hide output<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1i" style="user-select: none;"></div><div command="focus-next-tab" class="goog-menuitem " role="menuitem" id=":1j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Focus next tab<!--?lit$944599098$--></div></div><div command="focus-previous-tab" class="goog-menuitem " role="menuitem" id=":1k" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Focus previous tab<!--?lit$944599098$--></div></div><div command="move-tab-to-next" class="goog-menuitem " role="menuitem" id=":1l" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Move tab to next pane<!--?lit$944599098$--></div></div><div command="move-tab-to-prev" class="goog-menuitem " role="menuitem" id=":1m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Move tab to previous pane<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="insert-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="insert-cell-below" class="goog-menuitem " role="menuitem" id=":1o" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Code cell<!--?lit$944599098$--></div></div><div command="add-text" class="goog-menuitem " role="menuitem" id=":1p" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Text cell<!--?lit$944599098$--></div></div><div command="add-section-header" class="goog-menuitem " role="menuitem" id=":1q" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Section header cell<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1r" style="user-select: none;"></div><div command="open-scratch-code-cell" class="goog-menuitem " role="menuitem" id=":1s" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Scratch code cell<!--?lit$944599098$--></div></div><div command="snippets" class="goog-menuitem " role="menuitem" id=":1t" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Code snippets<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":1u" style="user-select: none;"></div><div command="add-form-field" class="goog-menuitem " role="menuitem" id=":1v" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Add a form field<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="runtime-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="runall" class="goog-menuitem " role="menuitem" id=":1x" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Run all<!--?lit$944599098$--></div></div><div command="runbefore" class="goog-menuitem " role="menuitem" id=":1y" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Run before<!--?lit$944599098$--></div></div><div command="runfocused" class="goog-menuitem " role="menuitem" id=":1z" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Run the focused cell<!--?lit$944599098$--></div></div><div command="runselected" class="goog-menuitem " role="menuitem" id=":20" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Run selection<!--?lit$944599098$--></div></div><div command="runafter" class="goog-menuitem " role="menuitem" id=":21" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Run after<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":22" style="user-select: none;"></div><div command="interrupt" class="goog-menuitem " role="menuitem" id=":23" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Interrupt execution<!--?lit$944599098$--></div></div><div command="restart" class="goog-menuitem " role="menuitem" id=":24" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Restart session<!--?lit$944599098$--></div></div><div command="restart-and-run-all" class="goog-menuitem " role="menuitem" id=":25" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Restart session and run all<!--?lit$944599098$--></div></div><div command="powerwash-current-vm" class="goog-menuitem " role="menuitem" id=":26" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Disconnect and delete runtime<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":27" style="user-select: none;"></div><div command="change-runtime-type" class="goog-menuitem " role="menuitem" id=":28" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Change runtime type<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":29" style="user-select: none;"></div><div command="manage-sessions" class="goog-menuitem " role="menuitem" id=":2a" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Manage sessions<!--?lit$944599098$--></div></div><div command="open-resource-viewer" class="goog-menuitem " role="menuitem" id=":2b" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->View resources<!--?lit$944599098$--></div></div><div command="view-runtime-logs" class="goog-menuitem " role="menuitem" id=":2c" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->View runtime logs<!--?lit$944599098$--></div></div></div><div class="goog-menu" id="tools-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="show-command-palette" class="goog-menuitem " role="menuitem" id=":2e" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Command palette<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2f" style="user-select: none;"></div><div command="preferences" class="goog-menuitem " role="menuitem" id=":2g" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Settings<!--?lit$944599098$--></div></div><div command="shortcuts" class="goog-menuitem " role="menuitem" id=":2h" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Keyboard shortcuts<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2i" style="user-select: none;"></div><div command="open-differ" class="goog-menuitem " role="menuitem" id=":2j" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Diff notebooks<!--?lit$944599098$--> <span class="screenreader-only" style="user-select: none;"><!--?lit$944599098$-->(opens in a new tab)</span></div></div></div><div class="goog-menu" id="help-menu" role="menu" aria-haspopup="true" style="display: none; user-select: none;"><!--?lit$944599098$--><div command="faq" class="goog-menuitem " role="menuitem" id=":2l" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Frequently asked questions<!--?lit$944599098$--></div></div><div command="view-relnotes" class="goog-menuitem " role="menuitem" id=":2m" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->View release notes<!--?lit$944599098$--></div></div><div command="snippets" class="goog-menuitem " role="menuitem" id=":2n" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Search code snippets<!--?lit$944599098$--></div></div><div class="goog-menuseparator goog-menuitem-disabled" aria-disabled="true" role="separator" id=":2o" style="user-select: none;"></div><div command="report-bug" class="goog-menuitem " role="menuitem" id=":2p" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Report a bug<!--?lit$944599098$--></div></div><div command="report-abuse" class="goog-menuitem " role="menuitem" id=":2q" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Report Drive abuse<!--?lit$944599098$--></div></div><div command="send-feedback" class="goog-menuitem " role="menuitem" id=":2r" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->Send feedback<!--?lit$944599098$--></div></div><div command="view-tos" class="goog-menuitem " role="menuitem" id=":2s" style="user-select: none;"><div class="goog-menuitem-content" style="user-select: none;"><!--?lit$944599098$-->View terms of service<!--?lit$944599098$--></div></div></div><div class="doc-comments-area" style="display: none;"><!----><div class="doc-comments-buttons">
        <md-text-button command="add-comment" role="presentation" value="" has-icon=""><template shadowrootmode="open" shadowrootdelegatesfocus><!---->
      <!--?lit$944599098$-->
      <div class="background"></div>
      <md-focus-ring part="focus-ring" for="button" aria-hidden="true"><template shadowrootmode="open"><!----></template></md-focus-ring>
      <md-ripple part="ripple" for="button" aria-hidden="true"><template shadowrootmode="open"><!----><div class="surface   "></div></template></md-ripple>
      <!--?lit$944599098$--><button id="button" class="button">
      <!--?lit$944599098$-->
      <span class="touch"></span>
      <!--?lit$944599098$--><slot name="icon"></slot>
      <span class="label"><slot></slot></span>
      <!--?lit$944599098$-->
    
    </button>
    </template>
          <md-icon slot="icon" filled="" aria-hidden="true"><template shadowrootmode="open"><!----><slot></slot></template>comment</md-icon>
          <!--?lit$944599098$-->Add a comment
        </md-text-button>
      </div></div><div class="thumbnail"></div><iframe id="apiproxy173790274af347b38122af4ba519a4dec1c3f5bf0.3372708558" name="apiproxy173790274af347b38122af4ba519a4dec1c3f5bf0.3372708558" src="./DataMining_Project3_HSM.ipynb - Colab_files/proxy.html" tabindex="-1" aria-hidden="true" style="width: 1px; height: 1px; position: absolute; top: -100px; display: none;"></iframe><div class="monaco-aria-container"><div class="monaco-alert" role="alert" aria-atomic="true"></div><div class="monaco-alert" role="alert" aria-atomic="true"></div><div class="monaco-status" role="complementary" aria-live="polite" aria-atomic="true"></div><div class="monaco-status" role="complementary" aria-live="polite" aria-atomic="true"></div></div><iframe src="./DataMining_Project3_HSM.ipynb - Colab_files/bscframe.html" style="display: none;"></iframe><div><div class="grecaptcha-badge" data-style="bottomright" style="width: 256px; height: 60px; position: fixed; visibility: hidden; display: block; transition: right 0.3s ease 0s; bottom: 14px; right: -186px; box-shadow: gray 0px 0px 5px; border-radius: 2px; overflow: hidden;"><div class="grecaptcha-logo"><iframe title="reCAPTCHA" width="256" height="60" role="presentation" name="a-jqk3alo2yv84" frameborder="0" scrolling="no" sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-top-navigation allow-modals allow-popups-to-escape-sandbox allow-storage-access-by-user-activation" src="./DataMining_Project3_HSM.ipynb - Colab_files/anchor.html"></iframe></div><div class="grecaptcha-error"></div><textarea id="g-recaptcha-response-100000" name="g-recaptcha-response" class="g-recaptcha-response" style="width: 250px; height: 40px; border: 1px solid rgb(193, 193, 193); margin: 10px 25px; padding: 0px; resize: none; display: none;"></textarea></div><iframe style="display: none;" src="./DataMining_Project3_HSM.ipynb - Colab_files/saved_resource.html"></iframe></div></body></html>ng DataMining_Project3_HSM.ipynb - Colab.html…]()
