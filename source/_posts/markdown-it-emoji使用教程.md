---
title: markdown-it-emoji使用教程
tags:
  - emoji
  - hexo
categories:
  - markdown
abbrlink: 19333065
date: 2020-09-11 15:10:42
---

> 在使用hexo写博客时，希望加入一些emoji表情，增加文章的趣味性。

<!--more-->
### 安装markdown-it-emoji包

```shell
npm install markdown-it-emoji --save
```

### 使用emoji

对于想使用的emoji表情，可以通过查看[emoji表情表](https://www.webfx.com/tools/emoji-cheat-sheet/)，对于想要使用的表情直接copy就好。
为了防止链接失效，对网站的表情进行备份（备份过程中，发现有部分表情无法解析）

|Symbols|Places|Objects|Nature|People|
|-:|-:|-:|-:|-:|
|`:one:` :one:|`:house:` :house:|`:bamboo:` :bamboo:|`:sunny:` :sunny:|`:bowtie:` :bowtie:|
|`:two:` :two:|`:house_with_garden:` :house_with_garden:|`:gift_heart:` :gift_heart:|`:umbrella:` :umbrella:|`:smile:` :smile:|
|`:three:` :three:|`:school:` :school:|`:dolls:` :dolls:|`:cloud:` :cloud:|`:simple_smile:` :simple_smile:|
|`:four:` :four:|`:office:` :office:|`:school_satchel:` :school_satchel:|`:snowflake:` :snowflake:|`:laughing:` :laughing:|
|`:five:` :five:|`:post_office:` :post_office:|`:mortar_board:` :mortar_board:|`:snowman:` :snowman:|`:blush:` :blush:|
|`:six:` :six:|`:hospital:` :hospital:|`:flags:` :flags:|`:zap:` :zap:|`:smiley:` :smiley:|
|`:seven:` :seven:|`:bank:` :bank:|`:fireworks:` :fireworks:|`:cyclone:` :cyclone:|`:relaxed:` :relaxed:|
|`:eight:` :eight:|`:convenience_store:` :convenience_store:|`:sparkler:` :sparkler:|`:foggy:` :foggy:|`:smirk:` :smirk:|
|`:nine:` :nine:|`:love_hotel:` :love_hotel:|`:wind_chime:` :wind_chime:|`:ocean:` :ocean:|`:heart_eyes:` :heart_eyes:|
|`:keycap_ten:` :keycap_ten:|`:hotel:` :hotel:|`:rice_scene:` :rice_scene:|`:cat:` :cat:|`:kissing_heart:` :kissing_heart:|
|`:1234:` :1234:|`:wedding:` :wedding:|`:jack_o_lantern:` :jack_o_lantern:|`:dog:` :dog:|`:kissing_closed_eyes:` :kissing_closed_eyes:|
|`:zero:` :zero:|`:church:` :church:|`:ghost:` :ghost:|`:mouse:` :mouse:|`:flushed:` :flushed:|
|`:hash:` :hash:|`:department_store:` :department_store:|`:santa:` :santa:|`:hamster:` :hamster:|`:relieved:` :relieved:|
|`:symbols:` :symbols:|`:european_post_office:` :european_post_office:|`:christmas_tree:` :christmas_tree:|`:rabbit:` :rabbit:|`:satisfied:` :satisfied:|
|`:arrow_backward:` :arrow_backward:|`:city_sunrise:` :city_sunrise:|`:gift:` :gift:|`:wolf:` :wolf:|`:grin:` :grin:|
|`:arrow_down:` :arrow_down:|`:city_sunset:` :city_sunset:|`:bell:` :bell:|`:frog:` :frog:|`:wink:` :wink:|
|`:arrow_forward:` :arrow_forward:|`:japanese_castle:` :japanese_castle:|`:no_bell:` :no_bell:|`:tiger:` :tiger:|`:stuck_out_tongue_winking_eye:` :stuck_out_tongue_winking_eye:|
|`:arrow_left:` :arrow_left:|`:european_castle:` :european_castle:|`:tanabata_tree:` :tanabata_tree:|`:koala:` :koala:|`:stuck_out_tongue_closed_eyes:` :stuck_out_tongue_closed_eyes:|
|`:capital_abcd:` :capital_abcd:|`:tent:` :tent:|`:tada:` :tada:|`:bear:` :bear:|`:grinning:` :grinning:|
|`:abcd:` :abcd:|`:factory:` :factory:|`:confetti_ball:` :confetti_ball:|`:pig:` :pig:|`:kissing:` :kissing:|
|`:abc:` :abc:|`:tokyo_tower:` :tokyo_tower:|`:balloon:` :balloon:|`:pig_nose:` :pig_nose:|`:kissing_smiling_eyes:` :kissing_smiling_eyes:|
|`:arrow_lower_left:` :arrow_lower_left:|`:japan:` :japan:|`:crystal_ball:` :crystal_ball:|`:cow:` :cow:|`:stuck_out_tongue:` :stuck_out_tongue:|
|`:arrow_lower_right:` :arrow_lower_right:|`:mount_fuji:` :mount_fuji:|`:cd:` :cd:|`:boar:` :boar:|`:sleeping:` :sleeping:|
|`:arrow_right:` :arrow_right:|`:sunrise_over_mountains:` :sunrise_over_mountains:|`:dvd:` :dvd:|`:monkey_face:` :monkey_face:|`:worried:` :worried:|
|`:arrow_up:` :arrow_up:|`:sunrise:` :sunrise:|`:floppy_disk:` :floppy_disk:|`:monkey:` :monkey:|`:frowning:` :frowning:|
|`:arrow_upper_left:` :arrow_upper_left:|`:stars:` :stars:|`:camera:` :camera:|`:horse:` :horse:|`:anguished:` :anguished:|
|`:arrow_upper_right:` :arrow_upper_right:|`:statue_of_liberty:` :statue_of_liberty:|`:video_camera:` :video_camera:|`:racehorse:` :racehorse:|`:open_mouth:` :open_mouth:|
|`:arrow_double_down:` :arrow_double_down:|`:bridge_at_night:` :bridge_at_night:|`:movie_camera:` :movie_camera:|`:camel:` :camel:|`:grimacing:` :grimacing:|
|`:arrow_double_up:` :arrow_double_up:|`:carousel_horse:` :carousel_horse:|`:computer:` :computer:|`:sheep:` :sheep:|`:confused:` :confused:|
|`:arrow_down_small:` :arrow_down_small:|`:rainbow:` :rainbow:|`:tv:` :tv:|`:elephant:` :elephant:|`:hushed:` :hushed:|
|`:arrow_heading_down:` :arrow_heading_down:|`:ferris_wheel:` :ferris_wheel:|`:iphone:` :iphone:|`:panda_face:` :panda_face:|`:expressionless:` :expressionless:|
|`:arrow_heading_up:` :arrow_heading_up:|`:fountain:` :fountain:|`:phone:` :phone:|`:snake:` :snake:|`:unamused:` :unamused:|
|`:leftwards_arrow_with_hook:` :leftwards_arrow_with_hook:|`:roller_coaster:` :roller_coaster:|`:telephone:` :telephone:|`:bird:` :bird:|`:sweat_smile:` :sweat_smile:|
|`:arrow_right_hook:` :arrow_right_hook:|`:ship:` :ship:|`:telephone_receiver:` :telephone_receiver:|`:baby_chick:` :baby_chick:|`:sweat:` :sweat:|
|`:left_right_arrow:` :left_right_arrow:|`:speedboat:` :speedboat:|`:pager:` :pager:|`:hatched_chick:` :hatched_chick:|`:disappointed_relieved:` :disappointed_relieved:|
|`:arrow_up_down:` :arrow_up_down:|`:boat:` :boat:|`:fax:` :fax:|`:hatching_chick:` :hatching_chick:|`:weary:` :weary:|
|`:arrow_up_small:` :arrow_up_small:|`:sailboat:` :sailboat:|`:minidisc:` :minidisc:|`:chicken:` :chicken:|`:pensive:` :pensive:|
|`:arrows_clockwise:` :arrows_clockwise:|`:rowboat:` :rowboat:|`:vhs:` :vhs:|`:penguin:` :penguin:|`:disappointed:` :disappointed:|
|`:arrows_counterclockwise:` :arrows_counterclockwise:|`:anchor:` :anchor:|`:sound:` :sound:|`:turtle:` :turtle:|`:confounded:` :confounded:|
|`:rewind:` :rewind:|`:rocket:` :rocket:|`:speaker:` :speaker:|`:bug:` :bug:|`:fearful:` :fearful:|
|`:fast_forward:` :fast_forward:|`:airplane:` :airplane:|`:mute:` :mute:|`:honeybee:` :honeybee:|`:cold_sweat:` :cold_sweat:|
|`:information_source:` :information_source:|`:helicopter:` :helicopter:|`:loudspeaker:` :loudspeaker:|`:ant:` :ant:|`:persevere:` :persevere:|
|`:ok:` :ok:|`:steam_locomotive:` :steam_locomotive:|`:mega:` :mega:|`:beetle:` :beetle:|`:cry:` :cry:|
|`:twisted_rightwards_arrows:` :twisted_rightwards_arrows:|`:tram:` :tram:|`:hourglass:` :hourglass:|`:snail:` :snail:|`:sob:` :sob:|
|`:repeat:` :repeat:|`:mountain_railway:` :mountain_railway:|`:hourglass_flowing_sand:` :hourglass_flowing_sand:|`:octopus:` :octopus:|`:joy:` :joy:|
|`:repeat_one:` :repeat_one:|`:bike:` :bike:|`:alarm_clock:` :alarm_clock:|`:tropical_fish:` :tropical_fish:|`:astonished:` :astonished:|
|`:new:` :new:|`:aerial_tramway:` :aerial_tramway:|`:watch:` :watch:|`:fish:` :fish:|`:scream:` :scream:|
|`:top:` :top:|`:suspension_railway:` :suspension_railway:|`:radio:` :radio:|`:whale:` :whale:|`:neckbeard:` :neckbeard:|
|`:up:` :up:|`:mountain_cableway:` :mountain_cableway:|`:satellite:` :satellite:|`:whale2:` :whale2:|`:tired_face:` :tired_face:|
|`:cool:` :cool:|`:tractor:` :tractor:|`:loop:` :loop:|`:dolphin:` :dolphin:|`:angry:` :angry:|
|`:free:` :free:|`:blue_car:` :blue_car:|`:mag:` :mag:|`:cow2:` :cow2:|`:rage:` :rage:|
|`:ng:` :ng:|`:oncoming_automobile:` :oncoming_automobile:|`:mag_right:` :mag_right:|`:ram:` :ram:|`:triumph:` :triumph:|
|`:cinema:` :cinema:|`:car:` :car:|`:unlock:` :unlock:|`:rat:` :rat:|`:sleepy:` :sleepy:|
|`:koko:` :koko:|`:red_car:` :red_car:|`:lock:` :lock:|`:water_buffalo:` :water_buffalo:|`:yum:` :yum:|
|`:signal_strength:` :signal_strength:|`:taxi:` :taxi:|`:lock_with_ink_pen:` :lock_with_ink_pen:|`:tiger2:` :tiger2:|`:mask:` :mask:|
|`:u5272:` :u5272:|`:oncoming_taxi:` :oncoming_taxi:|`:closed_lock_with_key:` :closed_lock_with_key:|`:rabbit2:` :rabbit2:|`:sunglasses:` :sunglasses:|
|`:u5408:` :u5408:|`:articulated_lorry:` :articulated_lorry:|`:key:` :key:|`:dragon:` :dragon:|`:dizzy_face:` :dizzy_face:|
|`:u55b6:` :u55b6:|`:bus:` :bus:|`:bulb:` :bulb:|`:goat:` :goat:|`:imp:` :imp:|
|`:u6307:` :u6307:|`:oncoming_bus:` :oncoming_bus:|`:flashlight:` :flashlight:|`:rooster:` :rooster:|`:smiling_imp:` :smiling_imp:|
|`:u6708:` :u6708:|`:rotating_light:` :rotating_light:|`:high_brightness:` :high_brightness:|`:dog2:` :dog2:|`:neutral_face:` :neutral_face:|
|`:u6709:` :u6709:|`:police_car:` :police_car:|`:low_brightness:` :low_brightness:|`:pig2:` :pig2:|`:no_mouth:` :no_mouth:|
|`:u6e80:` :u6e80:|`:oncoming_police_car:` :oncoming_police_car:|`:electric_plug:` :electric_plug:|`:mouse2:` :mouse2:|`:innocent:` :innocent:|
|`:u7121:` :u7121:|`:fire_engine:` :fire_engine:|`:battery:` :battery:|`:ox:` :ox:|`:alien:` :alien:|
|`:u7533:` :u7533:|`:ambulance:` :ambulance:|`:calling:` :calling:|`:dragon_face:` :dragon_face:|`:yellow_heart:` :yellow_heart:|
|`:u7a7a:` :u7a7a:|`:minibus:` :minibus:|`:email:` :email:|`:blowfish:` :blowfish:|`:blue_heart:` :blue_heart:|
|`:u7981:` :u7981:|`:truck:` :truck:|`:mailbox:` :mailbox:|`:crocodile:` :crocodile:|`:purple_heart:` :purple_heart:|
|`:sa:` :sa:|`:train:` :train:|`:postbox:` :postbox:|`:dromedary_camel:` :dromedary_camel:|`:heart:` :heart:|
|`:restroom:` :restroom:|`:station:` :station:|`:bath:` :bath:|`:leopard:` :leopard:|`:green_heart:` :green_heart:|
|`:mens:` :mens:|`:train2:` :train2:|`:bathtub:` :bathtub:|`:cat2:` :cat2:|`:broken_heart:` :broken_heart:|
|`:womens:` :womens:|`:bullettrain_front:` :bullettrain_front:|`:shower:` :shower:|`:poodle:` :poodle:|`:heartbeat:` :heartbeat:|
|`:baby_symbol:` :baby_symbol:|`:bullettrain_side:` :bullettrain_side:|`:toilet:` :toilet:|`:paw_prints:` :paw_prints:|`:heartpulse:` :heartpulse:|
|`:no_smoking:` :no_smoking:|`:light_rail:` :light_rail:|`:wrench:` :wrench:|`:bouquet:` :bouquet:|`:two_hearts:` :two_hearts:|
|`:parking:` :parking:|`:monorail:` :monorail:|`:nut_and_bolt:` :nut_and_bolt:|`:cherry_blossom:` :cherry_blossom:|`:revolving_hearts:` :revolving_hearts:|
|`:wheelchair:` :wheelchair:|`:railway_car:` :railway_car:|`:hammer:` :hammer:|`:tulip:` :tulip:|`:cupid:` :cupid:|
|`:metro:` :metro:|`:trolleybus:` :trolleybus:|`:seat:` :seat:|`:four_leaf_clover:` :four_leaf_clover:|`:sparkling_heart:` :sparkling_heart:|
|`:baggage_claim:` :baggage_claim:|`:ticket:` :ticket:|`:moneybag:` :moneybag:|`:rose:` :rose:|`:sparkles:` :sparkles:|
|`:accept:` :accept:|`:fuelpump:` :fuelpump:|`:yen:` :yen:|`:sunflower:` :sunflower:|`:star:` :star:|
|`:wc:` :wc:|`:vertical_traffic_light:` :vertical_traffic_light:|`:dollar:` :dollar:|`:hibiscus:` :hibiscus:|`:star2:` :star2:|
|`:potable_water:` :potable_water:|`:traffic_light:` :traffic_light:|`:pound:` :pound:|`:maple_leaf:` :maple_leaf:|`:dizzy:` :dizzy:|
|`:put_litter_in_its_place:` :put_litter_in_its_place:|`:warning:` :warning:|`:euro:` :euro:|`:leaves:` :leaves:|`:boom:` :boom:|
|`:secret:` :secret:|`:construction:` :construction:|`:credit_card:` :credit_card:|`:fallen_leaf:` :fallen_leaf:|`:collision:` :collision:|
|`:congratulations:` :congratulations:|`:beginner:` :beginner:|`:money_with_wings:` :money_with_wings:|`:herb:` :herb:|`:anger:` :anger:|
|`:m:` :m:|`:atm:` :atm:|`:e-mail:` :e-mail:|`:mushroom:` :mushroom:|`:exclamation:` :exclamation:|
|`:passport_control:` :passport_control:|`:slot_machine:` :slot_machine:|`:inbox_tray:` :inbox_tray:|`:cactus:` :cactus:|`:question:` :question:|
|`:left_luggage:` :left_luggage:|`:busstop:` :busstop:|`:outbox_tray:` :outbox_tray:|`:palm_tree:` :palm_tree:|`:grey_exclamation:` :grey_exclamation:|
|`:customs:` :customs:|`:barber:` :barber:|`:envelope:` :envelope:|`:evergreen_tree:` :evergreen_tree:|`:grey_question:` :grey_question:|
|`:ideograph_advantage:` :ideograph_advantage:|`:hotsprings:` :hotsprings:|`:incoming_envelope:` :incoming_envelope:|`:deciduous_tree:` :deciduous_tree:|`:zzz:` :zzz:|
|`:cl:` :cl:|`:checkered_flag:` :checkered_flag:|`:postal_horn:` :postal_horn:|`:chestnut:` :chestnut:|`:dash:` :dash:|
|`:sos:` :sos:|`:crossed_flags:` :crossed_flags:|`:mailbox_closed:` :mailbox_closed:|`:seedling:` :seedling:|`:sweat_drops:` :sweat_drops:|
|`:id:` :id:|`:izakaya_lantern:` :izakaya_lantern:|`:mailbox_with_mail:` :mailbox_with_mail:|`:blossom:` :blossom:|`:notes:` :notes:|
|`:no_entry_sign:` :no_entry_sign:|`:moyai:` :moyai:|`:mailbox_with_no_mail:` :mailbox_with_no_mail:|`:ear_of_rice:` :ear_of_rice:|`:musical_note:` :musical_note:|
|`:underage:` :underage:|`:circus_tent:` :circus_tent:|`:package:` :package:|`:shell:` :shell:|`:fire:` :fire:|
|`:no_mobile_phones:` :no_mobile_phones:|`:performing_arts:` :performing_arts:|`:door:` :door:|`:globe_with_meridians:` :globe_with_meridians:|`:hankey:` :hankey:|
|`:do_not_litter:` :do_not_litter:|`:round_pushpin:` :round_pushpin:|`:smoking:` :smoking:|`:sun_with_face:` :sun_with_face:|`:poop:` :poop:|
|`:non-potable_water:` :non-potable_water:|`:triangular_flag_on_post:` :triangular_flag_on_post:|`:bomb:` :bomb:|`:full_moon_with_face:` :full_moon_with_face:|`:shit:` :shit:|
|`:no_bicycles:` :no_bicycles:|`:jp:` :jp:|`:gun:` :gun:|`:new_moon_with_face:` :new_moon_with_face:|`:+1:` :+1:|
|`:no_pedestrians:` :no_pedestrians:|`:kr:` :kr:|`:hocho:` :hocho:|`:new_moon:` :new_moon:|`:thumbsup:` :thumbsup:|
|`:children_crossing:` :children_crossing:|`:cn:` :cn:|`:pill:` :pill:|`:waxing_crescent_moon:` :waxing_crescent_moon:|`:-1:` :-1:|
|`:no_entry:` :no_entry:|`:us:` :us:|`:syringe:` :syringe:|`:first_quarter_moon:` :first_quarter_moon:|`:thumbsdown:` :thumbsdown:|
|`:eight_spoked_asterisk:` :eight_spoked_asterisk:|`:fr:` :fr:|`:page_facing_up:` :page_facing_up:|`:waxing_gibbous_moon:` :waxing_gibbous_moon:|`:ok_hand:` :ok_hand:|
|`:sparkle:` :sparkle:|`:es:` :es:|`:page_with_curl:` :page_with_curl:|`:full_moon:` :full_moon:|`:punch:` :punch:|
|`:eight_pointed_black_star:` :eight_pointed_black_star:|`:it:` :it:|`:bookmark_tabs:` :bookmark_tabs:|`:waning_gibbous_moon:` :waning_gibbous_moon:|`:facepunch:` :facepunch:|
|`:heart_decoration:` :heart_decoration:|`:ru:` :ru:|`:bar_chart:` :bar_chart:|`:last_quarter_moon:` :last_quarter_moon:|`:fist:` :fist:|
|`:vs:` :vs:|`:gb:` :gb:|`:chart_with_upwards_trend:` :chart_with_upwards_trend:|`:waning_crescent_moon:` :waning_crescent_moon:|`:v:` :v:|
|`:vibration_mode:` :vibration_mode:|`:uk:` :uk:|`:chart_with_downwards_trend:` :chart_with_downwards_trend:|`:last_quarter_moon_with_face:` :last_quarter_moon_with_face:|`:wave:` :wave:|
|`:mobile_phone_off:` :mobile_phone_off:||`:scroll:` :scroll:|`:first_quarter_moon_with_face:` :first_quarter_moon_with_face:|`:hand:` :hand:|
|`:chart:` :chart:||`:clipboard:` :clipboard:|`:crescent_moon:` :crescent_moon:|`:raised_hand:` :raised_hand:|
|`:currency_exchange:` :currency_exchange:||`:calendar:` :calendar:|`:earth_africa:` :earth_africa:|`:open_hands:` :open_hands:|
|`:aries:` :aries:||`:date:` :date:|`:earth_americas:` :earth_americas:|`:point_up:` :point_up:|
|`:taurus:` :taurus:||`:card_index:` :card_index:|`:earth_asia:` :earth_asia:|`:point_down:` :point_down:|
|`:gemini:` :gemini:||`:file_folder:` :file_folder:|`:volcano:` :volcano:|`:point_left:` :point_left:|
|`:cancer:` :cancer:||`:open_file_folder:` :open_file_folder:|`:milky_way:` :milky_way:|`:point_right:` :point_right:|
|`:leo:` :leo:||`:scissors:` :scissors:|`:partly_sunny:` :partly_sunny:|`:raised_hands:` :raised_hands:|
|`:virgo:` :virgo:||`:pushpin:` :pushpin:|`:octocat:` :octocat:|`:pray:` :pray:|
|`:libra:` :libra:||`:paperclip:` :paperclip:|`:squirrel:` :squirrel:|`:point_up_2:` :point_up_2:|
|`:scorpius:` :scorpius:||`:black_nib:` :black_nib:||`:clap:` :clap:|
|`:sagittarius:` :sagittarius:||`:pencil2:` :pencil2:||`:muscle:` :muscle:|
|`:capricorn:` :capricorn:||`:straight_ruler:` :straight_ruler:||`:metal:` :metal:|
|`:aquarius:` :aquarius:||`:triangular_ruler:` :triangular_ruler:||`:fu:` :fu:|
|`:pisces:` :pisces:||`:closed_book:` :closed_book:||`:runner:` :runner:|
|`:ophiuchus:` :ophiuchus:||`:green_book:` :green_book:||`:running:` :running:|
|`:six_pointed_star:` :six_pointed_star:||`:blue_book:` :blue_book:||`:couple:` :couple:|
|`:negative_squared_cross_mark:` :negative_squared_cross_mark:||`:orange_book:` :orange_book:||`:family:` :family:|
|`:a:` :a:||`:notebook:` :notebook:||`:two_men_holding_hands:` :two_men_holding_hands:|
|`:b:` :b:||`:notebook_with_decorative_cover:` :notebook_with_decorative_cover:||`:two_women_holding_hands:` :two_women_holding_hands:|
|`:ab:` :ab:||`:ledger:` :ledger:||`:dancer:` :dancer:|
|`:o2:` :o2:||`:books:` :books:||`:dancers:` :dancers:|
|`:diamond_shape_with_a_dot_inside:` :diamond_shape_with_a_dot_inside:||`:bookmark:` :bookmark:||`:ok_woman:` :ok_woman:|
|`:recycle:` :recycle:||`:name_badge:` :name_badge:||`:no_good:` :no_good:|
|`:end:` :end:||`:microscope:` :microscope:||`:information_desk_person:` :information_desk_person:|
|`:back:` :back:||`:telescope:` :telescope:||`:raising_hand:` :raising_hand:|
|`:on:` :on:||`:newspaper:` :newspaper:||`:bride_with_veil:` :bride_with_veil:|
|`:soon:` :soon:||`:football:` :football:||`:person_with_pouting_face:` :person_with_pouting_face:|
|`:clock1:` :clock1:||`:basketball:` :basketball:||`:person_frowning:` :person_frowning:|
|`:clock130:` :clock130:||`:soccer:` :soccer:||`:bow:` :bow:|
|`:clock10:` :clock10:||`:baseball:` :baseball:||`:couplekiss:` :couplekiss:|
|`:clock1030:` :clock1030:||`:tennis:` :tennis:||`:couple_with_heart:` :couple_with_heart:|
|`:clock11:` :clock11:||`:8ball:` :8ball:||`:massage:` :massage:|
|`:clock1130:` :clock1130:||`:rugby_football:` :rugby_football:||`:haircut:` :haircut:|
|`:clock12:` :clock12:||`:bowling:` :bowling:||`:nail_care:` :nail_care:|
|`:clock1230:` :clock1230:||`:golf:` :golf:||`:boy:` :boy:|
|`:clock2:` :clock2:||`:mountain_bicyclist:` :mountain_bicyclist:||`:girl:` :girl:|
|`:clock230:` :clock230:||`:bicyclist:` :bicyclist:||`:woman:` :woman:|
|`:clock3:` :clock3:||`:horse_racing:` :horse_racing:||`:man:` :man:|
|`:clock330:` :clock330:||`:snowboarder:` :snowboarder:||`:baby:` :baby:|
|`:clock4:` :clock4:||`:swimmer:` :swimmer:||`:older_woman:` :older_woman:|
|`:clock430:` :clock430:||`:surfer:` :surfer:||`:older_man:` :older_man:|
|`:clock5:` :clock5:||`:ski:` :ski:||`:person_with_blond_hair:` :person_with_blond_hair:|
|`:clock530:` :clock530:||`:spades:` :spades:||`:man_with_gua_pi_mao:` :man_with_gua_pi_mao:|
|`:clock6:` :clock6:||`:hearts:` :hearts:||`:man_with_turban:` :man_with_turban:|
|`:clock630:` :clock630:||`:clubs:` :clubs:||`:construction_worker:` :construction_worker:|
|`:clock7:` :clock7:||`:diamonds:` :diamonds:||`:cop:` :cop:|
|`:clock730:` :clock730:||`:gem:` :gem:||`:angel:` :angel:|
|`:clock8:` :clock8:||`:ring:` :ring:||`:princess:` :princess:|
|`:clock830:` :clock830:||`:trophy:` :trophy:||`:smiley_cat:` :smiley_cat:|
|`:clock9:` :clock9:||`:musical_score:` :musical_score:||`:smile_cat:` :smile_cat:|
|`:clock930:` :clock930:||`:musical_keyboard:` :musical_keyboard:||`:heart_eyes_cat:` :heart_eyes_cat:|
|`:heavy_dollar_sign:` :heavy_dollar_sign:||`:violin:` :violin:||`:kissing_cat:` :kissing_cat:|
|`:copyright:` :copyright:||`:space_invader:` :space_invader:||`:smirk_cat:` :smirk_cat:|
|`:registered:` :registered:||`:video_game:` :video_game:||`:scream_cat:` :scream_cat:|
|`:tm:` :tm:||`:black_joker:` :black_joker:||`:crying_cat_face:` :crying_cat_face:|
|`:x:` :x:||`:flower_playing_cards:` :flower_playing_cards:||`:joy_cat:` :joy_cat:|
|`:heavy_exclamation_mark:` :heavy_exclamation_mark:||`:game_die:` :game_die:||`:pouting_cat:` :pouting_cat:|
|`:bangbang:` :bangbang:||`:dart:` :dart:||`:japanese_ogre:` :japanese_ogre:|
|`:interrobang:` :interrobang:||`:mahjong:` :mahjong:||`:japanese_goblin:` :japanese_goblin:|
|`:o:` :o:||`:clapper:` :clapper:||`:see_no_evil:` :see_no_evil:|
|`:heavy_multiplication_x:` :heavy_multiplication_x:||`:memo:` :memo:||`:hear_no_evil:` :hear_no_evil:|
|`:heavy_plus_sign:` :heavy_plus_sign:||`:pencil:` :pencil:||`:speak_no_evil:` :speak_no_evil:|
|`:heavy_minus_sign:` :heavy_minus_sign:||`:book:` :book:||`:guardsman:` :guardsman:|
|`:heavy_division_sign:` :heavy_division_sign:||`:art:` :art:||`:skull:` :skull:|
|`:white_flower:` :white_flower:||`:microphone:` :microphone:||`:feet:` :feet:|
|`:100:` :100:||`:headphones:` :headphones:||`:lips:` :lips:|
|`:heavy_check_mark:` :heavy_check_mark:||`:trumpet:` :trumpet:||`:kiss:` :kiss:|
|`:ballot_box_with_check:` :ballot_box_with_check:||`:saxophone:` :saxophone:||`:droplet:` :droplet:|
|`:radio_button:` :radio_button:||`:guitar:` :guitar:||`:ear:` :ear:|
|`:link:` :link:||`:shoe:` :shoe:||`:eyes:` :eyes:|
|`:curly_loop:` :curly_loop:||`:sandal:` :sandal:||`:nose:` :nose:|
|`:wavy_dash:` :wavy_dash:||`:high_heel:` :high_heel:||`:tongue:` :tongue:|
|`:part_alternation_mark:` :part_alternation_mark:||`:lipstick:` :lipstick:||`:love_letter:` :love_letter:|
|`:trident:` :trident:||`:boot:` :boot:||`:bust_in_silhouette:` :bust_in_silhouette:|
|`:black_small_square:` :black_small_square:||`:shirt:` :shirt:||`:busts_in_silhouette:` :busts_in_silhouette:|
|`:white_small_square:` :white_small_square:||`:tshirt:` :tshirt:||`:speech_balloon:` :speech_balloon:|
|`:black_medium_small_square:` :black_medium_small_square:||`:necktie:` :necktie:||`:thought_balloon:` :thought_balloon:|
|`:white_medium_small_square:` :white_medium_small_square:||`:womans_clothes:` :womans_clothes:||`:feelsgood:` :feelsgood:|
|`:black_medium_square:` :black_medium_square:||`:dress:` :dress:||`:finnadie:` :finnadie:|
|`:white_medium_square:` :white_medium_square:||`:running_shirt_with_sash:` :running_shirt_with_sash:||`:goberserk:` :goberserk:|
|`:black_large_square:` :black_large_square:||`:jeans:` :jeans:||`:godmode:` :godmode:|
|`:white_large_square:` :white_large_square:||`:kimono:` :kimono:||`:hurtrealbad:` :hurtrealbad:|
|`:white_check_mark:` :white_check_mark:||`:bikini:` :bikini:||`:rage1:` :rage1:|
|`:black_square_button:` :black_square_button:||`:ribbon:` :ribbon:||`:rage2:` :rage2:|
|`:white_square_button:` :white_square_button:||`:tophat:` :tophat:||`:rage3:` :rage3:|
|`:black_circle:` :black_circle:||`:crown:` :crown:||`:rage4:` :rage4:|
|`:white_circle:` :white_circle:||`:womans_hat:` :womans_hat:||`:suspect:` :suspect:|
|`:red_circle:` :red_circle:||`:mans_shoe:` :mans_shoe:||`:trollface:` :trollface:|
|`:large_blue_circle:` :large_blue_circle:||`:closed_umbrella:` :closed_umbrella:|||
|`:large_blue_diamond:` :large_blue_diamond:||`:briefcase:` :briefcase:|||
|`:large_orange_diamond:` :large_orange_diamond:||`:handbag:` :handbag:|||
|`:small_blue_diamond:` :small_blue_diamond:||`:pouch:` :pouch:|||
|`:small_orange_diamond:` :small_orange_diamond:||`:purse:` :purse:|||
|`:small_red_triangle:` :small_red_triangle:||`:eyeglasses:` :eyeglasses:|||
|||`:fishing_pole_and_fish:` :fishing_pole_and_fish:|||
|||`:coffee:` :coffee:|||
|||`:tea:` :tea:|||
|||`:sake:` :sake:|||
|||`:baby_bottle:` :baby_bottle:|||
|||`:beer:` :beer:|||
|||`:beers:` :beers:|||
|||`:cocktail:` :cocktail:|||
|||`:tropical_drink:` :tropical_drink:|||
|||`:wine_glass:` :wine_glass:|||
|||`:fork_and_knife:` :fork_and_knife:|||
|||`:pizza:` :pizza:|||
|||`:hamburger:` :hamburger:|||
|||`:fries:` :fries:|||
|||`:poultry_leg:` :poultry_leg:|||
|||`:meat_on_bone:` :meat_on_bone:|||
|||`:spaghetti:` :spaghetti:|||
|||`:curry:` :curry:|||
|||`:fried_shrimp:` :fried_shrimp:|||
|||`:bento:` :bento:|||
|||`:sushi:` :sushi:|||
|||`:fish_cake:` :fish_cake:|||
|||`:rice_ball:` :rice_ball:|||
|||`:rice_cracker:` :rice_cracker:|||
|||`:rice:` :rice:|||
|||`:ramen:` :ramen:|||
|||`:stew:` :stew:|||
|||`:oden:` :oden:|||
|||`:dango:` :dango:|||
|||`:egg:` :egg:|||
|||`:bread:` :bread:|||
|||`:doughnut:` :doughnut:|||
|||`:custard:` :custard:|||
|||`:icecream:` :icecream:|||
|||`:ice_cream:` :ice_cream:|||
|||`:shaved_ice:` :shaved_ice:|||
|||`:birthday:` :birthday:|||
|||`:cake:` :cake:|||
|||`:cookie:` :cookie:|||
|||`:chocolate_bar:` :chocolate_bar:|||
|||`:candy:` :candy:|||
|||`:lollipop:` :lollipop:|||
|||`:honey_pot:` :honey_pot:|||
|||`:apple:` :apple:|||
|||`:green_apple:` :green_apple:|||
|||`:tangerine:` :tangerine:|||
|||`:lemon:` :lemon:|||
|||`:cherries:` :cherries:|||
|||`:grapes:` :grapes:|||
|||`:watermelon:` :watermelon:|||
|||`:strawberry:` :strawberry:|||
|||`:peach:` :peach:|||
|||`:melon:` :melon:|||
|||`:banana:` :banana:|||
|||`:pear:` :pear:|||
|||`:pineapple:` :pineapple:|||
|||`:sweet_potato:` :sweet_potato:|||
|||`:eggplant:` :eggplant:|||
|||`:tomato:` :tomato:|||
|||`:corn:` :corn:|||

