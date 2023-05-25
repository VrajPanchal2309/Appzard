<div class="cooked"><p>Basically this is first guide on arduino, by end of this topic you will be able to change Bluetooth Module Name, Password and Know how to connect bluetooth with app.</p>
<p>Let’s get started -</p>
<p>Apparatus -</p>
<ol>
<li>Arduino UNO (I’ve used <a href="https://store-usa.arduino.cc/products/arduino-uno-rev3" rel="noopener nofollow ugc">Arduino Uno Rev3</a>)</li>
<li>Bluetooth Module (I’ve used <a href="https://www.amazon.in/HC-05-Bluetooth-Module-10g/dp/B00X86U4RW" rel="noopener nofollow ugc">HC-05 Bluetooth Module</a>)</li>
<li>
<a href="https://www.amazon.in/ApTechDeals-Jumper-Female-breadboard-jumper/dp/B074J9CPV3/ref=sr_1_4?crid=1HAOGF9JY6T5U&amp;keywords=jumper+wires&amp;qid=1678011827&amp;s=industrial&amp;sprefix=jumper+wires%2Cindustrial%2C289&amp;sr=1-4" rel="noopener nofollow ugc">Jumper Wires</a> for connections.</li>
<li><a href="https://www.arduino.cc/en/software" rel="noopener nofollow ugc">Arduino IDE</a></li>
<li>Little bit knowledge of Python.</li>
</ol>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/4/45f45a74a56351d255fed7c277cc2a5840cbe9db.png" data-download-href="https://community.appzard.com/uploads/default/45f45a74a56351d255fed7c277cc2a5840cbe9db" title="image_2023-03-05_15-55-29"><img src="https://community.appzard.com/uploads/default/optimized/2X/4/45f45a74a56351d255fed7c277cc2a5840cbe9db_2_333x250.png" alt="image_2023-03-05_15-55-29" data-base62-sha1="9YQt8ZPPIc79pIYT9T9D6VdSnmH" srcset="https://community.appzard.com/uploads/default/optimized/2X/4/45f45a74a56351d255fed7c277cc2a5840cbe9db_2_333x250.png, https://community.appzard.com/uploads/default/optimized/2X/4/45f45a74a56351d255fed7c277cc2a5840cbe9db_2_499x375.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/4/45f45a74a56351d255fed7c277cc2a5840cbe9db_2_666x500.png 2x" data-dominant-color="498698" style="aspect-ratio: 333 / 250;" loading="lazy" width="333" height="250"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_15-55-29</span><span class="informations">726×545 44.9 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/c/c0c39e67597b0e5690f711407efd019f17e77ace.png" data-download-href="https://community.appzard.com/uploads/default/c0c39e67597b0e5690f711407efd019f17e77ace" title="image_2023-03-05_15-56-16"><img src="https://community.appzard.com/uploads/default/optimized/2X/c/c0c39e67597b0e5690f711407efd019f17e77ace_2_345x145.png" alt="image_2023-03-05_15-56-16" data-base62-sha1="rvgMHPzD6D1EnKVLCwm6JnDrp5Y" srcset="https://community.appzard.com/uploads/default/optimized/2X/c/c0c39e67597b0e5690f711407efd019f17e77ace_2_345x145.png, https://community.appzard.com/uploads/default/optimized/2X/c/c0c39e67597b0e5690f711407efd019f17e77ace_2_517x217.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/c/c0c39e67597b0e5690f711407efd019f17e77ace_2_690x290.png 2x" data-dominant-color="64958A" style="aspect-ratio: 345 / 145;" loading="lazy" width="345" height="145"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_15-56-16</span><span class="informations">786×331 26.3 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>We’ll Have two parts here -</p>
<details>
<summary>
Part 1 (Connecting Bluetooth With Arduino)</summary>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/c/cbd786a608f04e49c43a7d0101b4f4d0aa11f776.png" data-download-href="https://community.appzard.com/uploads/default/cbd786a608f04e49c43a7d0101b4f4d0aa11f776" title="image_2023-03-05_16-14-20"><img src="https://community.appzard.com/uploads/default/optimized/2X/c/cbd786a608f04e49c43a7d0101b4f4d0aa11f776_2_345x220.png" alt="image_2023-03-05_16-14-20" data-base62-sha1="t5gGHBPWGwNQ5xaen9ExHJLWABM" srcset="https://community.appzard.com/uploads/default/optimized/2X/c/cbd786a608f04e49c43a7d0101b4f4d0aa11f776_2_345x220.png, https://community.appzard.com/uploads/default/optimized/2X/c/cbd786a608f04e49c43a7d0101b4f4d0aa11f776_2_517x330.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/c/cbd786a608f04e49c43a7d0101b4f4d0aa11f776_2_690x440.png 2x" data-dominant-color="9CB9BF" style="aspect-ratio: 345 / 220;" loading="lazy" width="345" height="220"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_16-14-20</span><span class="informations">1081×690 92.9 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>This is the circuit diagram of Bluetooth Module</p>
<p>Next you can find this bluetooth name in your device list on your phone click it to connect and if this device request for password just type 1234(Default Password) in it.<br>
</p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/3/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b.png" data-download-href="https://community.appzard.com/uploads/default/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b" title="image_2023-03-05_17-08-46"><img src="https://community.appzard.com/uploads/default/optimized/2X/3/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b_2_168x375.png" alt="image_2023-03-05_17-08-46" data-base62-sha1="8DTXIjPtDQRmh0RAK0jPY0OpxRF" srcset="https://community.appzard.com/uploads/default/optimized/2X/3/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b_2_168x375.png, https://community.appzard.com/uploads/default/optimized/2X/3/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b_2_252x562.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/3/3c941b0c9bf532b789bc52a0b33d47f4ae1f9a5b_2_336x750.png 2x" style="aspect-ratio: 168 / 375;" loading="lazy" width="168" height="375"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_17-08-46</span><span class="informations">1080×2400 156 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/d/d36283e7d11e88021800a3d3be0707f82d33b39f.jpeg" data-download-href="https://community.appzard.com/uploads/default/d36283e7d11e88021800a3d3be0707f82d33b39f" title="image_2023-03-05_17-09-02"><img src="https://community.appzard.com/uploads/default/optimized/2X/d/d36283e7d11e88021800a3d3be0707f82d33b39f_2_168x375.jpeg" alt="image_2023-03-05_17-09-02" data-base62-sha1="u9ZOtT9VvhD5Nxq5o9aRGkpZJfx" srcset="https://community.appzard.com/uploads/default/optimized/2X/d/d36283e7d11e88021800a3d3be0707f82d33b39f_2_168x375.jpeg, https://community.appzard.com/uploads/default/optimized/2X/d/d36283e7d11e88021800a3d3be0707f82d33b39f_2_252x562.jpeg 1.5x, https://community.appzard.com/uploads/default/optimized/2X/d/d36283e7d11e88021800a3d3be0707f82d33b39f_2_336x750.jpeg 2x" data-dominant-color="2C2C2C" style="aspect-ratio: 168 / 375;" loading="lazy" width="168" height="375"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_17-09-02</span><span class="informations">1080×2400 187 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>After it’s paired once bluetooth will be saved to your ‘Previously Connected Devices’.</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/2/221d78676b71276ee478bb87ccb3ef837cf95fcf.jpeg" data-download-href="https://community.appzard.com/uploads/default/221d78676b71276ee478bb87ccb3ef837cf95fcf" title="Screenshot_20230305_171037"><img src="https://community.appzard.com/uploads/default/optimized/2X/2/221d78676b71276ee478bb87ccb3ef837cf95fcf_2_168x375.jpeg" alt="Screenshot_20230305_171037" data-base62-sha1="4RNnbcx7DFNKnHx9b8z5KsxtCzl" srcset="https://community.appzard.com/uploads/default/optimized/2X/2/221d78676b71276ee478bb87ccb3ef837cf95fcf_2_168x375.jpeg, https://community.appzard.com/uploads/default/optimized/2X/2/221d78676b71276ee478bb87ccb3ef837cf95fcf_2_252x562.jpeg 1.5x, https://community.appzard.com/uploads/default/optimized/2X/2/221d78676b71276ee478bb87ccb3ef837cf95fcf_2_336x750.jpeg 2x" data-dominant-color="080808" style="aspect-ratio: 168 / 375;" loading="lazy" width="168" height="375"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">Screenshot_20230305_171037</span><span class="informations">1080×2400 79.8 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
</details>
<details>
<summary>
Part 2 (Setup with IDE)</summary>
<p>Here you will require Arduino IDE for changing name and password</p>
<p>So let’s get started.</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/e/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb.png" data-download-href="https://community.appzard.com/uploads/default/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb" title="image_2023-03-05_16-26-17"><img src="https://community.appzard.com/uploads/default/optimized/2X/e/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb_2_517x264.png" alt="image_2023-03-05_16-26-17" data-base62-sha1="w2oJWBWTQhKg6TpqnOogoxeoPFN" srcset="https://community.appzard.com/uploads/default/optimized/2X/e/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb_2_517x264.png, https://community.appzard.com/uploads/default/optimized/2X/e/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb_2_775x396.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/e/e08afdcb8c0c6213d1a0e22c8d98d90b74b5ddeb_2_1034x528.png 2x" data-dominant-color="C6CCCC" style="aspect-ratio: 517 / 264;" loading="lazy" width="517" height="264"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_16-26-17</span><span class="informations">1920×981 11.5 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>Here is your IDE</p>
<p>Connect Arduino with your pc / laptop and select port / device in IDE</p>
<p><img src="https://community.appzard.com/uploads/default/original/2X/2/2afc01df0ba46e9cd60039419d4327cbbe75964b.png" alt="image_2023-03-05_16-28-16" data-base62-sha1="68fYzjHpV00v8x3mJe0hpjNApDB" style="aspect-ratio: 301 / 169;" loading="lazy" width="301" height="169"></p>
<p>After this you have to open Serial Monitor</p>
<p><img src="https://community.appzard.com/uploads/default/original/2X/c/c66bb0e16e4ae3a36c350e87104439a4a2c19eae.png" alt="image_2023-03-05_16-29-30" data-base62-sha1="sjjgucYzx70OBUpY1FOac5BTsu2" style="aspect-ratio: 303 / 233;" loading="lazy" width="303" height="233"></p>
<p>Now Change some settings in serial montior</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/2/2df6e55a0f170fe96e22df12b4a68456fa86f3f7.png" data-download-href="https://community.appzard.com/uploads/default/2df6e55a0f170fe96e22df12b4a68456fa86f3f7" title="image_2023-03-05_16-31-13"><img src="https://community.appzard.com/uploads/default/optimized/2X/2/2df6e55a0f170fe96e22df12b4a68456fa86f3f7_2_517x75.png" alt="image_2023-03-05_16-31-13" data-base62-sha1="6yCsplNFE0OvGjsTt5qlRb2aiXR" srcset="https://community.appzard.com/uploads/default/optimized/2X/2/2df6e55a0f170fe96e22df12b4a68456fa86f3f7_2_517x75.png, https://community.appzard.com/uploads/default/optimized/2X/2/2df6e55a0f170fe96e22df12b4a68456fa86f3f7_2_775x112.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/2/2df6e55a0f170fe96e22df12b4a68456fa86f3f7_2_1034x150.png 2x" data-dominant-color="E0E9EA" style="aspect-ratio: 517 / 75;" loading="lazy" width="517" height="75"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image_2023-03-05_16-31-13</span><span class="informations">1920×279 7.72 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
</details>
<details>
<summary>
Part 3 (Changing Name and Password of Bluetooth)</summary>
<p>For this you need to change your bluetooth module Mode to AT(Attention Command) Mode. In this mode you can give commands from serial monitor to bluetooth to change it’s default settings like Name , Password etc.</p>
<p>First,<br>
You have to press and hold the small button on bluetooth module before connecting arduino to the pc / laptop.</p>
<p>If your bluetooth is in At Mode you will be able to notice that the led in bluetooth module keeps fading instead of fastly blinking.</p>
<p>Like this -</p>
<p><a href="https://res.cloudinary.com/dlwbp2or4/video/upload/v1678015546/video_20230305_165327_edit_vwmxnl.mp4" rel="noopener nofollow ugc">https://res.cloudinary.com/dlwbp2or4/video/upload/v1678015546/video_20230305_165327_edit_vwmxnl.mp4 <span class="badge badge-notification clicks" title="1 click">1</span></a></p>
<p>Now in Serial Monitor type AT and press enter.</p>
<p>You will be able to see OK</p>
<p>Next to check your current Name of Bluetooth Module type</p>
<pre class="codeblock-buttons"><div class="codeblock-button-wrapper" style="right: 0px;"><button class="btn nohighlight copy-cmd"><svg class="fa d-icon d-icon-copy svg-icon svg-string" xmlns="http://www.w3.org/2000/svg"><use href="#copy"></use></svg></button></div><code class="hljs language-undefined">AT +NAME?
</code></pre>
<p>Press Enter.</p>
<p>Here you will be able to see your current name of bluetooth</p>
<pre class="codeblock-buttons"><div class="codeblock-button-wrapper" style="right: 0px;"><button class="btn nohighlight copy-cmd"><svg class="fa d-icon d-icon-copy svg-icon svg-string" xmlns="http://www.w3.org/2000/svg"><use href="#copy"></use></svg></button></div><code class="hljs language-undefined">AT +PSWD?
</code></pre>
<p>Is for knowing your password</p>
<pre class="codeblock-buttons"><div class="codeblock-button-wrapper" style="right: 0px;"><button class="btn nohighlight copy-cmd"><svg class="fa d-icon d-icon-copy svg-icon svg-string" xmlns="http://www.w3.org/2000/svg"><use href="#copy"></use></svg></button></div><code class="hljs language-bash">AT +NAME=<span class="hljs-string">"Your Bluetooth Name"</span>
</code></pre>
<p>This will change name of your bluetooth module</p>
<pre class="codeblock-buttons"><div class="codeblock-button-wrapper" style="right: 0px;"><button class="btn nohighlight copy-cmd"><svg class="fa d-icon d-icon-copy svg-icon svg-string" xmlns="http://www.w3.org/2000/svg"><use href="#copy"></use></svg></button></div><code class="hljs language-bash">AT +PSWD=<span class="hljs-string">"Enter your password you want to change"</span>
</code></pre>
<p>You can change to any password you like.</p>
</details>
<p>So here our guide ends further guides for connecting apps with arduino will be shared in new topics. Till then have a nice day <img src="http://community.appzard.com/images/emoji/google/slightly_smiling_face.png?v=12" title=":slightly_smiling_face:" class="emoji" alt=":slightly_smiling_face:" loading="lazy" style="aspect-ratio: 20 / 20;" width="20" height="20"></p>
<p>Stay Safe Stay Healthy</p></div>
