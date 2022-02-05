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
<pre><code>k6 run --vus 10 --duration 30s script.js</code></pre>
