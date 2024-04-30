# Publication-statistics


 Obtain publication statistics for a given institution or author using OpenAlex and Google Scholar.
This repo contains two main scripts, [Author_statistics.ipynb]([url](https://github.com/boumpteryx/Publication-statistics/blob/main/Author_Statistics.ipynb)) 
<a target="_blank" href="https://colab.research.google.com/github/boumpteryx/Publication-statistics/blob/main/Author_Statistics.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open Author In Colab"/>
</a>
and [Institution_statistics.ipynb]([url](https://github.com/boumpteryx/Publication-statistics/blob/main/Institution_Statistics.ipynb)). 
<a target="_blank" href="https://colab.research.google.com/github/boumpteryx/Publication-statistics/blob/main/Institution_Statistics.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open Institution In Colab"/>
</a>
Run the author one if you want to obtain information about a specific author, possibly only as an affiliate to a specific institution. Run the institution one if you want to focus on information regarding a whole institution.

Two databases are used. OpenAlex is free to use and of very high quality. It contains a lot of information about author affiliation and topics for example. However, it only covers peer-reviewed publications such as full journal papers. Abstracts, ArXiv papers and the like will most likely not appear. Google Scholar includes all types of publications but with very few information about any one of them. We only use Scholar for publication and citation statistics. 

Instructions are detailed in the notebooks about how to find proper author and institution IDs. In order to query Google Scholar, we use the SerpAPI which requires an API key. My key is present as a default but will run out pretty quickly. Consider setting up your own key and possible getting a paid plan to run the scripts in full.

Another long step is collecting all the works an author has cited from OpenAlex. For a big institution this may take a whole day. This only happens towards the end of the script so that you may access quickly most of the statistics. 

There is a parameter to save all computed statistics as .csv, .json and .png files. Since these files are numerous and sometimes a bit heavy, the parameter save is by default set to ```False```; set it to ```True``` to get everything saved in your local folder.
 

