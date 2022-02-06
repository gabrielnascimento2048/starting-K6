![download](https://user-images.githubusercontent.com/93552647/152650021-b0f0a5a9-f778-4acf-a69b-d17eaa54f713.png)
# Starting-K6                                                                                                                      
>
> Base documentation: https://k6.io/docs/

## First Steps

### Install

need administrator access do run using POWERSHELL or CMD. 
Before install check if have installed chocolatey.
#### 1. for install: 
<pre><code>choco install k6</code></pre>

#### 2. for run the script: 
<pre><code>k6 run file_name.js</code></pre>

#### 3. for run with many users --VUS (virtual users) --duration (how long does this script run): 
<pre><code>k6 run --vus 10 --duration 30s file_name.js</code></pre>

#### 4. define metrics you can change the metrics '--summary-trend-stats' can also define differents time values unit using (seconds, milliseconds or microseconds) with '--summary-time-unit'  : 
<pre><code>k6 run --summary-trend-stats="min,avg,med,p(99),p(99.9),max,count" --summary-time-unit=ms  file_name.js
</code></pre>






<div align="center">

![download (1)](https://user-images.githubusercontent.com/93552647/152675277-5438e153-f098-476e-9594-0b86b3d7ad89.png)

</div>

# Postman-to-k6
>
> git clone for this project, currently maintence for apideck_libraries, fork of the original grafana project: 
```shell 
 git clone https://github.com/apideck-libraries/postman-to-k6 
 ```
>
## Installation

### Install in local machine

```shell
 npm install -D @apideck/postman-to-k6
```

>Note that this will require you to run the converter with >`npx @apideck/postman-to-k6 your-postman-file` or, if you >are
>using an older versions of npm, >`./node_modules/.bin/postman-to-k6 your-postman-file`.
>run this command inside the folder where the collection.



and

```shell
 npm install -g @apideck/postman-to-k6
```

## Usage

To convert an exported collection to a k6 script:
>note: run this command inside the folder where the collection.

```shell
 postman-to-k6 your_collection.json -o k6-script.js
```

Then run the script in k6, expect to create libs files with your code already converted as usual and them using:

```shell
 k6 run k6-script.js
```



