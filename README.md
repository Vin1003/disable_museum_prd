# 针对残障人士的智能博物馆设施

| 发布日期   | 2019.12.15    |
| ---------- | --- |
| 文件名称   | 针对残障人士的智能博物馆设施  |
| 文件现状   | 完善中    |
| 文件的主人 | 林咏妍    |
| 设计师     | 林咏妍    |
| 开发者     | 林咏妍    |
| 测试者     | 林咏妍    |

## 目标

针对聋、哑、盲的残障人士设计相应的博物馆的智能设施，方便他们在博物馆进行参观和使用基础设施。但由于目前技术限制，每种设施只考虑一种残障情况。对于有两种及两种以上残疾情况的残障人士，必须有监护人在旁进行协助。

## 背景和战略契合处

- 背景：大多数博物馆目前并没有针对残障人士进行相应的设施配套，尤其是大型博物馆，如故宫博物院。残障人士进入博物馆参观十分困难。

- 战略契合处：

              1.目前国内大多数博物馆都没有与之相关的配套设施。
 
              2.聋、哑、盲等残障人士参观博物馆时，拥有较大的参观障碍。

              3.保护博物馆内设施和其他人参观不受影响。

## 假设条件

- 用户在使用手机时：

1.使用手机可以进行知识图谱的查看，方便聋哑人士进行展品信息的查看。

2.盲人可以对着手机说出自己的话，语料库自动识别，调出相应的语料进行回复。

3.讲解员可以通过实时讲解，语音识别调出图像，方便聋人进行展品的参观。

4.聋哑盲人士为了不给其他参观者造成影响，可以事先查看展厅人流量，规划路线。

## 需求

| #   | 标题     | 用户故事                                                                                    | 重要性 | 笔记                                                     |
| --- | -------- | ------------------------------------------------------------------------------------------- | ------ | -------------------------------------------------------- |
| 1   | 语音识别 | 盲人说出自己的话，语音识别后调出相应语料进行回复                                            | 必须有 | 语音识别后，文字信息会通过语音合成传送到盲人耳朵里       |
| 2   | 知识图谱 | 聋哑人单独拿着手机参观时，对着手机打开博物馆APP界面进行展品信息的查看，帮助他们更好进行参观 | 必须有 | 知识图谱可查看展品的各种信息，在无法听取讲解的情况下进行展品信息查看 |
| 3   | 统计人流量 | 用户可以查看博物馆内展厅的人流量，错峰参观                                                        | 必须有 | 残障人士可根据目前的人流量选择一个人不那么多的展厅进行参观                                   |

## PRD价值主张

