# Tech Basics - Assignment 8

### Download Dataset From Kaggle Using Terminal

* Go to [kaggle.com](https://www.kaggle.com/) and create a new account (skip if you already have a Kaggle account)
* In order to download the data, you need to be logged in into Kaggle
* One solution is to export your cookies and tell wget to use your cookies when downloading the data
* Use this plugin on chrome to get cookie data from  [link](https://chrome.google.com/webstore/detail/cookietxt-export/lopabhfecdfhgogdbojmaicoicjekelh)
* Save it as `cookies.txt`. If you are doing on server you will have to upload the `cookies.txt` on your server
* Now use wget to download files
`wget -x -c --load-cookies cookies.txt -P data -nH --cut-dirs=5 https://www.kaggle.com/c/diabetic-retinopathy-detection/download/trainLabels.csv.zip
`
* Above command will use your exported cookies to download the file to a folder called data
