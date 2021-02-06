# Let's Enjoy SOM！
SOM（自己組織化マップ）を直感的に理解するためのデモプログラム．


# Overview
Self Organizing Map（自己組織化マップ）はT.Kohonenによって開発された教師なし学習手法で，高次元データを低次元に写像することができる．

本プログラムでは，SOMによって色配列を3次元（RGB）から2次元（位置）に変換している．
似た色（RGBの値が近い色）同士は近くにマッピングされる．


# Description
アルゴリズムは以下の通りである．
1. マッピング用の2次元色配列をランダムに与える．
2. 3以降を繰り返す．
3. 全入力に対して4を行う．
4. 1の配列のうち，入力の色に最も近い要素とその周囲の要素に入力の色を加える．
5. 色を変更する範囲と度合いを小さくする


# Usage
 - **start**...SOMを実行．
 - **stop**...一時停止．
 - **next**...1入力のみ実行．ひとつずつ見ながら理解するために使う．
 - **test**...入力のうちTestとRGB距離が最も近い色（Truth）と平面上の距離が最も近い色（Pred）が一致しているかを確かめ，正解率を算出する．
 - **reset panel**...マッピング用2次元色配列をリセット．
 - **reset**...マッピング用2次元色配列と入力をリセット．
