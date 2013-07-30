# NAME

events - show events

# format

    ; -*- coding: utf-8 -*-

    [taiso]
    title    = 体操のお兄さん 2013
    start    = 2013/07/23 16:00
    end      = 2013/08/27 10:00
    message  = やってるみたいです
    uri      = http://tinyurl.com/l4pd8bu
    time     = 0, 6, 12, 18, 23, 2013/08/27 9:00

    ; 表示抑止時間帯指定 start-end (wday)
    suspend  = 10:00-16:00 2
    ; いずれかの条件に当てはまる場合はtitleの表示をしない
    notitle  = daily last
    ; いずれかの条件に当てはまる場合はuriの表示をしない
    nouri    = daily last

    ; 毎日の残り時間が指定時間以下ならmessageを置き換えて表示
    daily    = 5
    dailyfmt = あと%d時間で今日のスタンプがもらえなくなります

    ; 最終日まで指定日数以下ならmessageに続けて表示
    days     = 3
    daysfmt  = (あと%d日!)

    ; 最終日の終了時刻まで指定時間以内になった時のメッセージを変更
    last     = 10
    lastfmth = あと%d時間くらいで終わります
    lastfmtm = あと%d分くらいで終わります   ; 1時間以内ならこちらを使う

