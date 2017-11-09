# zebra

[![Build Status](https://travis-ci.org/tietang/zebra.png?branch=master)](<https://travis-ci.org/tietang/zebra>)
 
一个基于golang动态网关，提供动态路由和负载均衡，容错。
详情请查看[wiki](<https://github.com/tietang/zebra/wiki>)。


## 特征：

- 支持3种启动配置
	- 通过ini文件
	- 通过zookeeper
	- 通过consul
- 支持多种配置管理
	- ini文件
	- zookeeper
	- consul
	- sql
- 支持多种服务发现
	- Eureka
	- Consul
	- Kubernetes
	- zookeeper，规划中...
	- etcd，规划中...
- 基于服务发现的动态路由
- 负载均衡
	- 简单轮询
	- 加权轮询
	- 随机
	- 一致性hash
	- 基于响应时间使用fibonacci加权轮询
- 简单监控
- 隔离降级&限流
	- hystrix熔断
	- 失败次数算法
- metrics

# 下载

下载Zebra，为预览版0.2



## Mac OS X

 <div class="icon pull-left"><svg xmlns="http://www.w3.org/2000/svg" viewbox="0 0 128 150" width="75" height="75">
  <path fill="#000" fill-rule="nonzero" d="M124.47 116.895c-2.268 5.24-4.954 10.064-8.065 14.5-4.24 6.045-7.712 10.23-10.388 12.554-4.148 3.814-8.593 5.768-13.352 5.88-3.416 0-7.536-.973-12.333-2.946-4.81-1.963-9.234-2.935-13.277-2.935-4.24 0-8.79.97-13.653 2.934-4.872 1.973-8.797 3-11.798 3.102-4.564.195-9.113-1.815-13.653-6.037-2.897-2.528-6.522-6.862-10.865-13-4.66-6.556-8.49-14.157-11.49-22.824C2.38 98.766.77 89.7.77 80.926c0-10.053 2.172-18.723 6.523-25.99 3.42-5.835 7.968-10.438 13.662-13.818 5.693-3.38 11.845-5.102 18.47-5.212 3.624 0 8.378 1.122 14.285 3.325 5.89 2.212 9.673 3.333 11.33 3.333 1.24 0 5.443-1.31 12.566-3.924 6.736-2.425 12.42-3.43 17.078-3.034 12.62 1.02 22.1 5.994 28.406 14.956-11.286 6.84-16.87 16.417-16.758 28.705.1 9.57 3.574 17.536 10.397 23.86 3.092 2.935 6.546 5.203 10.388 6.814-.833 2.418-1.713 4.732-2.648 6.955zM95.526 3c0 7.502-2.74 14.506-8.203 20.99-6.592 7.706-14.566 12.16-23.213 11.457-.11-.9-.174-1.847-.174-2.843 0-7.2 3.135-14.908 8.702-21.21 2.78-3.19 6.315-5.844 10.602-7.96C87.517 1.35 91.564.196 95.37 0c.11 1.002.156 2.005.156 3z"></path>
</svg>
</div>
  
<ul>
      <li><a href="https://github.com/tietang/zebra/releases/download/v0.2-pre/zebra_darwin_amd64-0.2-pre.tar.gz">v0.2-pre-64-bit</a></li>
</ul>

##  Linux
 <div class="row">
      <div class="col-md-12 download">
        <div class="icon pull-left"><svg xmlns="http://www.w3.org/2000/svg" viewbox="0 0 544 664" width="75" height="75">
  <defs>
    <lineargradient id="a" x1="49.181%" x2="49.482%" y1="115.284%" y2="41.252%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="b" x1="47.425%" x2="41.754%" y1="2.019%" y2="90.126%">
      <stop stop-color="#FFF" stop-opacity=".8" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="c" x1="46.201%" x2="49.215%" y1="87.917%" y2="9.628%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="d" x1="51.73%" x2="49.844%" y1="85.418%" y2="13.617%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="e" x1="46.558%" x2="41.366%" y1="2.882%" y2="93.366%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="f" x1="70.346%" x2="64.553%" y1="5.94%" y2="94.063%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="g" x1="50%" x2="50%" y1="89.843%" y2="40.625%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="h" x1="43.569%" x2="45.399%" y1="98.882%" y2="23.094%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="i" x1="50%" x2="50.4%" y1="13.171%" y2="94.634%">
      <stop stop-color="#FFF" stop-opacity=".8" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="j" x1="50.8%" x2="51.6%" y1="37.436%" y2="92.821%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="k" x1="50%" x2="50%" y1="2.344%" y2="81.25%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="l" x1="57.152%" x2="57.142%" y1="2.344%" y2="71.875%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="m" x1="60.793%" x2="46.264%" y1="51.06%" y2="100.24%">
      <stop stop-color="#FFA63F" offset="0%"></stop>
      <stop stop-color="#FF0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="n" x1="94.027%" x2="19.452%" y1="129.341%" y2="-67.53%">
      <stop stop-color="#FFEED7" offset="0%"></stop>
      <stop stop-color="#BDBFC2" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="o" x1="50.09%" x2="40.875%" y1="34.285%" y2="100.443%">
      <stop stop-color="#FFA63F" offset="0%"></stop>
      <stop stop-color="#FF0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="p" x1="-30.509%" x2="15.632%" y1="9.949%" y2="94.191%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="q" x1="43.398%" x2="48.705%" y1="2.218%" y2="102.569%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="r" x1="46.741%" x2="86.742%" y1="-3.616%" y2="75.858%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="s" x1="50%" x2="50.826%" y1="17.631%" y2="99.339%">
      <stop stop-color="#FFA63F" offset="0%"></stop>
      <stop stop-color="#FF0" offset="100%"></stop>
    </lineargradient>
    <lineargradient id="t" x1="55.881%" x2="55.392%" y1="3.119%" y2="94.531%">
      <stop stop-color="#FFF" stop-opacity=".65" offset="0%"></stop>
      <stop stop-color="#FFF" stop-opacity="0" offset="100%"></stop>
    </lineargradient>
  </defs>
  <g fill="none" fill-rule="evenodd">
    <path fill="#000" fill-rule="nonzero" d="M111.235 528.542c-27.985-40.278-33.442-171.23 31.86-251.787 32.357-38.648 40.612-65.58 43.163-101.74 1.736-41.225-29.156-164.304 87.354-173.68C391.62-8.08 385.282 108.41 384.602 170.052c-.563 52.05 38.218 81.552 64.746 122.12 49.1 74.537 44.946 202.874-9.25 272.34-68.645 86.96-127.44 49.247-166.486 52.412-73.117 4.002-75.534 42.988-162.377-88.382z"></path>
    <path fill="url(#a)" fill-rule="nonzero" d="M443.264 299.383c-20.53 18.382-74.476 101.638 8.168 154.99 29.137 18.584-27.473 87.52-53.69 53.41-46.25-61.22-14.814-157.315 13.95-191.512 19.546-24.25 49.034-33.35 31.572-16.88z" transform="matrix(-1 0 0 1 843.1 6)"></path>
    <path fill="#000" fill-rule="nonzero" stroke="#000" stroke-width="1.566" d="M390.554 288.337c33.41 26.996 94.238 122.038 5.516 183.773-29.14 19.247 25.823 79.94 56.684 48.895 107.302-107.91-2.8-231.996-40.7-274.654-33.873-37.09-63.878 8.77-21.5 41.99z"></path>
    <path fill="url(#b)" fill-rule="nonzero" d="M338.348 63.578c0 20.035-14.11 38.547-37.016 48.565-22.906 10.017-51.127 10.017-74.033 0-22.91-10.018-37.02-28.53-37.02-48.565 0-30.97 33.14-56.077 74.03-56.077s74.03 25.11 74.03 56.08z" transform="rotate(2.1 245.8 181)"></path>
    <path fill="url(#c)" fill-rule="nonzero" d="M240.512 134.393c0 20.15-10.582 36.486-23.634 36.486-13.053 0-23.634-16.34-23.634-36.49 0-13.04 4.505-25.08 11.817-31.6 7.32-6.52 16.33-6.52 23.64 0 7.31 6.514 11.82 18.56 11.82 31.594z" transform="rotate(-3.4 231.7 62.9)"></path>
    <path fill="url(#d)" fill-rule="nonzero" d="M329.64 133.672c0 23.28-14.668 42.152-32.764 42.152-18.096 0-32.766-18.872-32.766-42.152 0-15.06 6.245-28.976 16.383-36.505 10.138-7.53 22.628-7.53 32.765 0 10.138 7.53 16.383 21.445 16.383 36.505z" transform="matrix(-1 0 0 1 595.6 -4.4)"></path>
    <path fill="#000" fill-rule="nonzero" d="M283.36 140.28c-.283 12.775 6.153 23.28 14.374 23.462 8.22.182 15.115-10.028 15.398-22.804.183-8.264-2.485-15.964-7-20.2-4.513-4.233-10.188-4.36-14.885-.328-4.697 4.03-7.704 11.604-7.887 19.87zm-52.122.493c1.223 10.556-2.603 19.67-8.545 20.36-5.94.687-11.75-7.312-12.97-17.868-.792-6.83.528-13.376 3.462-17.176 2.933-3.8 7.034-4.28 10.758-1.25 3.724 3.03 6.505 9.1 7.295 15.93z"></path>
    <path fill="url(#e)" fill-rule="nonzero" d="M299.932 133.182c0 7.16-3.9 12.966-8.713 12.966-4.82 0-8.72-5.805-8.72-12.966 0-4.632 1.66-8.912 4.354-11.23 2.696-2.315 6.017-2.315 8.713 0 2.695 2.318 4.356 6.598 4.356 11.23z" transform="matrix(-1 -.1 -.1 1 598.2 29.6)"></path>
    <path fill="url(#f)" fill-rule="nonzero" d="M222 135.095c0 6.003-2.91 10.87-6.497 10.87-3.59 0-6.498-4.867-6.498-10.87 0-3.884 1.24-7.473 3.25-9.415 2.01-1.942 4.486-1.942 6.497 0 2.01 1.942 3.25 5.53 3.25 9.415z" transform="rotate(-6.6 224.1 98.7)"></path>
    <path fill="url(#g)" fill-rule="nonzero" d="M150.83 356.05c16.046-36.377 50.144-100.28 50.87-149.696 0-39.303 117.724-48.69 127.172-9.448 9.447 39.242 33.426 98.104 48.687 126.445 15.26 28.34 59.76 118.37 12.35 196.94-42.7 69.558-172.16 124.58-241.26-9.444-23.26-46.51-19.11-104.143 2.18-154.786z" transform="translate(4.2 .7)"></path>
    <path fill="url(#h)" fill-rule="nonzero" d="M144.186 328.062c-15.698 24.774-49.48 90.528 16.917 133.288 71.517 45.48 64.774 126.777-21.753 80.923-79.135-41.52-31.84-179.96-6.286-211.943 16.875-22.484 41.67-49.674 11.122-2.268z" transform="rotate(-4.2 165.1 371.4)"></path>
    <path fill="#000" fill-rule="nonzero" stroke="#000" stroke-width="1.563" d="M152.295 300.345c-21.83 35.635-74.22 119.766-4.11 163.404 94.46 57.94 67.716 115.88-18.5 63.71C8.3 454.63 114.905 307.94 163.6 252.04c55.555-62.75 10.693 11.36-11.305 48.3z"></path>
    <path fill="url(#i)" fill-rule="nonzero" d="M360.848 369.86c0 39.713-38.115 91.3-103.552 90.837-67.485.558-96.29-51.124-96.29-90.837s44.766-71.943 99.922-71.943 99.92 32.23 99.92 71.943z" transform="translate(4.2 .7)"></path>
    <path fill="url(#j)" fill-rule="nonzero" d="M325.24 244.87c-.728 41.16-27.51 50.87-61.406 50.87s-58.5-6.077-61.406-50.87c0-28.08 27.51-44.328 61.406-44.328 33.895 0 61.405 16.25 61.405 44.33z" transform="translate(4.2 .7)"></path>
    <path fill="url(#k)" fill-rule="nonzero" d="M120.31 308.09c22.145-33.746 68.77-85.456 8.72 7.265-48.687 76.304-18.002 125.34-2.178 138.8 45.658 40.7 43.707 67.935 7.993 46.506-77.03-45.78-61.043-122.81-14.535-192.57z" transform="translate(4.2 .7)"></path>
    <path fill="url(#l)" fill-rule="nonzero" d="M440.78 321.895c-19.146-39.626-80.165-139.877 2.91-23.254 75.576 105.38 22.527 178.77 13.08 186.04-9.446 7.27-41.42 21.8-31.974-3.63 9.446-25.433 56.543-73.715 15.986-159.145z" transform="translate(4.2 .7)"></path>
    <path fill="url(#m)" fill-rule="nonzero" stroke="#E68C3F" stroke-width="7.813" d="M103.598 633.646C53.045 606.876-20.467 638.8 6.22 566.064c5.345-16.548-7.968-41.26.727-57.408 10.173-19.622 31.975-15.26 45.056-28.342C64.9 466.7 73.076 443.252 97.058 446.886c23.98 3.634 39.93 33.076 56.68 69.036 12.353 25.798 56.176 62.08 53.312 90.948-3.37 44.375-53.784 52.737-103.452 26.776z" transform="translate(4.2 .7)"></path>
    <path fill="url(#n)" fill-rule="nonzero" d="M471.962 442.628c-1.972 16.49-23.484 50.735-45.585 53.984-22.466 3.533-43.562-22.55-48.62-47.085-6.486-27.282 14.81-38.136 47.17-37.492 34.953 1.095 48.605 9.197 47.035 30.593z" transform="rotate(21.8 424.5 465.9)"></path>
    <path fill="url(#o)" fill-rule="nonzero" stroke="#E68C3F" stroke-width="7.816" d="M422.002 627.53c-51.36-29.677-124.144 7.05-96.017-69.88 5.886-16.44-8.197-42.208.447-58.46 10.115-19.748 32.065-14.674 45.07-27.84 12.823-13.7 23.398-35.058 47.24-31.4 23.84 3.657 37.254 31.047 53.906 67.238 12.282 25.963 53.954 61.606 51.107 90.66-3.35 44.66-53.096 57.202-101.753 29.682z" transform="matrix(-.9 .4 .4 .9 613 -118.3)"></path>
    <path fill="url(#p)" fill-rule="nonzero" d="M392.175 569.75c-87.022-60.14-47.576-74.215-37.052-85.16 10.377-11.39 18.934-29.147 38.228-26.107 19.3 3.04 30.15 25.813 43.63 55.9 9.94 21.586 43.305 51.164 41.358 75.373-2.63 28.354-48.463 5.74-86.154-20.005z" transform="matrix(-.9 .4 .4 .9 566.8 -119.7)"></path>
    <path fill="url(#q)" fill-rule="nonzero" d="M92.513 572.445c-87.02-60.142-47.062-76.947-34.138-85.01 15.486-10.4 15.244-32.246 34.538-29.206 19.292 3.04 30.9 27.3 44.374 57.39 9.94 21.58 43.304 51.16 41.357 75.37-2.63 28.35-48.44 7.19-86.13-18.55z" transform="rotate(1 67.3 776.8)"></path>
    <path fill="#000" fill-rule="nonzero" d="M471.258 462.296c-6.524 11.77-33.848 30.69-52.308 26.13-18.832-4.462-27.666-30.75-24.28-50.792 3.083-22.56 23.195-23.97 48.597-13.233 27.315 11.9 35.674 22.32 27.99 37.9z"></path>
    <path fill="url(#r)" fill-rule="nonzero" d="M448.335 444.335c-1.148 9.137-13.67 28.11-26.536 29.91-13.08 1.958-25.36-12.494-28.31-26.087-3.777-15.116 8.62-21.13 27.46-20.774 20.342.607 28.29 5.096 27.38 16.95z" transform="rotate(20.1 420.6 463.2)"></path>
    <path fill="url(#s)" fill-rule="nonzero" stroke="#E68C3F" stroke-width="4.688" d="M214.897 160.906c8.933-8.462 31.013-33.832 72.45-7.194 7.703 5.013 13.953 5.472 28.777 11.82 29.657 12.185 15.477 41.573-15.93 51.384-13.447 4.362-25.67 20.695-50.16 19.3-20.92-1.222-26.4-14.844-39.25-22.383-22.835-12.89-26.205-30.318-13.874-39.567 12.333-9.248 17.156-12.573 17.987-13.36z" transform="translate(4.2 .7)"></path>
    <path stroke="#E68C3F" stroke-width="3.125" d="M320.718 185.25c-12.354.727-39.242 27.615-67.583 27.615-28.34 0-45.055-26.16-49.415-26.16"></path>
    <path fill="url(#t)" fill-rule="nonzero" d="M228.98 158.587c4.49-4.033 18.644-15.1 37.416-3.77 3.955 2.244 8.04 4.685 14.113 8.02 12.03 6.998 6.07 17.083-8.35 23.464-6.54 2.68-17.327 8.59-25.538 8.18-9.125-.84-15.03-6.79-21.077-10.663-11.094-7.33-10.42-13.246-5.267-18.173 3.896-3.383 8.28-6.674 8.694-7.05z" transform="translate(4.2 .7)"></path>
  </g>
</svg>
</div>
 
 <ul> 
     <li><a href="https://github.com/tietang/zebra/releases/download/v0.2-pre/zebra_linux_amd64-0.2-pre.tar.gz">v0.2-pre-64-bit</a></li>
     
 </ul>
  
    
    
    
## Windows 

<div class="icon pull-left"><svg xmlns="http://www.w3.org/2000/svg" viewbox="0 0 150 150" width="75" height="75">
  <path fill="#009bef" fill-rule="nonzero" d="M0 21.387l61.34-8.39v59.075H0m68.73-60.24L150 0v71.575H68.73M0 78.322h61.34v59.246L0 129.008M68.73 79.11H150V150l-81.27-11.473"></path>
</svg>
</div>

<ul>
    <li><a href="https://github.com/tietang/zebra/releases/download/v0.2-pre/zebra_windows_386-0.2-pre.zip">0.1.0-pre-32-bit</a></li>
    <li><a href="https://github.com/tietang/zebra/releases/download/v0.2-pre/zebra_windows_amd64-0.2-pre.zip">0.1.0-pre-64-bit</a></li>
</ul>





 