![针对残疾人的博物馆](https://images.gitee.com/uploads/images/2019/1219/002525_b5fbce41_1532294.png "残疾人博物馆.png")

### PRD1 加值宣言

1.百度AI平台短语音识别API进行语音识别，支持普通话和略带口音的中文识别；支持粤语、四川话方言识别。

2.百度AI平台在线语音合成API进行语音合成，提供REST API接口、在线离线融合SDK，满足不同网络环境下的语音合成需求，提供流畅自然的合成体验.

3.百度AI平台实体标注API结合上下文，识别文本中的实体并将其关联到百科知识库中的唯一实体对象，同时输出实体在当前上下文最合适的上位概念，以达到对文本中的实体进行辨别的作用。

4.百度AI平台人流量统计API进行人流量统计，面向展厅、通道等出入口场景，以头肩为识别目标，进行人体检测和追踪，根据目标轨迹判断进出区域方向，实现动态人数统计，返回区域进出人数。

5.微软azure语言理解API：在用户对话的自然语言文本中应用自定义机器学习智能，以便预测整体含义并提炼出相关的详细信息。

### PRD2 核心价值

#### 百度AI平台

- 短语音识别：支持普通话和略带口音的中文识别；支持粤语、四川话方言识别，支持英文识别；支持50多个领域的语义理解，如：天气，交通，娱乐等。根据语音内容理解可以将数字序列、小数、时间、分数、基础运算符正确转换为数字格式，使得识别的数字结果更符合使用习惯，直观自然；使用大规模数据集训练语言模型，根据语音的内容理解和停顿智能匹配合适的标点符号（包括，。！？），使识别结果的表现方式贴合表述，更加可懂。

- 在线语音合成：提供基础音库和精品音库共9种音库供您选择，适用于泛阅读、订单播报、智能硬件等应用场景，支持多种参数配置，可根据场景需求对音库的语速、音调、音量进行灵活设置，满足个性化需求，中文多音字可通过标注拼音、音调自行定义发音，例如“轻舟已过万重（chong2）山”、“脑筋急转（zhuan3）弯”。

- 实体标注：基于百科知识库，将实体链接到知识库中的实体，可用于搜索、推荐、广告、对话等多种场景下的知识解析任务，进而更好的解决应用问题。

- 人流量统计：实时监测机场、车站、展会、展馆、景区、学校、体育场等公共场所的人流量，及时导流、限流，预警核心区域人群过于密集等安全隐患。

#### 微软azure

- 语言理解（LUIS）：LUIS 的客户端应用程序可以是任何传统的应用程序，只要其能够以自然语言与用户通信并完成任务即可。 这些客户端应用程序包括社交媒体应用、聊天机器人以及支持语音的桌面应用程序。

### PRD3 核心价值与用户痛点

- **痛点一：盲人无法知道语音识别的键在哪里。**

    语音识别的键设计得比较大，让盲人可以按住按钮就能进行语音识别，无需手动操作，可以通过语音直接对手机发布指令。

- **痛点二：聋人无法听到语音识别，不知道自己说了什么。**

    语音识别后，语音会转换成文字。语音合成恢复后，也会转换成文字在手机页面上显示出来。

- **痛点三：聋人无法听讲解员讲解。**

    通过知识图谱查看展品基本信息，及时跟上进度。

### PRD4 人工智能概率性与用户痛点

- 短语音识别API：采用领先国际的流式端到端语音语言一体化建模方法，融合百度自然语言处理技术，近场中文普通话识别准确率达98%。

- 语音合成API：基于业界领先的深度神经网络技术，提供高度拟人、流畅自然的语音合成服务，让您的应用、设备开口说话，更具个性。

- 实体标注API：结合百科知识库及文本上下文语境，可将文本中的实体关联到百科知识库中唯一的实体对象。 

- 人流量统计API:基于区域人流量统计技术模型，为场馆提供了完善的区域人数统计方案——当区域人数超过限定数值时，系统会自动预警，帮助馆内辅助设施和工作人员及时实行疏散策略，保障潜在的参观者聚集区域长期安全通畅。

### PRD5 需求列表与人工智能API加值

#### 核心功能排序

1.语音识别：用户对着手机说出自己需要的服务，语音识别后转文字有15秒的时间让用户进行确认；语音提取关键字后进行语言理解识别，调出相应语料进行回复，文字回复后进行语音合成进行语音回复。

- 短语音识别：用户说出自己所需的服务后进行语音转文字，并有15秒的时间进行文字的确认。

- 语言理解：在用户对话的自然语言文本种预测整体含义并提炼出相关的详细信息，调出语料库中相应语料进行回复。

- 语音合成：文字语料回复后进行在线语音合成，传达到用户耳中。

2.知识图谱：用户通过手机查看展品基本信息，了解展品及展览

- 实体标注：用户通过手机查看展品基本信息，并将知识图谱进行语音播报。

3.查看人流量：用户在手机中进行人流量的查看，安排自己的观展路线。

- 人流量统计：动态人流量统计后，每十分种更新一次展厅内人数，反馈到服务器，显示在APP页面上。

## 原型

### 原型1 交互及界面设计

![语音识别](https://images.gitee.com/uploads/images/2019/1218/230948_2970d96c_1532294.png "语音识别.png")

![知识图谱](https://images.gitee.com/uploads/images/2019/1218/231008_4c537e47_1532294.png "知识图谱.png")

![查看人流量](https://images.gitee.com/uploads/images/2019/1218/231047_8744ae01_1532294.png "查看人流.png")

图一运用了短语音识别API，当短语音被识别后，会转化成文字给用户15秒的时间进行审核，审核不通过重新进行识别。15秒后将会语音会被提取关键字进行查找，提取处相关语料进行回答，并进行语音合成返回到用户耳中。

图二运用了知识图谱API，提供相关展品信息给用户查看，方便用户进行信息的了解。

图三运用了人流量统计API，能让用户实时看到展厅人数，规划参观路线。

### 原型2 信息设计

![语音识别](https://images.gitee.com/uploads/images/2019/1218/231552_8ffefadb_1532294.png "语音识别.png")

运用了短语音识别API、语音合成API、语言理解API，用户通过按住说话，提取语音关键信息，设备进行语言理解，提取出相关语料进行语音合成进行回复。

### 原型3 原型文档

https://vin1003.github.io/disable_museum_prd/


### 原型4 口头操作说明 

在进入APP首页后，用户可自行选择所需的服务，语音识别的“按住说话”键设计得比较大，且按下去会有微震的感觉，盲人也可以自行操作。查看人流量十分钟更新一次数据，用户可以根据各展厅的人数进行参观路线规划。在参观时，可以打开知识图谱进行展品信息的了解，利于聋哑人士在无法听取讲解员讲解时了解展品信息。

## API产品使用关键AI或机器学习之API的输出入展示

### API1 使用水平

- 短语音识别API：语音识别[示例Demo代码]( https://github.com/Baidu-AIP/speech-demo)


```
import sys
import json
import base64
import time

IS_PY3 = sys.version_info.major == 3

if IS_PY3:
    from urllib.request import urlopen
    from urllib.request import Request
    from urllib.error import URLError
    from urllib.parse import urlencode
    timer = time.perf_counter
else:
    from urllib2 import urlopen
    from urllib2 import Request
    from urllib2 import URLError
    from urllib import urlencode
    if sys.platform == "win32":
        timer = time.clock
    else:
        # On most other platforms the best timer is time.time()
        timer = time.time

API_KEY = 'kVcnfD9iW2XVZSMaLMrtLYIz'
SECRET_KEY = 'O9o1O213UgG5LFn0bDGNtoRN3VWl2du6'

# 需要识别的文件
AUDIO_FILE = './audio/16k.pcm'  # 只支持 pcm/wav/amr 格式，极速版额外支持m4a 格式
# 文件格式
FORMAT = AUDIO_FILE[-3:]  # 文件后缀只支持 pcm/wav/amr 格式，极速版额外支持m4a 格式

CUID = '123456PYTHON'
# 采样率
RATE = 16000  # 固定值

# 普通版

DEV_PID = 1536  # 1537 表示识别普通话，使用输入法模型。1536表示识别普通话，使用搜索模型。根据文档填写PID，选择语言及识别模型
ASR_URL = 'http://vop.baidu.com/server_api'
SCOPE = 'audio_voice_assistant_get'  # 有此scope表示有asr能力，没有请在网页里勾选，非常旧的应用可能没有

#测试自训练平台需要打开以下信息， 自训练平台模型上线后，您会看见 第二步：“”获取专属模型参数pid:8001，modelid:1234”，按照这个信息获取 dev_pid=8001，lm_id=1234
# DEV_PID = 8001 ;   
# LM_ID = 1234 ;
通用票据识别API:识别小票和发票接口说明
""" 读取图片 """
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

image = get_file_content('example.jpg')

""" 调用通用文字识别, 图片参数为本地图片 """
client.basicGeneral(image);

""" 如果有可选参数 """
options = {}
options["language_type"] = "CHN_ENG"
options["detect_direction"] = "true"
options["detect_language"] = "true"
options["probability"] = "true"

""" 带参数调用通用文字识别, 图片参数为本地图片 """
client.basicGeneral(image, options)

url = "https//www.x.com/sample.jpg"

""" 调用通用文字识别, 图片参数为远程url图片 """
client.basicGeneralUrl(url);

""" 如果有可选参数 """
options = {}
options["language_type"] = "CHN_ENG"
options["detect_direction"] = "true"
options["detect_language"] = "true"
options["probability"] = "true"

""" 带参数调用通用文字识别, 图片参数为远程url图片 """
client.basicGeneralUrl(url, options)
货币识别API：识别货币接口说明
""" 读取图片 """
def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

image = get_file_content('example.jpg')

""" 调用通用物体识别 """
client.advancedGeneral(image);

""" 如果有可选参数 """
options = {}
options["baike_num"] = 5

""" 带参数调用通用物体识别 """
client.advancedGeneral(image, options)
```

- 在线语音合成API：语音合成后，将声音传到用户耳中。

```
import sys
import json

IS_PY3 = sys.version_info.major == 3
if IS_PY3:
    from urllib.request import urlopen
    from urllib.request import Request
    from urllib.error import URLError
    from urllib.parse import urlencode
    from urllib.parse import quote_plus
else:
    import urllib2
    from urllib import quote_plus
    from urllib2 import urlopen
    from urllib2 import Request
    from urllib2 import URLError
    from urllib import urlencode

API_KEY = '4E1BG9lTnlSeIf1NQFlrSq6h'
SECRET_KEY = '544ca4657ba8002e3dea3ac2f5fdd241'

TEXT = "欢迎使用百度语音合成。"

# 发音人选择, 基础音库：0为度小美，1为度小宇，3为度逍遥，4为度丫丫，
# 精品音库：5为度小娇，103为度米朵，106为度博文，110为度小童，111为度小萌，默认为度小美 
PER = 4
# 语速，取值0-15，默认为5中语速
SPD = 5
# 音调，取值0-15，默认为5中语调
PIT = 5
# 音量，取值0-9，默认为5中音量
VOL = 5
# 下载的文件格式, 3：mp3(default) 4： pcm-16k 5： pcm-8k 6. wav
AUE = 3

FORMATS = {3: "mp3", 4: "pcm", 5: "pcm", 6: "wav"}
FORMAT = FORMATS[AUE]

CUID = "123456PYTHON"

TTS_URL = 'http://tsn.baidu.com/text2audio'


class DemoError(Exception):
    pass


"""  TOKEN start """

TOKEN_URL = 'http://openapi.baidu.com/oauth/2.0/token'
SCOPE = 'audio_tts_post'  # 有此scope表示有tts能力，没有请在网页里勾选


def fetch_token():
    print("fetch token begin")
    params = {'grant_type': 'client_credentials',
              'client_id': API_KEY,
              'client_secret': SECRET_KEY}
    post_data = urlencode(params)
    if (IS_PY3):
        post_data = post_data.encode('utf-8')
    req = Request(TOKEN_URL, post_data)
    try:
        f = urlopen(req, timeout=5)
        result_str = f.read()
    except URLError as err:
        print('token http response http code : ' + str(err.code))
        result_str = err.read()
    if (IS_PY3):
        result_str = result_str.decode()

    print(result_str)
    result = json.loads(result_str)
    print(result)
    if ('access_token' in result.keys() and 'scope' in result.keys()):
        if not SCOPE in result['scope'].split(' '):
            raise DemoError('scope is not correct')
        print('SUCCESS WITH TOKEN: %s ; EXPIRES IN SECONDS: %s' % (result['access_token'], result['expires_in']))
        return result['access_token']
    else:
        raise DemoError('MAYBE API_KEY or SECRET_KEY not correct: access_token or scope not found in token response')


"""  TOKEN end """

if __name__ == '__main__':
    token = fetch_token()
    tex = quote_plus(TEXT)  # 此处TEXT需要两次urlencode
    print(tex)
    params = {'tok': token, 'tex': tex, 'per': PER, 'spd': SPD, 'pit': PIT, 'vol': VOL, 'aue': AUE, 'cuid': CUID,
              'lan': 'zh', 'ctp': 1}  # lan ctp 固定参数

    data = urlencode(params)
    print('test on Web Browser' + TTS_URL + '?' + data)

    req = Request(TTS_URL, data.encode('utf-8'))
    has_error = False
    try:
        f = urlopen(req)
        result_str = f.read()

        headers = dict((name.lower(), value) for name, value in f.headers.items())

        has_error = ('content-type' not in headers.keys() or headers['content-type'].find('audio/') < 0)
    except  URLError as err:
        print('asr http response http code : ' + str(err.code))
        result_str = err.read()
        has_error = True

    save_file = "error.txt" if has_error else 'result.' + FORMAT
    with open(save_file, 'wb') as of:
        of.write(result_str)

    if has_error:
        if (IS_PY3):
            result_str = str(result_str, 'utf-8')
        print("tts api  error:" + result_str)

    print("result saved as :" + save_file)
```

- 实体标注：进行展品信息的标注

目前无可调用的SDK,目前调用接口需付费

- 人流量统计：进行动态人流量统计

```
import requests
import base64

'''
人流量统计
'''

request_url = "https://aip.baidubce.com/rest/2.0/image-classify/v1/body_num"
# 二进制方式打开图片文件
f = open('[本地文件]', 'rb')
img = base64.b64encode(f.read())

params = {"image":img}
access_token = '[调用鉴权接口获取的token]'
request_url = request_url + "?access_token=" + access_token
headers = {'content-type': 'application/x-www-form-urlencoded'}
response = requests.post(request_url, data=params, headers=headers)
if response:
    print (response.json())
```

- 语言理解：构建属于博物馆的语料库，进行回复

```
########### Python 3.6 #############
   # -*- coding: utf-8 -*-

   import http.client, sys, os.path, json

   # Authoring key, available in https://luis.azure.cn under Account Settings
   LUIS_authoringKey  = "YOUR-AUTHORING-KEY"

   # ID of your LUIS app to which you want to add an utterance
   LUIS_APP_ID      = "YOUR-APP-ID"

   # The version number of your LUIS app
   LUIS_APP_VERSION = "0.1"

   # Update the host if your LUIS subscription is not in the China East region
   LUIS_HOST       = "chinaeast2.api.cognitive.azure.cn"

   # uploadFile is the file containing JSON for utterance(s) to add to the LUIS app.
   # The contents of the file must be in this format described at: https://aka.ms/add-utterance-json-format
   UTTERANCE_FILE   = "./utterances.json"
   RESULTS_FILE     = "./utterances.results.json"

   # LUIS client class for adding and training utterances
   class LUISClient:
      
      # endpoint method names
      TRAIN    = "train"
      EXAMPLES = "examples"

      # HTTP verbs
      GET  = "GET"
      POST = "POST"

      # Encoding
      UTF8 = "UTF8"

      # path template for LUIS endpoint URIs
      PATH     = "/luis/api/v2.0/apps/{app_id}/versions/{app_version}/"

      # default HTTP status information for when we haven't yet done a request
      http_status = 200
      reason = ""
      result = ""

      def __init__(self, host, app_id, app_version, key):
         self.key = key
         self.host = host
         self.path = self.PATH.format(app_id=app_id, app_version=app_version)

      def call(self, luis_endpoint, method, data=""):
         path = self.path + luis_endpoint
         headers = {'Ocp-Apim-Subscription-Key': self.key}
         conn = http.client.HTTPSConnection(self.host)
         conn.request(method, path, data.encode(self.UTF8) or None, headers)
         response = conn.getresponse()
         self.result = json.dumps(json.loads(response.read().decode(self.UTF8)),
                                    indent=2)
         self.http_status = response.status
         self.reason = response.reason
         print(self.result)
         return self

      def add_utterances(self, filename=UTTERANCE_FILE):
         with open(filename, encoding=self.UTF8) as utterance:
               data = utterance.read()
         return self.call(self.EXAMPLES, self.POST, data)
         
      def train(self):
         return self.call(self.TRAIN, self.POST)

      def status(self):
         return self.call(self.TRAIN, self.GET)

      def print(self):
         if self.result:
               print(self.result)
         return self

      def raise_for_status(self):
         if 200 <= self.http_status < 300:
               return self
         raise http.client.HTTPException("{} {}".format(
               self.http_status, self.reason))

   if __name__ == "__main__":

      luis = LUISClient(LUIS_HOST, LUIS_APP_ID, LUIS_APP_VERSION,
                        LUIS_authoringKey)

      try:
         print("Adding utterance(s).")
         luis.add_utterances().raise_for_status()

         print("Requesting training.")
         luis.train().raise_for_status()

         print("Requesting training status.")
         luis.status().raise_for_status()

      except Exception as ex:
         luis.print()    # JSON response may have more details
         print("{0.__name__}: {1}".format(type(ex), ex))
```

### API2 使用分析比较

- face++与百度AI平台都有手势识别API，但是百度AI平台的手势识别API能识别24种手势，而face++只能识别19种，因此选择百度AI平台。

- 中国科学技术馆已使用百度AI平台的人流量统计API，并作为成功案例展示在百度AI平台页面上。

[展馆可以更“聪明”！百度大脑AI智慧场馆落地中国科技馆](https://ai.baidu.com/customer/cdstm)

- 虽然百度AI平台的语音合成有基础音频库，但考虑到博物馆的特殊性，因此需要用微软azure构建属于博物馆的语料库。

### API3 使用后风险报告

- 实体标注API接口调用需付费，博物馆需要注意费用及接口调用次数。

- 百度的百科知识库并没有过多的展品信息，有些展品信息需要博物馆去补充。

### API4 加分项

使用了百度AI平台的短语音识别API，在线语音合成API，实体标注API和人流量识别API，以及微软azure的语言理解API。
