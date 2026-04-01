# 浣撻噸杩借釜 Weight Tracker

涓€涓畝娲佷紭闆呯殑浣撻噸璁板綍搴旂敤锛屾敮鎸?**Android** 鍜?**Windows 11** 璺ㄥ钩鍙拌繍琛屻€?
## 鍔熻兘鐗规€?
- 鉁?姣忔棩浣撻噸璁板綍
- 鉁?瓒嬪娍鏇茬嚎鍥惧彲瑙嗗寲
- 鉁?7澶?30澶?鍏ㄩ儴鏁版嵁瑙嗗浘鍒囨崲
- 鉁?鐩爣浣撻噸璁剧疆锛堝弻鍑荤洰鏍囧崱鐗囷級
- 鉁?鍘嗗彶璁板綍绠＄悊锛堟敮鎸佸垹闄わ級
- 鉁?鏁版嵁鏈湴瀛樺偍锛坙ocalStorage锛?- 鉁?PWA 鏀寔锛堝彲瀹夎鍒颁富灞忓箷锛?- 鉁?鍝嶅簲寮忚璁★紙鎵嬫満/骞虫澘/妗岄潰锛?- 鉁?绂荤嚎鍙敤

## 浣跨敤鏂规硶

### Windows 11

1. **鐩存帴鎵撳紑**
   - 鍙屽嚮 `index.html` 鐢ㄦ祻瑙堝櫒鎵撳紑
   - 鎴栫敤 VS Code Live Server 鎻掍欢杩愯

2. **瀹夎涓哄簲鐢紙鎺ㄨ崘锛?*
   - 鍦?Edge 鎴?Chrome 涓墦寮€ `index.html`
   - 鐐瑰嚮鍦板潃鏍忓彸渚х殑"瀹夎"鍥炬爣
   - 鎴栫偣鍑婚〉闈㈠簳閮ㄧ殑"瀹夎"妯箙

### Android

**鏂规硶涓€锛氶€氳繃缃戦〉璁块棶**
1. 灏嗗簲鐢ㄩ儴缃插埌浠绘剰 Web 鏈嶅姟鍣紙鎴栫敤鎵嬫満娴忚鍣ㄨ闂數鑴戜笂鐨勬枃浠讹級
2. 鍦?Chrome 涓墦寮€椤甸潰
3. 鐐瑰嚮鑿滃崟 鈫?"娣诲姞鍒颁富灞忓箷"

**鏂规硶浜岋細鏈湴杩愯**
1. 鍦ㄧ數鑴戜笂鍚姩鏈湴鏈嶅姟鍣細
   ```bash
   # 浣跨敤 Python
   python -m http.server 8080
   
   # 鎴栦娇鐢?Node.js
   npx serve .
   ```
2. 纭繚鎵嬫満鍜岀數鑴戝湪鍚屼竴灞€鍩熺綉
3. 鍦ㄦ墜鏈烘祻瑙堝櫒璁块棶 `http://鐢佃剳IP:8080`
4. 娣诲姞鍒颁富灞忓箷

**鏂规硶涓夛細浣跨敤 Termux锛堢绾匡級**
1. 鍦?Android 瀹夎 Termux
2. 鍦?Termux 涓畨瑁?Node.js锛歚pkg install nodejs`
3. 澶嶅埗搴旂敤鏂囦欢鍒版墜鏈?4. 杩愯锛歚npx serve .`
5. 娴忚鍣ㄨ闂苟瀹夎

## 鏂囦欢璇存槑

```
weight-tracker/
鈹溾攢鈹€ index.html      # 涓诲簲鐢ㄦ枃浠讹紙鍗曟枃浠跺簲鐢級
鈹溾攢鈹€ manifest.json   # PWA 閰嶇疆
鈹溾攢鈹€ sw.js           # Service Worker锛堢绾挎敮鎸侊級
鈹斺攢鈹€ README.md       # 璇存槑鏂囨。
```

## 鎶€鏈爤

- **鍓嶇**: 绾?HTML/CSS/JavaScript锛堟棤妗嗘灦渚濊禆锛?- **鍥捐〃**: Canvas 2D 鍘熺敓缁樺埗
- **瀛樺偍**: localStorage
- **PWA**: Web App Manifest + Service Worker
- **璁捐**: 鑷畾涔夋殫鑹蹭富棰橈紝娓愬彉閰嶈壊

## 鐩爣浣撻噸璁剧疆

鍙屽嚮"鐩爣"鍗＄墖鍗冲彲淇敼鐩爣浣撻噸銆?
## 鏁版嵁澶囦唤

鏁版嵁瀛樺偍鍦ㄦ祻瑙堝櫒鐨?localStorage 涓€傚闇€澶囦唤锛?1. 鎵撳紑娴忚鍣ㄥ紑鍙戣€呭伐鍏凤紙F12锛?2. Application 鈫?Local Storage 鈫?鎵惧埌瀵瑰簲鍩熷悕
3. 澶嶅埗 `weight_tracker_data` 鐨勫€?
## 鑷畾涔?
濡傞渶淇敼閰嶈壊锛岀紪杈?`index.html` 涓殑 CSS 鍙橀噺锛?```css
:root {
    --accent: #00d9ff;      /* 涓昏壊璋?*/
    --success: #00ff88;     /* 涓嬮檷棰滆壊 */
    --danger: #ff4466;      /* 涓婂崌棰滆壊 */
    --bg-primary: #0f0f1a;  /* 鑳屾櫙鑹?*/
}
```

## License

MIT