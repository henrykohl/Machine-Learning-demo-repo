# jobot (How to Build an AI: The Chronicles of Jobot)

An AI developed by Jovian using cutting edge ML APIs and models

[Vercel Deployment](https://vercel.com/tayuan-hsus-projects/jobot-dev)

- Jobot Github Branch
  > e1-first-contact-with-jobot -- Ep1
  >
  > user-login -- Ep2
  >
  > blog-template -- Ep3

## (12/17/2024)

- [Episode 1 - First Contact with Jobot](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-1-first-contact-with-jobot)
  > [Lecture Jupyter Notebook in Github](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/jovian/how-to-build-an-ai/first_contact_with_jobot.ipynb)
  >
  > [Lecture Video - Episode 1 - First Contact with Jobot | How to Build an AI](https://www.youtube.com/watch?v=UiT5ueCEDww)

* 要執行時，將`./backup-files`中的要時執行的 **js**檔複製到 `./jobot-web/pages` 中，並改名為 `index.js`，與 Github 同步後，即可在 [vercel](https://vercel.com/tayuan-hsus-projects/jobot-dev) 執行此專案

* 需要安裝
  > - 安裝 **Tailwind**
  >
  > - 安裝 **Prettier**

- `/backup-files/single.js` 源自 [single-response.js](https://github.com/gopinav/ai/blob/main/examples/javascript-vanilla/single-response.js) 與 [index.html](https://github.com/gopinav/ai/blob/main/examples/javascript-vanilla/index.html)

  > 原本 (在上面 `index.html`)
  >
  > ```html
  > <p id="resultText" class="whitespace-pre-line"></p>
  > ```
  >
  > 改為 (在`/backup-files/single.js`)
  >
  > ```html
  > <div id="resultText" class="whitespace-pre-line">
  >   <div>...</div>
  > </div>
  > ```
  >
  > 原 `<p></p>` tag 改成 `<div></div>` tag，因為在 `<p></p>` tag 中插入 `<div></div>` tag, 就會出現 `React Minified Error #418` in the Inspector 的錯誤(在瀏覽器的開發模式)

- `/backup-files/stream.js` 源自 [stream-response.js](https://github.com/gopinav/ai/blob/main/examples/javascript-vanilla/stream-response.js) 與 [index.html](https://github.com/gopinav/ai/blob/main/examples/javascript-vanilla/index.html)

  > 注意
  >
  > ```javascript
  > const generate = async () => {
  >   ...
  >     /* eslint-disable no-constant-condition (必需加此行，否則會出現Unexpected constant condition)*/
  >     while (true) {
  >       ...
  >     }
  >   ...
  > }
  > ```
  >
  > [`Unexpected constant condition` -- solution](https://stackoverflow.com/questions/63697757/i-get-this-error-unexpected-constant-condition-no-constant-condition-and-cant-fi)

* `/backup-files/timestamp.txt`
  > 完成專案不同階段的版本說明，含 Lecture 使用的 測試輸入內容

- `/backup-files/stream_output.txt`
  > 儲存了，使用 `/backup-files/stream.js` 運行，輸入 `Hey, how are you today?` 後，decoder.decode(value) 也就是 const chunk 的結果

* `./backup-files/index_single.js` 是 Lecture 中主專案的最後完整檔 （無 Streaming 功能）

* `./backup-files/index_stream.js` (Bonus: Streaming the Message)

  > 注意需要安裝 `2.0.0` 的版本，可使用 `npm install eventsource-parser@2.0.0 --save`
  >
  > 如果直接在 terminal 執行 `npm install eventsource-parser` ，會安裝 3.0.0 版本（12/20/2024 最新版）
  >
  > > 則程式執行後沒有結果，原因在於`parser.feed()`根本不會執行

* `./backup-files/index_F.js` 是在學習 Lecture 的過程中，所以編輯內容（含 Streaming）

* `./backup-files/stream_js.js` 是純 js 版的 stream 測試程式(可在 playcode.io 或 Codepen.io 執行)

  > 不需要安裝 **React**，只需要安裝 **eventsource-parser** 2.0.0 版本，即可運行
  >
  > `const apiKey` 是 空的(為了安全起見) ，需要改成可用的 OpenAI Api Key

* `index.js` 是 `./backup-files/index_stream.js` (12/22/2024)

## (1/4/2025)

- [Episode 2 - Jobot Meets the World](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-2-jobot-meets-the-world)

  > [Lecture Jupyter Notebook in Github](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/jovian/how-to-build-an-ai/e2_jobot_meets_the_world.ipynb)
  >
  > [Lecture Video - Episode 2 - Jobot Meets the World | How to Build an AI](https://www.youtube.com/watch?v=iRc-7tzayMo)

---

- ${\color{red}{以下內容，沒有跟著實做，因為Lecture中，演示非一步步操作實現(跳過很多步驟)，只有瀏覽過}}$

* [Episode 3 - Jobot Learns New Tricks](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-3-jobot-learns-new-tricks)

  > [No Lecture Jupyter Notebook in Github]
  >
  > [Lecture Video - Jobot Learns Prompt Engineering | How to Build an AI - Ep 3](https://www.youtube.com/watch?v=uzKZjsRgX-Q)

* [Episode 4 - Jobot Makes New Friends](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-4-jobot-makes-new-friends)

  > [No Lecture Jupyter Notebook in Github]
  >
  > [Lecture Video - Episode 4 - Jobot Makes New Friends | How to Build an AI](https://www.youtube.com/watch?v=ZpD18odmZb4)

* [Episode 5 - Jobot Enters the Matrix](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-5-jobot-enters-the-matrix)

  > [No Lecture Jupyter Notebook in Github]
  >
  > [Lecture Video - Episode 5 - Jobot Enters the Matrix | How to Build an AI](https://www.youtube.com/watch?v=CgINtC_9rTk)

* [Episode 6 - Jobot's Trip Down Memory Lane](https://jovian.com/learn/how-to-build-an-ai/lesson/episode-6-jobots-trip-down-memory-lane)

  > [No Lecture Jupyter Notebook in Github]
  >
  > [Lecture Video - Episode 6 - Jobot's Trip Down Memory Lane | How to Build an AI](https://www.youtube.com/watch?v=Q2GSfcjr0QE)

* [Optional Ep - Building Custom AI Powered Apps with ChatGPT](https://jovian.com/learn/how-to-build-an-ai/lesson/building-ai-powered-apps-with-chatgpt)
  > [Source code in Github](https://github.com/aakashns/buildaiapps-live/)
  >
  > [Lecture Jupyter Notebook in Github](https://github.com/henrykohl/Machine-Learning-demo-repo/blob/master/jovian/how-to-build-an-ai/build-ai-apps-live.ipynb)
  >
  > [Lecture Video - How to Build your AI-Powered App with ChatGPT | Step-by-Step Framework for Deployment](https://www.youtube.com/watch?v=Y1IJU_hN0LM)
  >
  > ${\color{red}{Unfortunately,\ the\ library - \`usellm\` -\ has\ been\ down\ for\ some\ unknown\ reason.}}$
  >
  > > ${\color{red}{在 Lecture Video 中, (39:47) 發現 usellm 已經無法使用，所以此時間點之後的操作，已經實現不了！}}$
