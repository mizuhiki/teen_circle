# 使い方
## 時刻設定  
  
1. DCジャックにACアダプタを接続します。青LEDと赤LEDが１列ごとに１周点灯したら正しく動作しています  
  
2. スマートフォンのWiFi設定から、ESP_XXXXXX(X:英数字)というアクセスポイントに接続します  
<img src="../image/image_usage_1.png" width=50%>  
  
3. ChromeやSafariなどのブラウザを起動してURL欄に**192.168.4.1**と入力して実行します  
<img src="../image/image_usage_2.png" width=50%>  
  
4. 以下の画面が表示されたらTime Settingをタップ    
<img src="../image/image_usage_3.png" width=50%>  
  
5. 以下の画面で時刻を設定できます。System Time Setをタップでスマートフォンのシステム時刻をセットします  
また、テキストボックスに任意の日時を入力しManual Time Setをタップで任意の時間を設定できます  
<img src="../image/image_usage_4.png" width=50%>  
  
※システム時刻は画面左側のテキストBOXには反映されません  
  
## 調光機能  
Rev2から調光機能を追加しました。スマートフォンのUIからLEDの明るさを変更できます  
  
### 設定方法  
1. スマートフォンのWiFi設定から、ESP_XXXXXX(X:英数字)というアクセスポイントに接続します(時刻設定と同じ)  
  
2. 192.168.4.1/light.htmlとブラウザのURL欄に入力して実行します  
  
3. 以下の画面が表示されたらテキストボックスに数字を入力(0～255)をして、brightness setボタンをタップします  
<img src="../image/Rev2/image_rev2_usage_1.png" width=50%>  
  
4. LEDの明るさが変わります、数字が大きいほど輝度は高くなります  
  
## デモモード  
  
動作デモ用にLEDを順に光らすパターンを繰り返します  
LEDの実装確認などに使用してください  
1. 192.168.4.1/demo.htmlとブラウザのURL欄に入力して実行します  
  
2. 以下の画面が表示されたらDEMO1かDEMO2をタップしてモードを選択します  
  
<img src="../image/image_usage_5.png" width=50%>  
  
MODE1 : 起動時のLED点灯パターンと同じ。青LEDと赤LEDが順に1列のみ1周点灯します  
MODE2 : 青LEDと赤LEDの全てのLEDが順に1周点灯します  
        (MODE1→MODE2のモード変更の際、1周目はファームのバグで点灯しないLED列がありますが、2周目からは正しく点灯します)  