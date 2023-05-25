<div class="cooked"><p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/7/7523e647960e652878101b85d71781cb6e9dffa8.jpeg" data-download-href="https://community.appzard.com/uploads/default/7523e647960e652878101b85d71781cb6e9dffa8" title="image"><img src="https://community.appzard.com/uploads/default/optimized/2X/7/7523e647960e652878101b85d71781cb6e9dffa8_2_354x375.jpeg" alt="image" data-base62-sha1="gIgMghLRNYSjg2gqfFvmY1qt2Bi" srcset="https://community.appzard.com/uploads/default/optimized/2X/7/7523e647960e652878101b85d71781cb6e9dffa8_2_354x375.jpeg, https://community.appzard.com/uploads/default/optimized/2X/7/7523e647960e652878101b85d71781cb6e9dffa8_2_531x562.jpeg 1.5x, https://community.appzard.com/uploads/default/optimized/2X/7/7523e647960e652878101b85d71781cb6e9dffa8_2_708x750.jpeg 2x" data-dominant-color="5E6951" style="aspect-ratio: 354 / 375;" loading="lazy" width="354" height="375"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">1080×1144 197 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p><strong>Want to create custom notification to statusBar like this ??</strong></p>
<p>Follow next,</p>
<p><strong>Requirements -</strong></p>
<ol>
<li>Little bit knowledge of xml</li>
<li>Android Studio</li>
<li>Curiosity <img src="http://community.appzard.com/images/emoji/google/wink.png?v=12" title=":wink:" class="emoji" alt=":wink:" loading="lazy" style="aspect-ratio: 20 / 20;" width="20" height="20">
</li>
</ol>
<p><strong>Let’s get started</strong></p>
<details>
<summary>
Step 1 (Component Section)</summary>
<p>Import some components.</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/6/6947e949b3a34cadd70e0c9271298f8380d760ab.png" data-download-href="https://community.appzard.com/uploads/default/6947e949b3a34cadd70e0c9271298f8380d760ab" title="image"><img src="https://community.appzard.com/uploads/default/optimized/2X/6/6947e949b3a34cadd70e0c9271298f8380d760ab_2_474x375.png" alt="image" data-base62-sha1="f1mcCEXR0HvGJ04UiFdTQE3QXzR" srcset="https://community.appzard.com/uploads/default/optimized/2X/6/6947e949b3a34cadd70e0c9271298f8380d760ab_2_474x375.png, https://community.appzard.com/uploads/default/optimized/2X/6/6947e949b3a34cadd70e0c9271298f8380d760ab_2_711x562.png 1.5x, https://community.appzard.com/uploads/default/original/2X/6/6947e949b3a34cadd70e0c9271298f8380d760ab.png 2x" data-dominant-color="E5EAED" style="aspect-ratio: 474 / 375;" loading="lazy" width="474" height="375"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">923×730 60.4 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
</details>
<details>
<summary>
Step 2  (Xml Section)</summary>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/8/886db8c21b9ca3c20c07b340b62a8a8041c9271e.png" data-download-href="https://community.appzard.com/uploads/default/886db8c21b9ca3c20c07b340b62a8a8041c9271e" title="image"><img src="https://community.appzard.com/uploads/default/optimized/2X/8/886db8c21b9ca3c20c07b340b62a8a8041c9271e_2_690x255.png" alt="image" data-base62-sha1="jsU0QwDUlJkHoyDd3YkWF3kJUXY" srcset="https://community.appzard.com/uploads/default/optimized/2X/8/886db8c21b9ca3c20c07b340b62a8a8041c9271e_2_690x255.png, https://community.appzard.com/uploads/default/optimized/2X/8/886db8c21b9ca3c20c07b340b62a8a8041c9271e_2_1035x382.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/8/886db8c21b9ca3c20c07b340b62a8a8041c9271e_2_1380x510.png 2x" data-dominant-color="435D83" style="aspect-ratio: 690 / 255;" loading="lazy" width="690" height="255"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">1679×621 86.5 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>In your android studio create any design.</p>
<p>Example -</p>
<pre class="codeblock-buttons"><div class="codeblock-button-wrapper" style="right: 0px;"><button class="btn nohighlight copy-cmd"><svg class="fa d-icon d-icon-copy svg-icon svg-string" xmlns="http://www.w3.org/2000/svg"><use href="#copy"></use></svg></button></div><code class="hljs language-bash">&lt;ImageView
        android:<span class="hljs-built_in">id</span>=<span class="hljs-string">"@+id/image"</span>
        android:layout_width=<span class="hljs-string">"match_parent"</span>
        android:layout_height=<span class="hljs-string">"match_parent"</span>
        android:scaleType=<span class="hljs-string">"fitXY"</span>
        android:src=<span class="hljs-string">"@mipmap/ic_launcher"</span> /&gt;

    &lt;TextView
        android:<span class="hljs-built_in">id</span>=<span class="hljs-string">"@+id/text"</span>
        android:layout_width=<span class="hljs-string">"match_parent"</span>
        android:layout_height=<span class="hljs-string">"match_parent"</span>
        android:text=<span class="hljs-string">"Hii, this is a custom image notification with text.
        This notification is built by Vraj Panchal and made on Appzard
        by using Notification Style component.
        How is this notification ??
        Thankyou 😊😊"</span>
        android:textColor=<span class="hljs-string">"#151515"</span>
        android:textSize=<span class="hljs-string">"17dp"</span>
        android:textStyle=<span class="hljs-string">"bold"</span> /&gt;
