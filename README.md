<p align="center">
   <a href="https://yay.space/">
      <img src="Yay-logo.jpg" width="10%" alt="Yay_BtCl" />
   </a>
  <h1 align="center">Yay_BtCl</h1>
</p>

<p align="center">
      <a href="https://travis-ci.com/TanakashiXr/Yay_BtCl"><img alt="Build Status" src="https://travis-ci.com/TanakashiXr/Yay_BtCl.svg?token=hQziw2chDyu4Ysu1ptd9&branch=master" /></a>
      <a href="https://github.com/TanakashiXr/Yay_BtCl"><img alt="release (latest by date including pre-releases)" src="https://img.shields.io/github/v/release/TanakashiXr/Yay_BtCl?include_prereleases" /></a>
      <a href="https://github.com/TanakashiXr/Yay_BtCl/blob/master/LICENSE"><img alt="LICENSE" src="https://img.shields.io/badge/License-MIT%20License-blue.svg" /></a>
      <a href="https://www.python.org/downloads/"><img alt="Supported python versions: 3.x.x" src="https://img.shields.io/badge/Python-3.x.x-green.svg" /></a>
</p>

<p align="center">
こちらは当ソースコードの説明になります。ご使用前に必ずご覧ください。<br>
This is the description of this source code. Please read before use.
</p>

## Requirement / 動作条件

* Python 3.x.x
* Selenium 3.x.x
* ChromeDriver 80.x.x.x
* Google Chrome 80.x.x.x

## Install / インストール

当プログラムを使用するには上記、動作条件を満たす必要があります。  
To use this program, you must meet the above requirements.

最初に必要なパッケージをインストールします。Python3のインストールも同時に行ってください。  
Install the required packages first.At this point, install Python3 yourself.
```sh
$ yum -y install libX11 GConf2 fontconfig unzip wget
```

ChromeDriverを公式サイトからダウンロードしてインストールします。  
Download and install ChromeDriver from the official website.
```sh
$ wget https://chromedriver.storage.googleapis.com/80.0.3987.106/chromedriver_linux64.zip
$ unzip chromedriver_linux64.zip
$ mv chromedriver /usr/local/bin/
$ chmod 755 /usr/local/bin/chromedriver
```

GoogleChromeをインストールします。  
Install GoogleChrome.
```sh
$ vi /etc/yum.repos.d/google-chrome.repo
----- 以下を書き込む（Write the following） -----
[google-chrome]
name=google-chrome
baseurl=http://dl.google.com/linux/chrome/rpm/stable/x86_64
enabled=1
gpgcheck=1
gpgkey=https://dl.google.com/linux/linux_signing_key.pub
----------------------------------------------

$ yum -y install google-chrome-stable libOSMesa
```

必ずChromeDriverとGoogleChromeのバージョンを確認してください。  
Be sure to check the version of ChromeDriver and GoogleChrome.
```sh
$ google-chrome --version
Google Chrome 80.0.3987.132
$ chromedriver --version
ChromeDriver 80.0.3987.106
```

Seleniumをインストールします。  
Install Selenium.
```sh
$ pip install selenium
```

当ソースコードをダウンロードし、解凍します。  
Download and unzip this source code.
Install Selenium.
```sh
$ git clone https://github.com/TanakashiXr/Yay_BtCl.git
$ cd Yay_BtCl
```

## Usage / 使用方法

各自の環境に合わせて編集を行ってください。  
Edit according to your environment.
```sh
$ vi auto_clicker.py
$ python auto_clicker.py
```

## Features / 機能

* 自動いいね
* 自動レター
* 半ボット

## Author / 作者

* たなか氏

## License / ライセンス

このソフトウェアは、MITライセンスの下でリリースされています。ライセンスを参照してください。  
This software is released under the MIT License, see LICENSE.
