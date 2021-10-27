### OpenCV 使用

#### NOTE: 程式碼不包含字幕

#### NOTE: width與height設定和原本影片相同的尺寸
```
width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
```

#### NOTE: cv2.imshow('frame', frame) # 使用相同的'frame'視窗才不會生出新的視窗

#### 改:設定換濾鏡跳轉時間， ex:1400~1500毫秒的位置跳出，1400毫秒前就是此濾鏡的運行時間
```
if 1500>=int(cap.get(cv2.CAP_PROP_POS_MSEC)) >= 1400: # 單位是每毫秒，會因FPS變動影響原影片在程式運行時的毫秒數
```