</code></pre>
</details>
<details>
<summary>
Step 3 (Xml in notepad)</summary>
<p>Copy paste your xml from android studio to notepad into relative view like this -</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/a/a869e93a9459d6ed4bb791552b4c1f8c92f30bce.png" data-download-href="https://community.appzard.com/uploads/default/a869e93a9459d6ed4bb791552b4c1f8c92f30bce" title="image"><img src="https://community.appzard.com/uploads/default/original/2X/a/a869e93a9459d6ed4bb791552b4c1f8c92f30bce.png" alt="image" data-base62-sha1="o1R7XCB2a2AYy7cHbzHkQGW1QDQ" data-dominant-color="333742" style="aspect-ratio: 690 / 243;" loading="lazy" width="690" height="243"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">1867×658 19.3 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>and save file as .xml</p>
</details>
<details>
<summary>
Step 4 (Final Setup)</summary>
<p>Import .xml file in asset.</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/e/edb501999a6638bc3456220ed0dd62fa7f6a1da0.png" data-download-href="https://community.appzard.com/uploads/default/edb501999a6638bc3456220ed0dd62fa7f6a1da0" title="image"><img src="https://community.appzard.com/uploads/default/original/2X/e/edb501999a6638bc3456220ed0dd62fa7f6a1da0.png" alt="image" data-base62-sha1="xUQXNURiOSypMfa2LgFX3W0qxwI" data-dominant-color="F2F5FC" style="aspect-ratio: 345 / 225;" loading="lazy" width="345" height="225"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">756×495 3.51 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>Then,</p>
<p>In Notification Style component , set custom notification source to .xml file</p>
<p><img src="https://community.appzard.com/uploads/default/original/2X/b/b5ac51dc322c2161d08f42d0102911ba77003d0a.png" alt="image" data-base62-sha1="pV9CaaeevWmFxklQLc0j0bSbkvg" style="aspect-ratio: 227 / 54;" loading="lazy" width="227" height="54"></p>
</details>
<details>
<summary>
Step 5 (Blocks Section)</summary>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/b/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5.png" data-download-href="https://community.appzard.com/uploads/default/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5" title="blocks (11)"><img src="https://community.appzard.com/uploads/default/optimized/2X/b/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5_2_517x65.png" alt="blocks (11)" data-base62-sha1="qs8gcXGoujJdavFSZtHXoUFfEYB" srcset="https://community.appzard.com/uploads/default/optimized/2X/b/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5_2_517x65.png, https://community.appzard.com/uploads/default/optimized/2X/b/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5_2_775x97.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/b/b966a6bbd4d7e01aa592b1c881c53fda9684e4e5_2_1034x130.png 2x" data-dominant-color="7E56A0" style="aspect-ratio: 517 / 65;" loading="lazy" width="517" height="65"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">blocks (11)</span><span class="informations">1594×202 11.2 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/f/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e.png" data-download-href="https://community.appzard.com/uploads/default/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e" title="blocks (12)"><img src="https://community.appzard.com/uploads/default/optimized/2X/f/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e_2_516x120.png" alt="blocks (12)" data-base62-sha1="AhHxeATeejWddi4TQsraV4AXuuG" srcset="https://community.appzard.com/uploads/default/optimized/2X/f/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e_2_516x120.png, https://community.appzard.com/uploads/default/optimized/2X/f/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e_2_774x180.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/f/fe4e88bb9f12c2f3f2ec6535f1fcf8cffde0ff0e_2_1032x240.png 2x" data-dominant-color="A45673" style="aspect-ratio: 516 / 120;" loading="lazy" width="516" height="120"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">blocks (12)</span><span class="informations">1206×282 12.5 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>Here, viewId is set to “image” because in your xml file you set ImageView id to image.</p>
<p><img src="https://community.appzard.com/uploads/default/original/2X/2/2f130bc84453b8a05cfccb6677b32e4ee5254f0a.jpeg" alt="image" data-base62-sha1="6IrfjAiLuvtkdWDScDgBWvCLFdU" style="aspect-ratio: 425 / 141;" loading="lazy" width="425" height="141"></p>
<p>Next,<br>
</p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/e/ee28023258fa88658328eea59259acd531190dbd.png" data-download-href="https://community.appzard.com/uploads/default/ee28023258fa88658328eea59259acd531190dbd" title="blocks (13)"><img src="https://community.appzard.com/uploads/default/optimized/2X/e/ee28023258fa88658328eea59259acd531190dbd_2_517x130.png" alt="blocks (13)" data-base62-sha1="xYPm4ielkZ5J2bx8AMOGc4QDJet" srcset="https://community.appzard.com/uploads/default/optimized/2X/e/ee28023258fa88658328eea59259acd531190dbd_2_517x130.png, https://community.appzard.com/uploads/default/optimized/2X/e/ee28023258fa88658328eea59259acd531190dbd_2_775x195.png 1.5x, https://community.appzard.com/uploads/default/optimized/2X/e/ee28023258fa88658328eea59259acd531190dbd_2_1034x260.png 2x" data-dominant-color="904F87" style="aspect-ratio: 517 / 130;" loading="lazy" width="517" height="130"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">blocks (13)</span><span class="informations">1124×284 13.5 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
<p>Same here viewId is set to “text” as you have set TextView id to text in your xml file.</p>
<p></p><div class="lightbox-wrapper"><a class="lightbox" href="https://community.appzard.com/uploads/default/original/2X/8/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f.jpeg" data-download-href="https://community.appzard.com/uploads/default/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f" title="image"><img src="https://community.appzard.com/uploads/default/optimized/2X/8/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f_2_517x77.jpeg" alt="image" data-base62-sha1="jJq9jTrkEER6dFXJsSGOY2NAAP5" srcset="https://community.appzard.com/uploads/default/optimized/2X/8/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f_2_517x77.jpeg, https://community.appzard.com/uploads/default/optimized/2X/8/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f_2_775x115.jpeg 1.5x, https://community.appzard.com/uploads/default/optimized/2X/8/8a4bbbe98162ef4b1b261aafa2fdc8eedb9ee29f_2_1034x154.jpeg 2x" data-dominant-color="2F323C" style="aspect-ratio: 517 / 77;" loading="lazy" width="517" height="77"><div class="meta">
<svg class="fa d-icon d-icon-far-image svg-icon" aria-hidden="true"><use href="#far-image"></use></svg><span class="filename">image</span><span class="informations">1280×192 39.7 KB</span><svg class="fa d-icon d-icon-discourse-expand svg-icon" aria-hidden="true"><use href="#discourse-expand"></use></svg>
</div></a></div><p></p>
</details>
<p><strong>Yup Completed</strong></p>
<p><a href="https://drive.google.com/file/d/1XrHv7l5QamLBbD9cjdJZModYg7XObrE8/view?usp=sharing" rel="noopener nofollow ugc">CustomNotificationStyle.xml</a><br>
<a href="https://drive.google.com/file/d/1qMI9xGAKCpS13NdrqdtbXdumLpaD5zUl/view?usp=sharing" rel="noopener nofollow ugc">TestNotification.apk</a></p>
<p><strong>You can try creating more codes like this one and post your work here.</strong></p>
<p><strong>Kindness multiplies Kindness, So be Kind <img src="http://community.appzard.com/images/emoji/google/slightly_smiling_face.png?v=12" title=":slightly_smiling_face:" class="emoji" alt=":slightly_smiling_face:" loading="lazy" style="aspect-ratio: 20 / 20;" width="20" height="20"></strong></p>
<details>
<summary>
Some Useful Links -</summary>
<p><a href="https://appzard.com/" rel="noopener nofollow ugc">Appzard Home <span class="badge badge-notification clicks" title="1 click">1</span></a><br>
<a href="https://developer.android.com/develop/ui/views/notifications/custom-notification" rel="noopener nofollow ugc">Custom Notification Layout Android Studio</a><br>
<a href="https://stackoverflow.com/questions/41888161/how-to-create-a-custom-notification-layout-in-android" rel="noopener nofollow ugc">Custom Notification Layout StackOverFlow</a><br>
<a href="https://medium.com/degoo/android-creating-a-custom-notification-layout-with-an-image-or-photo-bd282637a04e" rel="noopener nofollow ugc">Custom Notification Layout Degoo <span class="badge badge-notification clicks" title="1 click">1</span></a></p>
</details></div>
