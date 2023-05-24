# douyin
####  抖音直播 抖音弹幕 直播弹幕


### 返回code常用状态码说明
|状态码|说明|
|--|--|
|0|仅表示请求成功|
|401004|用户不存在,请先开户|
|401005|用户被锁定|
|401017|次数用完|
|401018|token缺失|
|500001|系统内部异常|
|500002|请求有问题|

|已完成|等待添加|
|--|--|
|主页信息|粉丝列表|
|视频详情|用户搜索|
|评论列表|视频搜索|
|回复列表|话题搜索|
|作品列表|用户橱窗|
|点赞列表|商品详情|
|主页手机|水印解析|
| |实时弹幕|




## 1.抖音主页完整信息
```
/dy/user/info/all
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|uid|string|是|用户uid|
|secId|string|否|MS4开头的id,和 uid二选一|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "extra": {
        "fatal_item_ids": [],
        "logid": "202305220145556E84E1F618497AE3ED04",
        "now": 1684691155000
    },
    "log_pb": {
        "impr_id": "202305220145556E84E1F618497AE3ED04"
    },
    "status_code": 0,
    "status_msg": null,
    "user": {
        "apple_account": 0,
        "avatar_168x168": {
            "height": 720,
            "uri": "aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
            "url_list": [
                "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03~c5_168x168.jpeg?from=2956013662"
            ],
            "width": 720
        },
        "avatar_300x300": {
            "height": 720,
            "uri": "aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
            "url_list": [
                "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03~c5_300x300.jpeg?from=2956013662"
            ],
            "width": 720
        },
        "avatar_larger": {
            "height": 720,
            "uri": "aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
            "url_list": [
                "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=2956013662"
            ],
            "width": 720
        },
        "avatar_medium": {
            "height": 720,
            "uri": "aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
            "url_list": [
                "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=2956013662"
            ],
            "width": 720
        },
        "avatar_thumb": {
            "height": 720,
            "uri": "aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
            "url_list": [
                "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=2956013662"
            ],
            "width": 720
        },
        "aweme_count": 7781,
        "aweme_count_correction_threshold": -1,
        "birthday_hide_level": 0,
        "can_set_item_cover": false,
        "can_show_group_card": 1,
        "card_entries": [
            {
                "card_data": "{\"has_yellow_point\":false,\"announcement_release_time\":0,\"preview_video_release_time\":0,\"precipitation_video_release_time\":0,\"style\":0,\"appointment_id\":0,\"typ\":0,\"subscribe_cnt\":0,\"subscribe_status\":0,\"top_title\":\"\",\"top_subtitle\":\"\",\"cycle\":0}",
                "goto_url": "sslocal://webcast_lynxview?url=https%3A%2F%2Flf-webcast-gr-sourcecdn.bytegecko.com%2Fobj%2Fbyte-gurd-source-gr%2Fwebcast%2Fmono%2Flynx%2Fcommunity_live_dynamic_douyin%2Ftemplate%2Fpages%2Flive_dynamic%2Ftemplate.js%3Fanchor_id%3D66598046050%26sec_anchor_id%3DMS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M&web_bg_color=%23161823&status_bar_color=white&type=fullscreen&hide_nav_bar=1&trans_status_bar=1&enable_preload=main&fallback_url=sslocal%3A%2F%2Fwebcast_webview%3Furl%3Dhttps%253A%252F%252Flf-webcast-gr-sourcecdn.bytegecko.com%252Fobj%252Fbyte-gurd-source-gr%252Fwebcast%252Fmono%252Flynx%252Fcommunity_live_dynamic_douyin%252Fweb%252Ftemplate%252Fpages%252Flive_dynamic%252Findex.html%253Fanchor_id%253D66598046050%2526sec_anchor_id%253DMS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M%26web_bg_color%3D%2523161823%26status_bar_color%3Dwhite%26type%3Dfullscreen%26hide_nav_bar%3D1%26trans_status_bar%3D1",
                "icon_dark": {
                    "uri": "obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_dark.png",
                    "url_list": [
                        "https://p6-dy-ipv6.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_dark.png",
                        "https://p3-dy-ipv6.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_dark.png",
                        "https://p9-dy.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_dark.png"
                    ]
                },
                "icon_light": {
                    "uri": "obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_light.png",
                    "url_list": [
                        "https://p6-dy-ipv6.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_light.png",
                        "https://p3-dy-ipv6.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_light.png",
                        "https://p9-dy.byteimg.com/obj/eden-cn/91eh7uhfnult/all_cards_old_version/type6_live_dynamic_light.png"
                    ]
                },
                "sub_title": "查看历史记录",
                "title": "直播动态",
                "type": 6
            }
        ],
        "city": null,
        "close_friend_type": 0,
        "commerce_info": {
            "challenge_list": null,
            "head_image_list": null,
            "offline_info_list": [],
            "smart_phone_list": null,
            "task_list": null
        },
        "commerce_user_info": {
            "ad_revenue_rits": null,
            "has_ads_entry": true,
            "show_star_atlas_cooperation": false,
            "star_atlas": 1
        },
        "commerce_user_level": 0,
        "country": null,
        "cover_and_head_image_info": {
            "cover_list": null,
            "profile_cover_list": []
        },
        "cover_colour": "#02161823",
        "cover_url": [
            {
                "uri": "c8510002be9a3a61aad2",
                "url_list": [
                    "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1684861200&x-signature=mLAXUOzJcpxMW1WsQ6wLkaD40W4%3D&from=2480802190",
                    "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1684861200&x-signature=k6G%2B1dX2kNMCtRixS%2Fxn5QHQxTA%3D&from=2480802190",
                    "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1684861200&x-signature=Eq2KVZbKlh0P8mni%2BlB1jaL%2FIw4%3D&from=2480802190"
                ]
            }
        ],
        "custom_verify": "",
        "district": null,
        "dog_card_info": {
            "dog_card_text": "短剧最热榜",
            "rank": 11,
            "rank_schema": "https://aweme.snssdk.com/magic/eco/procode/magicProcodeActivity_playsot/index.html?activityId=60810dc17819ac032ce3bd3a&page=2&activeIndex=0&hide_nav_bar=1&should_full_screen=1",
            "rank_type": "hot"
        },
        "dongtai_count": 0,
        "dynamic_cover": {},
        "enable_wish": false,
        "enterprise_user_info": "{\"commerce_info\":{\"offline_info_list\":[],\"challenge_list\":null,\"task_list\":null,\"head_image_list\":null,\"smart_phone_list\":null},\"homepage_bottom_toast\":null,\"permissions\":[{\"Id\":3,\"Key\":\"ItemShop\",\"Name\":\"视频电商\",\"AppId\":1128,\"Status\":1,\"Extra\":null,\"Customization\":null,\"Parent\":0,\"Actions\":null},{\"Id\":4,\"Key\":\"LiveShop\",\"Name\":\"直播电商\",\"AppId\":1128,\"Status\":1,\"Extra\":null,\"Customization\":null,\"Parent\":0,\"Actions\":null},{\"Id\":5,\"Key\":\"UserShop\",\"Name\":\"个人橱窗\",\"AppId\":1128,\"Status\":1,\"Extra\":null,\"Customization\":null,\"Parent\":1,\"Actions\":null}],\"tab_ceiling_toast\":null,\"limiters\":null,\"attic_info\":null,\"profile_edit_button\":null,\"elite_center\":null,\"enterprise_card_visibility\":false,\"blue_label_edit_jump_url\":\"aweme://webview/?url=https%3A%2F%2Fapi.amemv.com%2Finsights%2Flite%2FcontactSetting%3Fhide_nav_bar%3D1%26title%3D%25E8%2581%2594%25E7%25B3%25BB%25E6%2596%25B9%25E5%25BC%258F%26enter_from%3Dcustomized_tab&hide_nav_bar=1&title=%E8%81%94%E7%B3%BB%E6%96%B9%E5%BC%8F&rn_schema=aweme%3A%2F%2Freactnative%2F%3Fchannel_name%3Drn_patch%26bundle_name%3Dbusiness%26module_name%3Dpage_e_lite_contactSetting%26force_h5%3D1%26hide_nav_bar%3D1%26bundle_url%3D%26title%3D%25E8%2581%2594%25E7%25B3%25BB%25E6%2596%25B9%25E5%25BC%258F%26enter_from%3Dcustomized_tab\"}",
        "enterprise_verify_reason": "央视新闻官方抖音号",
        "favorite_permission": null,
        "favoriting_count": 53,
        "follow_status": 0,
        "follower_count": 153036243,
        "follower_request_status": 0,
        "follower_status": 0,
        "following_count": 38,
        "forward_count": 8,
        "gender": null,
        "has_e_account_role": false,
        "has_subscription": false,
        "im_primary_role_id": 17,
        "im_role_ids": [
            17,
            8,
            19,
            9,
            23
        ],
        "image_send_exempt": false,
        "ins_id": "",
        "is_activity_user": false,
        "is_ban": false,
        "is_block": false,
        "is_blocked": false,
        "is_effect_artist": false,
        "is_gov_media_vip": true,
        "is_mix_user": true,
        "is_not_show": false,
        "is_series_user": true,
        "is_sharing_profile_user": 0,
        "is_star": false,
        "life_story_block": {
            "life_story_block": false
        },
        "live_commerce": true,
        "live_status": 0,
        "max_follower_count": 153040032,
        "message_chat_entry": true,
        "mix_count": 4,
        "mplatform_followers_count": 153036243,
        "nickname": "央视新闻",
        "original_musician": {
            "digg_count": 0,
            "music_count": 0,
            "music_used_count": 0
        },
        "pigeon_daren_status": "",
        "pigeon_daren_warn_tag": "",
        "profile_tab_type": 0,
        "province": null,
        "public_collects_count": 0,
        "publish_landing_tab": 3,
        "r_fans_group_info": {},
        "recommend_reason_relation": "",
        "recommend_user_reason_source": 0,
        "risk_notice_text": "",
        "room_id": 0,
        "school_name": null,
        "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
        "secret": 0,
        "series_count": 0,
        "share_info": {
            "bool_persist": 1,
            "share_desc": "长按复制此条消息，打开抖音搜索，查看TA的更多作品。",
            "share_image_url": {
                "uri": "tos-cn-p-0015/687326b41272448ba01c9fc91501f832_1684655619",
                "url_list": [
                    "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/687326b41272448ba01c9fc91501f832_1684655619?x-expires=1684861200&x-signature=2dKQp1i01nqS3ULLKAMR9J59JHo%3D&from=2480802190",
                    "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/687326b41272448ba01c9fc91501f832_1684655619?x-expires=1684861200&x-signature=y3Pju9pR8BPLanIz85C0rPmWcTo%3D&from=2480802190",
                    "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/687326b41272448ba01c9fc91501f832_1684655619?x-expires=1684861200&x-signature=GRyliJQv8vo6EFVfMaF%2B8uTCitU%3D&from=2480802190"
                ]
            },
            "share_qrcode_url": {
                "uri": "72a4000fe1b5d865c51b",
                "url_list": [
                    "https://p3.douyinpic.com/obj/72a4000fe1b5d865c51b",
                    "https://p11.douyinpic.com/obj/72a4000fe1b5d865c51b",
                    "https://p26.douyinpic.com/obj/72a4000fe1b5d865c51b"
                ]
            },
            "share_title": "快来加入抖音，让你发现最有趣的我！",
            "share_url": "www.iesdouyin.com/share/user/MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M?did=MS4wLjABAAAAE8wkYt5jM2Q_4d2t3xUR_x6iLPspX4br7zSL0vfTIDyIgCHvWkw3AMTMm1sGVVhp&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&sec_uid=MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M&from_ssr=1",
            "share_weibo_desc": "长按复制此条消息，打开抖音搜索，查看TA的更多作品。"
        },
        "short_id": "0",
        "show_favorite_list": true,
        "show_subscription": false,
        "signature": "我用心，你放心。",
        "signature_display_lines": 0,
        "signature_language": "un",
        "special_follow_status": 0,
        "sync_to_toutiao": 0,
        "tab_settings": {
            "private_tab": {
                "private_tab_style": 1,
                "show_private_tab": false
            }
        },
        "total_favorited": 7810192431,
        "total_favorited_correction_threshold": -1,
        "twitter_id": "",
        "twitter_name": "",
        "uid": "66598046050",
        "unique_id": "cctvnews",
        "urge_detail": {
            "user_urged": 0
        },
        "user_age": null,
        "user_not_see": 0,
        "user_not_show": 1,
        "verification_type": 0,
        "video_cover": {},
        "video_icon": {
            "height": 720,
            "uri": "",
            "url_list": [],
            "width": 720
        },
        "watch_status": false,
        "white_cover_url": [
            {
                "uri": "318f1000413827e122102",
                "url_list": [
                    "https://p6-pc-sign.douyinpic.com/obj/318f1000413827e122102?x-expires=1684861200&x-signature=qckEx0q3yH9v5%2B6EfiVvMIjvLZ4%3D&from=2480802190",
                    "https://p3-pc-sign.douyinpic.com/obj/318f1000413827e122102?x-expires=1684861200&x-signature=ismw9oDMn50IehnIHOKtSREKpR8%3D&from=2480802190",
                    "https://p9-pc-sign.douyinpic.com/obj/318f1000413827e122102?x-expires=1684861200&x-signature=NOIduiLN7hx03m7zMTLBD6qGAOA%3D&from=2480802190"
                ]
            }
        ],
        "with_commerce_enterprise_tab_entry": false,
        "with_commerce_entry": true,
        "with_fusion_shop_entry": true,
        "with_new_goods": false,
        "youtube_channel_id": "",
        "youtube_channel_title": ""
    }
}

  </code>
 </pre>
</details>


## 2.抖音主页基本信息
```
/dy/user/info/base
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|dyId|string|是|抖音号,和secId二选一|
|secId|string|否|MS4开头的id,和 dyId二选一|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "status_code": 0,
    "user_info": {
        "short_id": "0",
        "nickname": "大象新闻",
        "signature": "脚踏实地做新闻！\n拍客投稿，请发送至daxiangbaoliao@163.com\n求助帮忙请关注后私信（时间+地点+人物+事件+联系方式）\n商务v：DAXIANGMCN",
        "avatar_thumb": {
            "uri": "aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d",
            "url_list": [
                "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662",
                "https://p11.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662",
                "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662"
            ]
        },
        "avatar_medium": {
            "uri": "aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d",
            "url_list": [
                "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662",
                "https://p11.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662",
                "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_932c080d8ee0445da29f2daa9b522c8d.jpeg?from=2956013662"
            ]
        },
        "follow_status": 0,
        "aweme_count": 45761,
        "following_count": 1000,
        "favoriting_count": 0,
        "total_favorited": "2743452015",
        "custom_verify": "",
        "unique_id": "ElephantNews",
        "verification_type": 0,
        "original_musician": {
            "music_count": 0,
            "music_used_count": 0,
            "digg_count": 0
        },
        "enterprise_verify_reason": "河南广播电视台大象新闻官方抖音号",
        "mplatform_followers_count": 27242000,
        "followers_detail": null,
        "platform_sync_info": null,
        "geofencing": null,
        "policy_version": null,
        "sec_uid": "MS4wLjABAAAAl6JYmBWwiAwBFL_0NeoxwIjLD43oCae8gi0jeh3xRVVVHP5TPEQ2Zhut8OFZ2BSk",
        "type_label": null,
        "show_favorite_list": false,
        "card_entries": [
            {
                "type": 7,
                "title": "Ta的音乐",
                "sub_title": "听听ta的歌单",
                "icon_dark": {
                    "uri": "",
                    "url_list": [
                        "https://p3.douyinpic.com/aweme-server-static-resource/music_card_dark_v1.png~tplv-obj.image",
                        "https://p6.douyinpic.com/aweme-server-static-resource/music_card_dark_v1.png~tplv-obj.image",
                        "https://p9.douyinpic.com/aweme-server-static-resource/music_card_dark_v1.png~tplv-obj.image"
                    ]
                },
                "icon_light": {
                    "uri": "",
                    "url_list": [
                        "https://p3.douyinpic.com/aweme-server-static-resource/music_card_light_v1.png~tplv-obj.image",
                        "https://p6.douyinpic.com/aweme-server-static-resource/music_card_light_v1.png~tplv-obj.image",
                        "https://p9.douyinpic.com/aweme-server-static-resource/music_card_light_v1.png~tplv-obj.image"
                    ]
                }
            }
        ],
        "mix_info": [
            {
                "mix_id": "7217653834410100792",
                "mix_name": "2023清明奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7206962302652794917",
                "mix_name": "2023全国两会",
                "charge_episodes": null
            },
            {
                "mix_id": "7196216963805218877",
                "mix_name": "2023元宵奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7189531091932284985",
                "mix_name": "十台晚会闹兔年",
                "charge_episodes": null
            },
            {
                "mix_id": "7187267741974267942",
                "mix_name": "2023河南春晚",
                "charge_episodes": null
            },
            {
                "mix_id": "7179172767315527741",
                "mix_name": "2022世界杯",
                "charge_episodes": null
            },
            {
                "mix_id": "7150252526619592712",
                "mix_name": "2022河南卫视重阳奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7141389025138444302",
                "mix_name": "河南卫视2022中秋奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7131379968671483940",
                "mix_name": "河南卫视少年奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7136404958517463053",
                "mix_name": "抓捕鳄雀鳝",
                "charge_episodes": null
            },
            {
                "mix_id": "7127865582532937742",
                "mix_name": "2022七夕奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7105342391627810830",
                "mix_name": "2022端午奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7059604822223243300",
                "mix_name": "2022河南春晚",
                "charge_episodes": null
            },
            {
                "mix_id": "7082989124143024136",
                "mix_name": "2022清明奇妙游",
                "charge_episodes": null
            },
            {
                "mix_id": "7051920776479377439",
                "mix_name": "河南战“疫”",
                "charge_episodes": null
            }
        ]
    },
    "extra": {
        "now": 1684692978913,
        "logid": "20230522021618D01B52B510B5DD0B11AD"
    }
}

  </code>
 </pre>
</details>


## 3.抖音视频详情
```
/dy/v/detail
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|vid|string|是|视频id|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "aweme_detail": {
        "admire_auth": {
            "admire_button": 1,
            "is_admire": 0,
            "is_click_admire_icon_recently": 0,
            "is_fifty_admire_author_stable_fans": 0,
            "is_show_admire_button": 0,
            "is_show_admire_tab": 0
        },
        "anchors": null,
        "authentication_token": "MS4wLjAAAAAAaD9e4z23m8TJjFiqRKpYXmD_ZmsK17k9LVo32-U2IlOIi0Hdewq1XhomXl9FkleA6FwXo8oawAIZ3EVSlXKubVjGA4it3MuFK8sDOCEgveojQM51PSC607mOspCA__mcqVNUn55o6y8sAitkIr17wioDlOHYjZ3ha5P6TwyXaTTlGwSzl-izy2PRcc0MWq4A",
        "author": {
            "avatar_thumb": {
                "height": 720,
                "uri": "100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p5.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "cf_list": null,
            "close_friend_type": 0,
            "contacts_status": 2,
            "contrail_list": null,
            "cover_url": [
                {
                    "height": 720,
                    "uri": "c8510002be9a3a61aad2",
                    "url_list": [
                        "https://p6-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=P4iyz7%2FyfUoC8p06njskffZHMKo%3D&from=116350172",
                        "https://p96-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=6C8LFqSk4MX%2FwqMIYggrDjcDnac%3D&from=116350172",
                        "https://p3-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=%2FuuJFUGi46rI4V%2Fuuka7x3DQ%2F5Q%3D&from=116350172"
                    ],
                    "width": 720
                }
            ],
            "create_time": 0,
            "custom_verify": "",
            "data_label_list": null,
            "endorsement_info_list": null,
            "enterprise_verify_reason": "",
            "familiar_visitor_user": null,
            "favoriting_count": 4299,
            "follow_status": 0,
            "follower_count": 0,
            "follower_list_secondary_information_struct": null,
            "follower_status": 0,
            "following_count": 0,
            "im_role_ids": null,
            "is_ad_fake": false,
            "is_blocked_v2": false,
            "is_blocking_v2": false,
            "is_cf": 0,
            "live_high_value": 0,
            "max_follower_count": 0,
            "nickname": "CC lol",
            "not_seen_item_id_list": null,
            "not_seen_item_id_list_v2": null,
            "offline_info_list": null,
            "personal_tag_list": null,
            "prevent_download": false,
            "risk_notice_text": "",
            "sec_uid": "MS4wLjABAAAAHmrBxWjZzbZY9lMHYRJ9-Xx5xUT5aqQ2Y69xtN6iJ2c",
            "secret": 0,
            "share_info": {
                "share_desc": "",
                "share_desc_info": "",
                "share_qrcode_url": {
                    "height": 720,
                    "uri": "5adb00224377f11a3b1f",
                    "url_list": [
                        "https://p96-sign.douyinpic.com/obj/5adb00224377f11a3b1f?x-expires=1684710000&x-signature=D57fc33lHmxqructa5IB7kZqo8Y%3D&from=116350172",
                        "https://p26-sign.douyinpic.com/obj/5adb00224377f11a3b1f?x-expires=1684710000&x-signature=PnNFXWXaYfkl%2BHoPi4LvBmWiN7E%3D&from=116350172",
                        "https://p3-sign.douyinpic.com/obj/5adb00224377f11a3b1f?x-expires=1684710000&x-signature=3JNgapaAqZSErzTzmmlBOtXu0N8%3D&from=116350172"
                    ],
                    "width": 720
                },
                "share_title": "",
                "share_title_myself": "",
                "share_title_other": "",
                "share_url": "",
                "share_weibo_desc": ""
            },
            "short_id": "272886049",
            "signature": "CC带你玩转新加坡",
            "signature_extra": null,
            "special_follow_status": 0,
            "special_people_labels": null,
            "status": 1,
            "text_extra": null,
            "total_favorited": 1998,
            "uid": "88347654936",
            "unique_id": "cissylol",
            "user_age": -1,
            "user_canceled": false,
            "user_permissions": null,
            "verification_type": 1
        },
        "author_mask_tag": 0,
        "author_user_id": 88347654936,
        "aweme_acl": {
            "download_mask_panel": {
                "code": 1,
                "show_type": 0
            }
        },
        "aweme_control": {
            "can_comment": true,
            "can_forward": true,
            "can_share": true,
            "can_show_comment": true
        },
        "aweme_id": "6790345451242671364",
        "aweme_type": 0,
        "book_bar": {},
        "challenge_position": null,
        "chapter_list": null,
        "collect_stat": 0,
        "collection_corner_mark": 0,
        "comment_gid": 6790345451242671000,
        "comment_list": null,
        "comment_permission_info": {
            "can_comment": true,
            "comment_permission_status": 0,
            "item_detail_entry": true,
            "press_entry": true,
            "toast_guide": false
        },
        "commerce_config_data": null,
        "common_bar_info": "[]",
        "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
        "cover_labels": null,
        "create_time": 1581000509,
        "desc": "孩子衣服破了 想找件新衣服#百变贺新年 #猫精",
        "digg_lottie": {
            "can_bomb": 0,
            "lottie_id": ""
        },
        "disable_relation_bar": 0,
        "dislike_dimension_list": null,
        "dislike_dimension_list_v2": null,
        "distribute_circle": {
            "campus_block_interaction": false,
            "distribute_type": 0
        },
        "duet_aggregate_in_music_tab": false,
        "duration": 11034,
        "feed_comment_config": {
            "input_config_text": "善语结善缘，恶言伤人心"
        },
        "geofencing": [],
        "geofencing_regions": null,
        "group_id": "6790345451242671364",
        "guide_scene_info": {
            "diamond_expose_info_str": "",
            "feed_origin_gid_info_str": "",
            "guide_scene_type": 0
        },
        "hybrid_label": null,
        "image_album_music_info": {
            "begin_time": -1,
            "end_time": -1,
            "volume": -1
        },
        "image_comment": {},
        "image_infos": null,
        "image_list": null,
        "images": null,
        "img_bitrate": null,
        "impression_data": {
            "group_id_list_a": [],
            "group_id_list_b": [],
            "group_id_list_c": [],
            "similar_id_list_a": null,
            "similar_id_list_b": null
        },
        "interaction_stickers": null,
        "is_ads": false,
        "is_collects_selected": 0,
        "is_duet_sing": false,
        "is_image_beat": false,
        "is_life_item": false,
        "is_share_post": false,
        "is_story": 0,
        "is_top": 0,
        "item_warn_notification": {
            "content": "",
            "show": false,
            "type": 0
        },
        "label_top_text": null,
        "long_video": null,
        "music": {
            "album": "",
            "artist_user_infos": null,
            "artists": [],
            "audition_duration": 10,
            "author": "CC lol",
            "author_deleted": false,
            "author_position": null,
            "author_status": 1,
            "avatar_large": {
                "height": 720,
                "uri": "1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p3.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p6.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "avatar_medium": {
                "height": 720,
                "uri": "720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p11.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "avatar_thumb": {
                "height": 720,
                "uri": "100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p11.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "binded_challenge_id": 0,
            "can_background_play": true,
            "collect_stat": 0,
            "cover_hd": {
                "height": 720,
                "uri": "1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p3.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p6.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "cover_large": {
                "height": 720,
                "uri": "1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p3.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p6.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "cover_medium": {
                "height": 720,
                "uri": "720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p11.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "cover_thumb": {
                "height": 720,
                "uri": "100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0",
                "url_list": [
                    "https://p11.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172",
                    "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_2dfbc0002163b81d4cff0.jpeg?from=116350172"
                ],
                "width": 720
            },
            "dmv_auto_show": false,
            "dsp_status": 10,
            "duration": 10,
            "end_time": 0,
            "external_song_info": [],
            "extra": "{\"dsp_switch\":0,\"douyin_beats_info\":{},\"schedule_search_time\":0,\"aggregate_exempt_conf\":[],\"beats\":{},\"music_label_id\":null,\"extract_item_id\":6790345451242671364,\"has_edited\":0,\"reviewed\":0,\"hotsoon_review_time\":-1,\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_subsidy_exp\":false,\"with_aed_model\":1,\"review_unshelve_reason\":0,\"is_red\":0,\"is_aed_music\":1}",
            "id": 6790338686212640000,
            "id_str": "6790338686212639496",
            "is_audio_url_with_cookie": false,
            "is_commerce_music": false,
            "is_del_video": false,
            "is_matched_metadata": false,
            "is_original": false,
            "is_original_sound": true,
            "is_pgc": false,
            "is_restricted": false,
            "is_video_self_see": false,
            "luna_info": {
                "is_luna_user": false
            },
            "lyric_short_position": null,
            "mid": "6790338686212639496",
            "music_chart_ranks": null,
            "music_collect_count": 0,
            "music_cover_atmosphere_color_value": "",
            "music_status": 1,
            "musician_user_infos": null,
            "mute_share": false,
            "offline_desc": "",
            "owner_handle": "cissylol",
            "owner_id": "88347654936",
            "owner_nickname": "CC lol",
            "pgc_music_type": 2,
            "play_url": {
                "height": 720,
                "uri": "https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/1657797688424504.mp3",
                "url_key": "6790338686212639496",
                "url_list": [
                    "https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/1657797688424504.mp3",
                    "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1657797688424504.mp3"
                ],
                "width": 720
            },
            "position": null,
            "prevent_download": false,
            "prevent_item_download_status": 0,
            "preview_end_time": 0,
            "preview_start_time": 0,
            "reason_type": 0,
            "redirect": false,
            "schema_url": "",
            "search_impr": {
                "entity_id": "6790338686212639496"
            },
            "sec_uid": "MS4wLjABAAAAHmrBxWjZzbZY9lMHYRJ9-Xx5xUT5aqQ2Y69xtN6iJ2c",
            "shoot_duration": 10,
            "source_platform": 23,
            "start_time": 0,
            "status": 1,
            "tag_list": null,
            "title": "@CC lol创作的原声",
            "unshelve_countries": null,
            "user_count": 0,
            "video_duration": 10
        },
        "nickname_position": null,
        "origin_comment_ids": null,
        "origin_text_extra": [],
        "original_images": null,
        "packed_clips": null,
        "photo_search_entrance": {
            "ecom_type": 0
        },
        "position": null,
        "press_panel_info": "[{\"interactive\":[\"2_story\",\"2_friend\"]},{\"feedback\":[\"rr_feedback\",\"dislike\",\"ignore\",\"block\",\"unfollow\",\"sever\",\"dislike_collect\"]},{\"control\":[\"speed\",\"auth\",\"delete\",\"save\",\"collect\",\"reward\",\"bg_play\",\"duet\",\"together\"]}]",
        "preview_title": "孩子衣服破了 想找件新衣服#百变贺新年 #猫精",
        "preview_video_status": 1,
        "promotions": [],
        "rate": 12,
        "ref_tts_id_list": null,
        "ref_voice_modify_id_list": null,
        "region": "CN",
        "relation_labels": null,
        "search_impr": {
            "entity_id": "6790345451242671364",
            "entity_type": "GENERAL"
        },
        "series_paid_info": {
            "item_price": 0,
            "series_paid_status": 0
        },
        "share_info": {
            "share_desc": "在抖音，记录美好生活",
            "share_desc_info": "#在抖音，记录美好生活#孩子衣服破了 想找件新衣服#百变贺新年 #猫精",
            "share_link_desc": "1.05 Zzt:/ 复制打开抖音，看看【CC lol的作品】孩子衣服破了 想找件新衣服# 百变贺新年 # 猫精... %s",
            "share_url": "https://www.iesdouyin.com/share/video/6790345451242671364/?region=CN&mid=6790338686212639496&u_code=-1&did=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
        },
        "share_url": "https://www.iesdouyin.com/share/video/6790345451242671364/?region=CN&mid=6790338686212639496&u_code=-1&did=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
        "should_open_ad_report": false,
        "show_follow_button": {},
        "social_tag_list": null,
        "standard_bar_info_list": null,
        "statistics": {
            "admire_count": 0,
            "aweme_id": "6790345451242671364",
            "collect_count": 0,
            "comment_count": 2,
            "digg_count": 16,
            "play_count": 0,
            "share_count": 0
        },
        "status": {
            "allow_share": true,
            "aweme_id": "6790345451242671364",
            "in_reviewing": false,
            "is_delete": false,
            "is_prohibited": false,
            "listen_video_status": 0,
            "part_see": 0,
            "private_status": 0,
            "review_result": {
                "review_status": 0
            }
        },
        "text_extra": [
            {
                "end": 19,
                "hashtag_id": "1655157240549389",
                "hashtag_name": "百变贺新年",
                "is_commerce": false,
                "start": 13,
                "type": 1
            },
            {
                "end": 23,
                "hashtag_id": "1583375783105550",
                "hashtag_name": "猫精",
                "is_commerce": false,
                "start": 20,
                "type": 1
            }
        ],
        "tts_id_list": null,
        "uniqid_position": null,
        "user_digged": 0,
        "user_recommend_status": 0,
        "video": {
            "big_thumbs": null,
            "bit_rate": [
                {
                    "FPS": 30,
                    "HDR_bit": "",
                    "HDR_type": "",
                    "bit_rate": 686958,
                    "gear_name": "normal_540_0",
                    "is_bytevc1": 0,
                    "is_h265": 0,
                    "play_addr": {
                        "data_size": 947488,
                        "file_cs": "c:0-13501-6d94",
                        "file_hash": "1032b5e049bd43164be5279b4830adbd",
                        "height": 1024,
                        "uri": "v0200fe40000bou2e92j2booni4ba6vg",
                        "url_key": "v0200fe40000bou2e92j2booni4ba6vg_h264_540p_686958",
                        "url_list": [
                            "https://v9-cold1.douyinvod.com/0aa6c92429906c0c72dc32b2ea8707de/646a673e/video/tos/cn/tos-cn-ve-15/c6210274529c4ce58a5470b7db12ef58/?a=1128&ch=26&cr=0&dr=0&lr=all&cd=0%7C0%7C0%7C0&cv=1&br=670&bt=670&cs=0&ds=6&ft=GNvhKpVVywSWRso0hmo~ySqTeaApuhK66vrKUJVlSto0g3&mime_type=video_mp4&qs=0&rc=NTpnZTw3NmhmaDQ7N2czPEBpajllbHJlbTw1cjMzN2kzM0BfYi0vNGEzXi8xLWJjNmIxYSNzXjFrbC8vYnJfLS1iLS9zcw%3D%3D&l=2023052201471517EF9C8C6CBC2728F948&btag=e00088000&cdn_n80=1",
                            "https://v26-cold.douyinvod.com/c857a030d2b0c8ba85453c60cfd01305/646a673e/video/tos/cn/tos-cn-ve-15/c6210274529c4ce58a5470b7db12ef58/?a=1128&ch=26&cr=0&dr=0&lr=all&cd=0%7C0%7C0%7C0&cv=1&br=670&bt=670&cs=0&ds=6&ft=GNvhKpVVywSWRso0hmo~ySqTeaApuhK66vrKUJVlSto0g3&mime_type=video_mp4&qs=0&rc=NTpnZTw3NmhmaDQ7N2czPEBpajllbHJlbTw1cjMzN2kzM0BfYi0vNGEzXi8xLWJjNmIxYSNzXjFrbC8vYnJfLS1iLS9zcw%3D%3D&l=2023052201471517EF9C8C6CBC2728F948&btag=e00088000",
                            "https://api-play.amemv.com/aweme/v1/play/?video_id=v0200fe40000bou2e92j2booni4ba6vg&line=0&file_id=49e09df4e8014e2cae63d4792b0de7b2&sign=1032b5e049bd43164be5279b4830adbd&is_play_url=1&source=PackSourceEnum_AWEME_DETAIL",
                            "https://api.amemv.com/aweme/v1/play/?video_id=v0200fe40000bou2e92j2booni4ba6vg&line=1&file_id=49e09df4e8014e2cae63d4792b0de7b2&sign=1032b5e049bd43164be5279b4830adbd&is_play_url=1&source=PackSourceEnum_AWEME_DETAIL"
                        ],
                        "width": 576
                    },
                    "quality_type": 20,
                    "video_extra": "{\"PktOffsetMap\":\"\"}"
                }
            ],
            "bit_rate_audio": null,
            "cover": {
                "height": 720,
                "uri": "tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558",
                "url_list": [
                    "https://p26-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~c5_300x400.jpeg?x-expires=1685898000&x-signature=Tk3K00nD15SWpbRESqnLlx3rnLc%3D&from=3213915784_large&s=PackSourceEnum_AWEME_DETAIL&se=false&sc=cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p6-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~c5_300x400.jpeg?x-expires=1685898000&x-signature=vWwePtW6dje8GV0iSZ9kdYq9DMs%3D&from=3213915784_large&s=PackSourceEnum_AWEME_DETAIL&se=false&sc=cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p3-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~c5_300x400.jpeg?x-expires=1685898000&x-signature=EtH8zeWne1TYfpQ4mM5%2BI33EhYI%3D&from=3213915784_large&s=PackSourceEnum_AWEME_DETAIL&se=false&sc=cover&l=2023052201471517EF9C8C6CBC2728F948"
                ],
                "width": 720
            },
            "cover_original_scale": {
                "height": 720,
                "uri": "tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558",
                "url_list": [
                    "https://p26-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=Yi6kUOjmE7YX%2F1qd02j8ogC9e8g%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p6-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=qofbT4Cd9%2B%2BXSJAkpgzeWz85vYg%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p3-sign.douyinpic.com/tos-cn-p-0015/2a41ae6f32cc41349e3159773f714558~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=YPPjyUSBYkKQBtfsAodbRWUCmaQ%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948"
                ],
                "width": 720
            },
            "duration": 11034,
            "dynamic_cover": {
                "height": 720,
                "uri": "tos-cn-p-0015/91fa27a985584bf59773f83dc7603b44_1581000514",
                "url_list": [
                    "https://p3-sign.douyinpic.com/obj/tos-cn-p-0015/91fa27a985584bf59773f83dc7603b44_1581000514?x-expires=1685898000&x-signature=8%2BeZ2FjLdeD5QGd9ERr0ha7w39w%3D&from=3213915784_large",
                    "https://p26-sign.douyinpic.com/obj/tos-cn-p-0015/91fa27a985584bf59773f83dc7603b44_1581000514?x-expires=1685898000&x-signature=poWwn2ToOYeqL9mYh8UYlrxym3Q%3D&from=3213915784_large",
                    "https://p9-sign.douyinpic.com/obj/tos-cn-p-0015/91fa27a985584bf59773f83dc7603b44_1581000514?x-expires=1685898000&x-signature=y2L2kDW5%2Fc06G3vBy%2B3VYP0WKBM%3D&from=3213915784_large"
                ],
                "width": 720
            },
            "height": 1280,
            "is_h265": 0,
            "is_source_HDR": 1,
            "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"0.000\"}",
            "origin_cover": {
                "height": 720,
                "uri": "tos-cn-p-0015/9a62e500976b407bad046f8b6f0e5c55_1581000514",
                "url_list": [
                    "https://p3-sign.douyinpic.com/tos-cn-p-0015/9a62e500976b407bad046f8b6f0e5c55_1581000514~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=1UNjjnzBUQzjoNHjVnRX3oapu0M%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p6-sign.douyinpic.com/tos-cn-p-0015/9a62e500976b407bad046f8b6f0e5c55_1581000514~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=ZucVwR%2FdItNIMpoOM5jo4gaS4bw%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948",
                    "https://p26-sign.douyinpic.com/tos-cn-p-0015/9a62e500976b407bad046f8b6f0e5c55_1581000514~tplv-dy-360p.jpeg?x-expires=1685898000&x-signature=jxChcpjIWxR3mz6HNvzWSTb%2BrnU%3D&from=3213915784&se=false&biz_tag=feed_cover&l=2023052201471517EF9C8C6CBC2728F948"
                ],
                "width": 720
            },
            "play_addr": {
                "data_size": 947488,
                "file_cs": "c:0-13501-6d94",
                "file_hash": "1032b5e049bd43164be5279b4830adbd",
                "height": 1024,
                "uri": "v0200fe40000bou2e92j2booni4ba6vg",
                "url_key": "v0200fe40000bou2e92j2booni4ba6vg_h264_540p_686958",
                "url_list": [
                    "https://v9-cold1.douyinvod.com/0aa6c92429906c0c72dc32b2ea8707de/646a673e/video/tos/cn/tos-cn-ve-15/c6210274529c4ce58a5470b7db12ef58/?a=1128&ch=26&cr=0&dr=0&lr=all&cd=0%7C0%7C0%7C0&cv=1&br=670&bt=670&cs=0&ds=6&ft=GNvhKpVVywSWRso0hmo~ySqTeaApuhK66vrKUJVlSto0g3&mime_type=video_mp4&qs=0&rc=NTpnZTw3NmhmaDQ7N2czPEBpajllbHJlbTw1cjMzN2kzM0BfYi0vNGEzXi8xLWJjNmIxYSNzXjFrbC8vYnJfLS1iLS9zcw%3D%3D&l=2023052201471517EF9C8C6CBC2728F948&btag=e00088000&cdn_n80=1",
                    "https://v26-cold.douyinvod.com/c857a030d2b0c8ba85453c60cfd01305/646a673e/video/tos/cn/tos-cn-ve-15/c6210274529c4ce58a5470b7db12ef58/?a=1128&ch=26&cr=0&dr=0&lr=all&cd=0%7C0%7C0%7C0&cv=1&br=670&bt=670&cs=0&ds=6&ft=GNvhKpVVywSWRso0hmo~ySqTeaApuhK66vrKUJVlSto0g3&mime_type=video_mp4&qs=0&rc=NTpnZTw3NmhmaDQ7N2czPEBpajllbHJlbTw1cjMzN2kzM0BfYi0vNGEzXi8xLWJjNmIxYSNzXjFrbC8vYnJfLS1iLS9zcw%3D%3D&l=2023052201471517EF9C8C6CBC2728F948&btag=e00088000",
                    "https://api-play.amemv.com/aweme/v1/play/?video_id=v0200fe40000bou2e92j2booni4ba6vg&line=0&file_id=49e09df4e8014e2cae63d4792b0de7b2&sign=1032b5e049bd43164be5279b4830adbd&is_play_url=1&source=PackSourceEnum_AWEME_DETAIL",
                    "https://api.amemv.com/aweme/v1/play/?video_id=v0200fe40000bou2e92j2booni4ba6vg&line=1&file_id=49e09df4e8014e2cae63d4792b0de7b2&sign=1032b5e049bd43164be5279b4830adbd&is_play_url=1&source=PackSourceEnum_AWEME_DETAIL"
                ],
                "width": 576
            },
            "ratio": "540p",
            "width": 720
        },
        "video_game_data_channel_config": {},
        "video_labels": null,
        "video_tag": [
            {
                "level": 0,
                "tag_id": 0,
                "tag_name": ""
            },
            {
                "level": 0,
                "tag_id": 0,
                "tag_name": ""
            },
            {
                "level": 0,
                "tag_id": 0,
                "tag_name": ""
            }
        ],
        "video_text": [],
        "voice_modify_id_list": null
    },
    "log_pb": {
        "impr_id": "2023052201471517EF9C8C6CBC2728F948"
    },
    "status_code": 0
}

  </code>
 </pre>
</details>


## 4.抖音评论列表
```
/dy/v/comments
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|vid|string|是|视频id|
|pageIndex|string|是|翻页参数，首次为0，根据下一次的返回cursor的值进行下一页|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "bottom_prompt": null,
    "comment_config": {},
    "comment_prompt": null,
    "comment_surprise": null,
    "comments": [
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229907835226931979",
            "create_time": 1683344101,
            "digg_count": 5407,
            "ip_label": "湖南",
            "is_author_digged": false,
            "label_text": "作者",
            "label_type": 1,
            "reply_comment_total": 133,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 1,
            "text": "路不通就转弯 心不悦就看淡[抱抱你]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 2,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "权旨",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "2141481823910699"
                },
                "sec_uid": "MS4wLjABAAAArBczou3rFJHi9ttvEL5mGD9duN-6MN6nQVDqDzy8YGaeoxowBaE2cNf1IzGi0xxF",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "2905743766",
                "show_gender_strategy": 1,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "素材均来自直播\nAMG CLUB：YE99271\n（下午4:30-6:30/晚上10:30-2:00 周一休息",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2141481823910699",
                "unique_id": "QuanJiang_",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 20,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": true,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7231146066929484577",
            "create_time": 1683632401,
            "digg_count": 1221,
            "ip_label": "黑龙江",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 19,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "静姐前180多w粉丝，半年了，现在170w",
            "text_extra": [
                {
                    "end": 2,
                    "search_extra": "{\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                    "search_hide_words": 0,
                    "search_query_id": "6574749780130403588",
                    "search_rank": 0,
                    "search_text": "静姐",
                    "start": 0,
                    "type": 5
                }
            ],
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_3ec1aa3d3cefe73a6d363b9a93dd846c",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [
                    5,
                    6
                ],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 2,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.75,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "方恨长生",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "1310241391120087"
                },
                "sec_uid": "MS4wLjABAAAASTptscbn6RMTkijrKIswvJ9TZ5mpscz-hdbk2u5Fj52sCvWoi9Ww9_Q2GnZXyQF4",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3618169395",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "I want to win your heart\n爱听歌 爱耍帅 爱看风景\n09天才少年",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "1310241391120087",
                "unique_id": "H09131415",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229991035975500582",
            "create_time": 1683363478,
            "digg_count": 1592,
            "ip_label": "江苏",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 65,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "带静姐这么玩过吗[酷拽]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_512c79a659fea6d08ceaacbaf7e12ac0",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 4,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "巩新",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "106024635278"
                },
                "sec_uid": "MS4wLjABAAAACFmew45NsTOnYkHXFV3KM49Pyy-MKWDp6bTaWW8A_eE",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "1696159536",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "#中二病",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "106024635278",
                "unique_id": "",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 33,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7234958954270802700",
            "create_time": 1684520218,
            "digg_count": 3,
            "ip_label": "河北",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 4,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "什么歌啊 好好听",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813c001_ee516146f5f0464e892884d8d2622424",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 9,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.75,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "儒安",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "95502704858"
                },
                "sec_uid": "MS4wLjABAAAAkOdefcIH9YgOf5LBbR2hXU5Y8ISlivZVdFpprN8BZYo",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "1006681658",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "过客",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "95502704858",
                "unique_id": "",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7232372124140569401",
            "create_time": 1683917950,
            "digg_count": 105,
            "ip_label": "贵州",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 14,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "唉，每个作品里面都有人在骂，说实话权确实有一点对不住静姐[捂脸]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813_0b0b737d1add4cac9dcc88e2516ef1d4",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 0,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.592981,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": ",飞鱼",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "58529483673"
                },
                "sec_uid": "MS4wLjABAAAA6E3fJ3vTUIqqdVQfUUFHiVedTCE2RT_61CeimIS56ZQ",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "1938966140",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "你好",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "58529483673",
                "unique_id": "",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229908571625177891",
            "create_time": 1683344275,
            "digg_count": 4843,
            "ip_label": "湖南",
            "is_author_digged": true,
            "label_list": [
                {
                    "text": "作者赞过",
                    "type": 20
                }
            ],
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 19,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "好看 爱看",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/mosaic-legacy_3113a000631caf7e98e9a",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 9,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "今天一穿四了吗",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "59846696274"
                },
                "sec_uid": "MS4wLjABAAAAVHomoH4IWjkvHH-ld12W3EaecvCn3WXAzgx7vRq-NF4",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "12757524",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "直播时间：周一休息\n\n合作🛰️：SGTYYDS77\n只有抖音平台账号 谨防上当受骗",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "59846696274",
                "unique_id": "YCS777777777",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 22,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": true,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7234861609427878715",
            "create_time": 1684497492,
            "digg_count": 9,
            "ip_label": "湖北",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 2,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "谁还不会犯错，权的三观也很正",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_e070ff157df305099f306f1d28f60302",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "aweme_hotsoon_auth_relation": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 0,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.75,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "小泉",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "2058699470799582"
                },
                "sec_uid": "MS4wLjABAAAAg8IP-aOGobQUpgndpDnxU_TVPG7kOI8cOsoAOTJLfF-Oc7o9w-43VuelF_2hpqF_",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "92100341155",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2058699470799582",
                "unique_id": "92100341155",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229928808777433914",
            "create_time": 1683348986,
            "digg_count": 2102,
            "ip_label": "广东",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 133,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "记得很清楚那天违背的那句“我向所有人炫耀了你的好 你让我如何收场”[流泪][流泪][流泪]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813_6392f13d0fba406f8c7eabf5ce3a75fa",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 1,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.63882923,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "@zzzz",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "110478111686"
                },
                "sec_uid": "MS4wLjABAAAAFs5PT_NMREG2tUfT9Ug5DzlFCHNbEqnYdPlp3UpwuyM",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "2080256622",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "110478111686",
                "unique_id": "",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 17,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229906012503966519",
            "create_time": 1683343678,
            "digg_count": 1786,
            "ip_label": "河南",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 6,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "刘双权，你在搞什么飞机✈️[流泪]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813c001_67958126e546496898865a59e7850fb0",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "aweme_hotsoon_auth_relation": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 3,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.5380652,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "青 衣",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "2392140733225614"
                },
                "sec_uid": "MS4wLjABAAAA5xWKxFCOdcAqIe5gSujA7sSHBp-wJcD5HxH1qhhPOK_hZxVZdWAKkiNUSwI6LR0l",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3567072587",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2392140733225614",
                "unique_id": "HGX_1016",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229984399995142924",
            "create_time": 1683361933,
            "digg_count": 710,
            "ip_label": "陕西",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 112,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "做主播最重要的就是三观正，而不是拿你那个所谓的人设来骗粉丝",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813_3dce1f072b1345b2a397594d9bd9a377",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 3,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "uu7",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "3280552891517870"
                },
                "sec_uid": "MS4wLjABAAAAnl5Eo23ZYY78ZLYvQtXwUvnUr6tZxrpbKJE0mFFVLJbNz9ioCmel6PqVTtzUB_bn",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "4185332437",
                "show_gender_strategy": 1,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "1",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "3280552891517870",
                "unique_id": "danbao524",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 17,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229986399037752067",
            "create_time": 1683362396,
            "digg_count": 87,
            "ip_label": "山西",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 57,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "说实话没必要抓着一件事不放 有这时间多提升自己吧[捂脸]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_5b5515146569cbbd2e5321345bac27d7",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 12,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.5365251,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "若",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "109172817358"
                },
                "sec_uid": "MS4wLjABAAAApNuK09Hxuwye-AI3H5iWdmm-rZVxddDWxEtpnfv9ycE",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "1986438256",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "随心而动",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "109172817358",
                "unique_id": "712125h",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229929455728100152",
            "create_time": 1683349137,
            "digg_count": 743,
            "ip_label": "湖南",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 70,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "这几天下雨壁虎都跑出来了[绿帽子]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813c001_db114b6cf80047b98ba931d0380aa4df",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 8,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "殇",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "97889459217"
                },
                "sec_uid": "MS4wLjABAAAAw3ttBnFyXzWcohQNbrnmPjkigX2etsNWqXG6nrmcyBk",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "890297931",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "人性的背后是白云苍狗 愿你我都能做生活的高手.",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "97889459217",
                "unique_id": "Travebiu",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 18,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229914667781964581",
            "create_time": 1683345693,
            "digg_count": 730,
            "ip_label": "广东",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment": [
                {
                    "aweme_id": "7229903986495687991",
                    "can_share": true,
                    "cid": "7229915140090938116",
                    "create_time": 1683345805,
                    "digg_count": 775,
                    "image_list": null,
                    "ip_label": "湖南",
                    "is_author_digged": false,
                    "is_hot": false,
                    "is_note_comment": 0,
                    "label_list": null,
                    "label_text": "作者",
                    "label_type": 1,
                    "level": 2,
                    "reply_comment": null,
                    "reply_id": "7229914667781964581",
                    "reply_to_reply_id": "0",
                    "status": 1,
                    "text": "电鱼电死了",
                    "text_extra": [],
                    "text_music_info": null,
                    "user": {
                        "accept_private_policy": false,
                        "account_region": "",
                        "ad_cover_url": null,
                        "apple_account": 0,
                        "authority_status": 0,
                        "avatar_168x168": {
                            "height": 720,
                            "uri": "168x168/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                            "url_list": [
                                "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835~c5_168x168.jpeg?from=2956013662"
                            ],
                            "width": 720
                        },
                        "avatar_300x300": {
                            "height": 720,
                            "uri": "300x300/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                            "url_list": [
                                "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835~c5_300x300.jpeg?from=2956013662"
                            ],
                            "width": 720
                        },
                        "avatar_larger": {
                            "height": 720,
                            "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                            "url_list": [
                                "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                            ],
                            "width": 720
                        },
                        "avatar_medium": {
                            "height": 720,
                            "uri": "720x720/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                            "url_list": [
                                "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                            ],
                            "width": 720
                        },
                        "avatar_thumb": {
                            "height": 720,
                            "uri": "100x100/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                            "url_list": [
                                "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835.jpeg?from=2956013662"
                            ],
                            "width": 720
                        },
                        "avatar_uri": "aweme-avatar/tos-cn-avt-0015_a056048c602c168c2f9509749ed5f835",
                        "aweme_control": {
                            "can_comment": true,
                            "can_forward": true,
                            "can_share": true,
                            "can_show_comment": true
                        },
                        "aweme_count": 0,
                        "aweme_hotsoon_auth": 1,
                        "ban_user_functions": [],
                        "bind_phone": "",
                        "can_set_geofencing": null,
                        "card_entries": null,
                        "card_entries_not_display": null,
                        "card_sort_priority": null,
                        "cf_list": null,
                        "cha_list": null,
                        "close_friend_type": 0,
                        "comment_filter_status": 0,
                        "comment_setting": 0,
                        "commerce_user_level": 0,
                        "constellation": 2,
                        "contacts_status": 2,
                        "contrail_list": null,
                        "cover_url": [
                            {
                                "height": 720,
                                "uri": "c8510002be9a3a61aad2",
                                "url_list": [
                                    "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                                    "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                                    "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                                ],
                                "width": 720
                            }
                        ],
                        "custom_verify": "",
                        "cv_level": "",
                        "data_label_list": null,
                        "display_info": null,
                        "download_prompt_ts": 0,
                        "download_setting": -1,
                        "duet_setting": 0,
                        "enable_nearby_visible": true,
                        "endorsement_info_list": null,
                        "enterprise_verify_reason": "",
                        "familiar_visitor_user": null,
                        "favoriting_count": 0,
                        "fb_expire_time": 0,
                        "follow_status": 0,
                        "follower_count": 0,
                        "follower_list_secondary_information_struct": null,
                        "follower_request_status": 0,
                        "follower_status": 0,
                        "followers_detail": null,
                        "following_count": 0,
                        "geofencing": [],
                        "google_account": "",
                        "has_email": false,
                        "has_facebook_token": false,
                        "has_insights": false,
                        "has_orders": false,
                        "has_twitter_token": false,
                        "has_unread_story": false,
                        "has_youtube_token": false,
                        "hide_location": false,
                        "hide_search": true,
                        "homepage_bottom_toast": null,
                        "im_role_ids": null,
                        "ins_id": "",
                        "interest_tags": null,
                        "is_ad_fake": false,
                        "is_binded_weibo": false,
                        "is_block": false,
                        "is_blocked_v2": false,
                        "is_blocking_v2": false,
                        "is_cf": 0,
                        "is_discipline_member": false,
                        "is_gov_media_vip": false,
                        "is_mix_user": false,
                        "is_not_show": false,
                        "is_phone_binded": false,
                        "is_star": false,
                        "is_verified": true,
                        "item_list": null,
                        "ky_only_predict": 0,
                        "language": "zh-Hans",
                        "link_item_list": null,
                        "live_agreement": 0,
                        "live_agreement_time": 0,
                        "live_commerce": false,
                        "live_high_value": 0,
                        "live_status": 0,
                        "live_verify": 0,
                        "location": "",
                        "max_follower_count": 0,
                        "need_points": null,
                        "need_recommend": 0,
                        "neiguang_shield": 0,
                        "new_story_cover": null,
                        "nickname": "权旨",
                        "not_seen_item_id_list": null,
                        "not_seen_item_id_list_v2": null,
                        "offline_info_list": null,
                        "personal_tag_list": null,
                        "platform_sync_info": null,
                        "prevent_download": false,
                        "react_setting": 0,
                        "reflow_page_gid": 0,
                        "reflow_page_uid": 0,
                        "region": "CN",
                        "relative_users": null,
                        "risk_notice_text": "",
                        "room_id": 0,
                        "school_category": 0,
                        "school_name": "",
                        "school_poi_id": "",
                        "school_type": 0,
                        "search_impr": {
                            "entity_id": "2141481823910699"
                        },
                        "sec_uid": "MS4wLjABAAAArBczou3rFJHi9ttvEL5mGD9duN-6MN6nQVDqDzy8YGaeoxowBaE2cNf1IzGi0xxF",
                        "secret": 0,
                        "shield_comment_notice": 0,
                        "shield_digg_notice": 0,
                        "shield_follow_notice": 0,
                        "short_id": "2905743766",
                        "show_gender_strategy": 1,
                        "show_image_bubble": false,
                        "show_nearby_active": false,
                        "signature": "素材均来自直播\nAMG CLUB：YE99271\n（下午4:30-6:30/晚上10:30-2:00 周一休息",
                        "signature_display_lines": 0,
                        "signature_extra": null,
                        "special_follow_status": 0,
                        "special_lock": 1,
                        "special_people_labels": null,
                        "status": 1,
                        "stitch_setting": 0,
                        "story_count": 0,
                        "story_open": false,
                        "sync_to_toutiao": 0,
                        "text_extra": null,
                        "total_favorited": 0,
                        "tw_expire_time": 0,
                        "twitter_id": "",
                        "twitter_name": "",
                        "type_label": null,
                        "uid": "2141481823910699",
                        "unique_id": "QuanJiang_",
                        "unique_id_modify_time": 1684691414,
                        "urge_detail": {
                            "user_urged": 0
                        },
                        "user_age": 20,
                        "user_canceled": false,
                        "user_mode": 0,
                        "user_not_see": 0,
                        "user_not_show": 1,
                        "user_period": 0,
                        "user_permissions": null,
                        "user_rate": 1,
                        "user_tags": null,
                        "verification_type": 1,
                        "verify_info": "",
                        "video_icon": {
                            "height": 720,
                            "uri": "",
                            "url_list": [],
                            "width": 720
                        },
                        "weibo_name": "",
                        "weibo_schema": "",
                        "weibo_url": "",
                        "weibo_verify": "",
                        "white_cover_url": null,
                        "with_commerce_entry": false,
                        "with_dou_entry": false,
                        "with_fusion_shop_entry": true,
                        "with_shop_entry": false,
                        "youtube_channel_id": "",
                        "youtube_channel_title": "",
                        "youtube_expire_time": 0
                    },
                    "user_buried": false,
                    "user_digged": 0,
                    "video_list": null
                }
            ],
            "reply_comment_total": 25,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "咋没见知子哥",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813c001_ad8d7da2e70a4ff483eec10b1dfdd0c0",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "aweme_hotsoon_auth_relation": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 12,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.50313777,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "阁",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "4116993592012039"
                },
                "sec_uid": "MS4wLjABAAAAhHO-6sVXQaiAm2JvYSjKJtJwzxez9YBVw_2z32b8-CsnMeEWngBUoh0bgEwYyOoy",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "4154779421",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "06",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "4116993592012039",
                "unique_id": "zhiaicanshi2",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 17,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229913023686869797",
            "create_time": 1683345312,
            "digg_count": 120,
            "ip_label": "山东",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 7,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "你怎么还穿这个红裤衩[送心]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_2d68c75bfbde9a391e7d636586ba640e",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "aweme_hotsoon_auth_relation": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 0,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "陈决池",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "2093944504330968"
                },
                "sec_uid": "MS4wLjABAAAAqrhWlXPBtoaWnYGdOaZ5GdSdDx9mvuJbrMHgb2KS3CnBzXXo9JM8fn8IN2xljCQU",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "30482194701",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "@陈决池",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2093944504330968",
                "unique_id": "Love_xc520qaq",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7230753724686844728",
            "create_time": 1683541053,
            "digg_count": 160,
            "ip_label": "河南",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 31,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "干完跑路确实爽[尬笑]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_6fec9bfdfe35b6be05ccf65f139a49af",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 6,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "ㅤ秋酱",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "967167892262270"
                },
                "sec_uid": "MS4wLjABAAAAobBmqHs9h8NY034jRRB7ptoY2pvblEsBghJ6rEUBs9U",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3817828122",
                "show_gender_strategy": 1,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "剪辑：2198970496",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "967167892262270",
                "unique_id": "QiuQiu2006yyds",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7229906256735535911",
            "create_time": 1683343740,
            "digg_count": 1026,
            "ip_label": "广东",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 16,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-avt-0015_7ab8f825365eac281cbd73e5553dccf9",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 7,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "Joker ㅤ",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "2902329669460324"
                },
                "sec_uid": "MS4wLjABAAAAEL1gOurWhcSnE9dV368_J-pD03H3N6tA2Dbg78kG3h-6LVIaZE5NxhG6BYK_HU9n",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3881011872",
                "show_gender_strategy": 1,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "平安喜乐 万事胜意 祝你 祝大伙",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2902329669460324",
                "unique_id": "DanZi17",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7235514203434746680",
            "create_time": 1684649436,
            "digg_count": 1,
            "ip_label": "贵州",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 0,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "@寒心雨落 这就是我向往的",
            "text_extra": [
                {
                    "end": 5,
                    "hashtag_id": "",
                    "hashtag_name": "",
                    "sec_uid": "MS4wLjABAAAALW6bSp-6Hhxg1_z3eroqA5yFl-EnN6CErllhmU3rI70",
                    "start": 0,
                    "type": 0,
                    "user_id": "99203109721"
                }
            ],
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813_2886a67182194f25a5c2bd9b16210929",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "aweme_hotsoon_auth_relation": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 1,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.601821,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "Dr.",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "1494948672965854"
                },
                "sec_uid": "MS4wLjABAAAATEvqevh26PaR5IWO8TCXCV2O12fTTKqL1puut_6RQFjTuQguPhfUfBddwBSoU74N",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3844123907",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "在",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "1494948672965854",
                "unique_id": "Heimdall.yyds",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7235104112500884224",
            "create_time": 1684553959,
            "digg_count": 0,
            "ip_label": "河南",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 2,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "@爷帅灬奈我何... 这就是我理想的生活[尬笑][泣不成声]",
            "text_extra": [
                {
                    "end": 10,
                    "hashtag_id": "",
                    "hashtag_name": "",
                    "sec_uid": "MS4wLjABAAAAqys4Nfnt-Z2nXAD5J3y5GHQ-rl1S0aWLD3NayZTFXN4",
                    "start": 0,
                    "type": 0,
                    "user_id": "109812614044"
                }
            ],
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813_30070d9d1eba41c59b2b776fa50fc201",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "aweme_hotsoon_auth": 1,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 10,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.68379825,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "烏✨",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "school_category": 0,
                "search_impr": {
                    "entity_id": "2532872488761885"
                },
                "sec_uid": "MS4wLjABAAAAA0oDKCvKllrSQW2pPCYOpxTr0Mt90tTgbkkCwYCdbLaq3NXTkJhKsV-09Dtzgasy",
                "secret": 1,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "3788409138",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "2532872488761885",
                "unique_id": "wer2756tu",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7229903986495687991",
            "cid": "7235662599110558522",
            "create_time": 1684683995,
            "digg_count": 0,
            "ip_label": "江西",
            "is_author_digged": false,
            "label_text": "",
            "label_type": -1,
            "reply_comment_total": 1,
            "reply_id": "0",
            "reply_to_reply_id": "0",
            "status": 1,
            "stick_position": 0,
            "text": "希望是你@莫羡枫",
            "text_extra": [
                {
                    "end": 8,
                    "hashtag_id": "",
                    "hashtag_name": "",
                    "sec_uid": "MS4wLjABAAAAOrTR75GUGdCFSvCk4bVCMPs8xYeC6xwf-T1xjZflOlCFoe5yspuyqkivJ1_m1Xs6",
                    "start": 4,
                    "type": 0,
                    "user_id": "2586490495581022"
                }
            ],
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "168x168/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc~c5_168x168.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "300x300/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/img/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc~c5_300x300.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "aweme-avatar/tos-cn-i-0813c001_97c7d20b9123499f8a3d29a27fda9cbc",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "commerce_user_level": 0,
                "constellation": 11,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [
                    {
                        "height": 720,
                        "uri": "c8510002be9a3a61aad2",
                        "url_list": [
                            "https://p3-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=xZfFaYNrtVrNC5jRjVYReW2vFpE%3D&from=2956013662",
                            "https://p9-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=FAjSrIoXmQ9Oyc%2FY87DF92lV7Vg%3D&from=2956013662",
                            "https://p6-pc-sign.douyinpic.com/obj/c8510002be9a3a61aad2?x-expires=1685898000&x-signature=rpuxlcrBtHbWtz3colFFx1ed08c%3D&from=2956013662"
                        ],
                        "width": 720
                    }
                ],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_discipline_member": false,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.75,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "忧郁的螺蛳粉",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "72909546507"
                },
                "sec_uid": "MS4wLjABAAAA6KYSm6ME6g4RmrjI8FbZzyr6TKJC9qcIdFPbhflqo5s",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "569109391",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "@莫羡枫",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "72909546507",
                "unique_id": "",
                "unique_id_modify_time": 1684691414,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": 19,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        }
    ],
    "cursor": 20,
    "extra": {
        "fatal_item_ids": null,
        "now": 1684691413000
    },
    "fast_response_comment": {
        "constant_response_words": [
            "赞",
            "比心",
            "加油"
        ],
        "timed_response_words": [
            "早上好",
            "下午好",
            "晚上好"
        ]
    },
    "general_comment_config": {},
    "has_more": 1,
    "hotsoon_filtered_count": 0,
    "hotsoon_has_more": null,
    "hotsoon_text": null,
    "log_pb": {
        "impr_id": "20230522015013627E39E46D661DFD09C4"
    },
    "new_insert_ids": null,
    "reply_style": 2,
    "review_status": null,
    "show_friend_comment_desc": null,
    "status_code": 0,
    "total": 3870,
    "user_commented": 0,
    "xigua_text": null
}

  </code>
 </pre>
</details>


## 5.评论回复列表
```
/dy/v/comments4replays
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|vid|string|是|视频id|
|cid|string|是|组id，根据视频评论接口获取|
|pageIndex|string|是|翻页参数，首次为0，根据下一次请求结果cursor值进行下一页|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "comments": [
        {
            "aweme_id": "7231266605701926148",
            "cid": "7231508251488420620",
            "create_time": 1683716728,
            "digg_count": 3349,
            "is_author_digged": false,
            "label_text": "IP:上海",
            "label_type": 2,
            "reply_id": "7231428904149467941",
            "reply_to_reply_id": "0",
            "status": 1,
            "text": "尔等小小坏我道心。",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_d87b68bff9bc4edda3a15db6e36fc8dd.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "constellation": 7,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0.5806463,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "𓄂kꫛⅈᧁꫝt𓆃",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "61058290461"
                },
                "sec_uid": "MS4wLjABAAAABIpjjgoTpdHw6paq6oNYCbwnEw-l86EpYnNwlVzdMak",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "2259148028",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 5,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "61058290461",
                "unique_id": "chuancai4888",
                "unique_id_modify_time": 1684691616,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7231266605701926148",
            "cid": "7231514732754076450",
            "create_time": 1683718242,
            "digg_count": 402,
            "is_author_digged": false,
            "label_text": "IP:辽宁",
            "label_type": 2,
            "reply_id": "7231428904149467941",
            "reply_to_reply_id": "7231508251488420620",
            "reply_to_user_sec_id": "MS4wLjABAAAABIpjjgoTpdHw6paq6oNYCbwnEw-l86EpYnNwlVzdMak",
            "reply_to_userid": "61058290461",
            "reply_to_username": "𓄂kꫛⅈᧁꫝt𓆃",
            "status": 1,
            "text": "肖小吧[看][看][看]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/mosaic-legacy_314b400069b122998fb6f",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/mosaic-legacy_314b400069b122998fb6f",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/100x100/aweme-avatar/mosaic-legacy_314b400069b122998fb6f.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "constellation": 3,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "请叫我女帝大人",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "school_category": 0,
                "search_impr": {
                    "entity_id": "55441880474"
                },
                "sec_uid": "MS4wLjABAAAAHpXhe2hsIRZ9C6JKkmy-I59WI52i2NomQhCGrsS5g8Q",
                "secret": 1,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "1115978316",
                "show_gender_strategy": 1,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 0,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "55441880474",
                "unique_id": "",
                "unique_id_modify_time": 1684691616,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7231266605701926148",
            "cid": "7231532494464811837",
            "create_time": 1683722369,
            "digg_count": 335,
            "is_author_digged": false,
            "label_text": "IP:安徽",
            "label_type": 2,
            "reply_id": "7231428904149467941",
            "reply_to_reply_id": "7231514732754076450",
            "reply_to_user_sec_id": "MS4wLjABAAAAHpXhe2hsIRZ9C6JKkmy-I59WI52i2NomQhCGrsS5g8Q",
            "reply_to_userid": "55441880474",
            "reply_to_username": "请叫我女帝大人",
            "status": 1,
            "text": "尔等宵小",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_1b251674ed564b78ac0194c5a95db700.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "constellation": 8,
                "contacts_status": 2,
                "contrail_list": null,
                "cover_url": [],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": false,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": true,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "晨光熹微",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 1,
                "search_impr": {
                    "entity_id": "540567473503836"
                },
                "sec_uid": "MS4wLjABAAAAsde_cTX4xSSG4D5yVqreJVvGGA2sJhJCOdRIhaK9vBE",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "2368262627",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 5,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "540567473503836",
                "unique_id": "zxcvbj567889",
                "unique_id_modify_time": 1684691616,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7231266605701926148",
            "cid": "7231579611266663207",
            "create_time": 1683733343,
            "digg_count": 7,
            "is_author_digged": false,
            "label_text": "IP:广东",
            "label_type": 2,
            "reply_id": "7231428904149467941",
            "reply_to_reply_id": "7231508251488420620",
            "reply_to_user_sec_id": "MS4wLjABAAAABIpjjgoTpdHw6paq6oNYCbwnEw-l86EpYnNwlVzdMak",
            "reply_to_userid": "61058290461",
            "reply_to_username": "𓄂kꫛⅈᧁꫝt𓆃",
            "status": 1,
            "text": "这么小坏了就坏了吧！重新凝聚肉身[看]",
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-avt-0015_d46ed47b6996b8e62724ac4b226c6a7c.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "constellation": 0,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "༄ོ࿆清风ོ࿆༅࿐",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "79167927417"
                },
                "sec_uid": "MS4wLjABAAAArNm-CLSxQesIqGQC9MgrUsz1G95znWQjSZyaGiidki4",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "147790478",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 5,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "79167927417",
                "unique_id": "8888888dubhim",
                "unique_id_modify_time": 1684691616,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        },
        {
            "aweme_id": "7231266605701926148",
            "cid": "7231728847829173051",
            "create_time": 1683768095,
            "digg_count": 2,
            "is_author_digged": false,
            "label_text": "IP:云南",
            "label_type": 2,
            "reply_id": "7231428904149467941",
            "reply_to_reply_id": "7231508251488420620",
            "reply_to_user_sec_id": "MS4wLjABAAAABIpjjgoTpdHw6paq6oNYCbwnEw-l86EpYnNwlVzdMak",
            "reply_to_userid": "61058290461",
            "reply_to_username": "𓄂kꫛⅈᧁꫝt𓆃",
            "status": 1,
            "text": "@。十二。 [看]",
            "text_extra": [
                {
                    "end": 5,
                    "hashtag_id": "",
                    "hashtag_name": "",
                    "sec_uid": "MS4wLjABAAAAddb6KmpgjE1jX7q2vnebvMOI8lcjBgaDturWkx3k3xM",
                    "start": 0,
                    "type": 0,
                    "user_id": "69357781542"
                }
            ],
            "user": {
                "accept_private_policy": false,
                "account_region": "",
                "ad_cover_url": null,
                "apple_account": 0,
                "authority_status": 0,
                "avatar_168x168": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_300x300": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_larger": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52",
                    "url_list": [
                        "https://p26.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662",
                        "https://p3.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662",
                        "https://p6.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813_e8450351b0fd4255a3bfae562c66cb52.jpeg?from=2956013662"
                    ],
                    "width": 720
                },
                "avatar_uri": "",
                "aweme_control": {
                    "can_comment": true,
                    "can_forward": true,
                    "can_share": true,
                    "can_show_comment": true
                },
                "aweme_count": 0,
                "ban_user_functions": [],
                "bind_phone": "",
                "can_set_geofencing": null,
                "card_entries": null,
                "card_entries_not_display": null,
                "card_sort_priority": null,
                "cf_list": null,
                "cha_list": null,
                "close_friend_type": 0,
                "comment_filter_status": 0,
                "comment_setting": 0,
                "constellation": 2,
                "contacts_status": 1,
                "contrail_list": null,
                "cover_url": [],
                "custom_verify": "",
                "cv_level": "",
                "data_label_list": null,
                "display_info": null,
                "download_prompt_ts": 0,
                "download_setting": -1,
                "duet_setting": 0,
                "enable_nearby_visible": true,
                "endorsement_info_list": null,
                "enterprise_verify_reason": "",
                "familiar_visitor_user": null,
                "favoriting_count": 0,
                "fb_expire_time": 0,
                "follow_status": 0,
                "follower_count": 0,
                "follower_list_secondary_information_struct": null,
                "follower_request_status": 0,
                "follower_status": 0,
                "following_count": 0,
                "geofencing": [],
                "google_account": "",
                "has_email": false,
                "has_facebook_token": false,
                "has_insights": false,
                "has_orders": false,
                "has_twitter_token": false,
                "has_unread_story": false,
                "has_youtube_token": false,
                "hide_location": false,
                "hide_search": false,
                "homepage_bottom_toast": null,
                "im_role_ids": null,
                "ins_id": "",
                "interest_tags": null,
                "is_ad_fake": false,
                "is_binded_weibo": false,
                "is_block": false,
                "is_blocked_v2": false,
                "is_blocking_v2": false,
                "is_cf": 0,
                "is_gov_media_vip": false,
                "is_mix_user": false,
                "is_not_show": false,
                "is_phone_binded": false,
                "is_star": false,
                "is_verified": true,
                "item_list": null,
                "ky_only_predict": 0,
                "language": "zh-Hans",
                "link_item_list": null,
                "live_agreement": 0,
                "live_agreement_time": 0,
                "live_commerce": false,
                "live_high_value": 0,
                "live_status": 0,
                "live_verify": 0,
                "max_follower_count": 0,
                "need_points": null,
                "need_recommend": 0,
                "neiguang_shield": 0,
                "new_story_cover": null,
                "nickname": "肆也",
                "not_seen_item_id_list": null,
                "not_seen_item_id_list_v2": null,
                "offline_info_list": null,
                "personal_tag_list": null,
                "platform_sync_info": null,
                "prevent_download": false,
                "react_setting": 0,
                "reflow_page_gid": 0,
                "reflow_page_uid": 0,
                "region": "CN",
                "relative_users": null,
                "risk_notice_text": "",
                "room_id": 0,
                "school_category": 0,
                "search_impr": {
                    "entity_id": "15777419913"
                },
                "sec_uid": "MS4wLjABAAAA5Jk685pkSgj1vkWCRL56W8WiDa9s57rTfTmgCAmtt7E",
                "secret": 0,
                "shield_comment_notice": 0,
                "shield_digg_notice": 0,
                "shield_follow_notice": 0,
                "short_id": "42090873",
                "show_gender_strategy": 0,
                "show_image_bubble": false,
                "show_nearby_active": false,
                "signature": "",
                "signature_display_lines": 5,
                "signature_extra": null,
                "special_follow_status": 0,
                "special_lock": 1,
                "special_people_labels": null,
                "status": 1,
                "stitch_setting": 0,
                "story_count": 0,
                "story_open": false,
                "sync_to_toutiao": 0,
                "text_extra": null,
                "total_favorited": 0,
                "tw_expire_time": 0,
                "twitter_id": "",
                "twitter_name": "",
                "type_label": null,
                "uid": "15777419913",
                "unique_id": "Hyakuya_",
                "unique_id_modify_time": 1684691616,
                "urge_detail": {
                    "user_urged": 0
                },
                "user_age": -1,
                "user_canceled": false,
                "user_mode": 0,
                "user_not_see": 0,
                "user_not_show": 1,
                "user_period": 0,
                "user_permissions": null,
                "user_rate": 1,
                "user_tags": null,
                "verification_type": 1,
                "verify_info": "",
                "video_icon": {
                    "height": 720,
                    "uri": "",
                    "url_list": [],
                    "width": 720
                },
                "weibo_name": "",
                "weibo_schema": "",
                "weibo_url": "",
                "weibo_verify": "",
                "white_cover_url": null,
                "with_commerce_entry": false,
                "with_dou_entry": false,
                "with_fusion_shop_entry": false,
                "with_shop_entry": false,
                "youtube_channel_id": "",
                "youtube_channel_title": "",
                "youtube_expire_time": 0
            },
            "user_buried": false,
            "user_digged": 0
        }
    ],
    "cursor": 5,
    "extra": {
        "fatal_item_ids": [],
        "logid": "20230522015336A887E75354AA2CF96DE6",
        "now": 1684691616000
    },
    "has_more": 1,
    "log_pb": {
        "impr_id": "20230522015336A887E75354AA2CF96DE6"
    },
    "status_code": 0,
    "total": 586
}

  </code>
 </pre>
</details>


## 6.抖音用户视频作品列表
```
/dy/user/videos
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|secId|string|是|开头MS4的id|
|pageIndex|string|是|翻页参数，首次为0，根据下一次请求结果max_cursor值进行翻页|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    
  </code>
 </pre>
</details>


## 7.抖音用户喜欢点赞列表
```
/dy/user/likes
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|maxCursor|string|是|翻页参数，首次为0，根据下一次请求结果max_cursor值进行翻页|
|secId|string|否|MS4开头的id|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
    "aweme_list": [
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAzkWVq_QH5fFqp6RA6m7Q-d_Mg7klnBh_SVoc1VgBvsRjI2rOa5tDv9DVcrB7fs_5uqfyVUEuLtCxI44PUA2H9i1H7LElTicrDJYuF9T9VbirCbFBT7lO9x1bMljamlw_KogPBX2CelryIrxlQA9uCrjvfuLt5kK7fTGmWhuzSHVP_iP6cIFb3ZHbQ3O_PImlRvppy3bExrec5YFKBYM-y1SSe6BySGBgZMRE_IXpXi8",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7154932103690472741",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7154932103690472741,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1665887472,
            "desc": " 中国共产党第二十次全国代表大会开幕，习近平代表第十九届中央委员会向党的二十大作报告。 ",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 30106,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7154932103690472741",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7154932103690472741
                ],
                "similar_id_list_a": [
                    7154932103690472741
                ],
                "similar_id_list_b": [
                    7154932103690472741
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 30,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 30,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"has_edited\":0,\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_subsidy_exp\":false,\"aggregate_exempt_conf\":[],\"filter_reason\":\"gov_takedown\",\"review_unshelve_reason\":0,\"schedule_search_time\":0,\"hotsoon_review_time\":-1,\"extract_item_id\":7154932103690472741,\"original_song_uri\":\"ies-music/7154932206652132103.mp3\",\"with_aed_model\":1,\"dsp_switch\":0,\"reviewed\":1,\"beats\":{},\"douyin_beats_info\":{},\"is_red\":0,\"original_song_url\":\"https://sf6-sign.douyinstatic.com/ies-music/7154932206652132103.mp3?x-expires=1685008788&x-signature=%2FkAMc5xMRSSEumPIK%2B%2B9qEMmmOU%3D\",\"music_label_id\":null,\"is_aed_music\":0}",
                "id": 7154932208061516551,
                "id_str": "7154932208061516551",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7154932208061516551",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7154932208061516551",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7154932208061516551"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 30,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf26-sign.douyinstatic.com/ies-music/pattern/96b263b0127dc5ef9872e018903e10b2.json?x-expires=1685008788&x-signature=En4BjEC%2Bst%2FtZJo8DNe1FL%2BnqfU%3D",
                    "url_list": [
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/96b263b0127dc5ef9872e018903e10b2.json?x-expires=1685008788&x-signature=En4BjEC%2Bst%2FtZJo8DNe1FL%2BnqfU%3D",
                        "https://sf9-sign.douyinstatic.com/ies-music/pattern/96b263b0127dc5ef9872e018903e10b2.json?x-expires=1685008788&x-signature=4rE7oO2AgA%2BEySXK6hrUlWZOXGo%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 30
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "2.00 IvF:/  中国共产党第二十次全国代表大会开幕，习近平代表第十九届中央委员会向党的二十大作报告。   %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7154932103690472741/?region=CN&mid=7154932208061516551&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7154932103690472741/?region=CN&mid=7154932208061516551&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7154932103690472741",
                "collect_count": 55194,
                "comment_count": 89775,
                "digg_count": 2338355,
                "play_count": 0,
                "share_count": 49601
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7154932103690472741",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [
                    {
                        "duration": 30.04,
                        "fext": "jpg",
                        "img_num": 30,
                        "img_url": "http://p3-sign.douyinpic.com/tos-cn-p-0015/e3a5819a42e94ef480f93eda390ec661_1665887477~tplv-noop.image?x-expires=1684926018&x-signature=Bhnl8fHveAxbY3le4dBcx%2BQ1cbc%3D",
                        "img_x_len": 10,
                        "img_x_size": 136,
                        "img_y_len": 3,
                        "img_y_size": 202,
                        "interval": 1,
                        "uri": "tos-cn-p-0015/e3a5819a42e94ef480f93eda390ec661_1665887477"
                    }
                ],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2101092,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 7906936,
                            "file_cs": "c:0-26449-b29f|d:0-3953467-9091,3953468-7906935-d2da|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "file_hash": "8dd449124a85bdbc325cfd8939677753",
                            "height": 1600,
                            "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_1080p_2101092",
                            "url_list": [
                                "http://v3-web.douyinvod.com/bc317698a7d2077cad247abd1bfd58e2/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/1eec98fc3ca3407c86cd0a9b85ce7577/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2051&bt=2051&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDlpPDVlNDg2M2k1PDZoaEBpMzc6PDU6Zm1wZzMzNGkzM0BiMDE0YjJgNjExMF8xYDVgYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/60f45b14cd4b6e952afb9513ab5170f9/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/1eec98fc3ca3407c86cd0a9b85ce7577/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2051&bt=2051&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDlpPDVlNDg2M2k1PDZoaEBpMzc6PDU6Zm1wZzMzNGkzM0BiMDE0YjJgNjExMF8xYDVgYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=ce8ec349b23f404395c15be2794f36e1&sign=8dd449124a85bdbc325cfd8939677753&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1102237,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4147994,
                            "file_cs": "c:0-26032-d0c4|d:0-2073996-dfd9,2073997-4147993-9b63|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "file_hash": "6576bf0118b8657576a4a4a046ba0989",
                            "height": 1066,
                            "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_720p_1102237",
                            "url_list": [
                                "http://v3-web.douyinvod.com/5c20fdf89722ff44384c45ae906321e4/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/83b66f4450a14560961320d1c74326e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1076&bt=1076&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWhkPDRlOWk7aWYzM2ZoZkBpMzc6PDU6Zm1wZzMzNGkzM0AuMmE2NC1fXjUxLS5iMWI2YSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/0c7487588b21ea119f297a294e97dec0/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/83b66f4450a14560961320d1c74326e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1076&bt=1076&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWhkPDRlOWk7aWYzM2ZoZkBpMzc6PDU6Zm1wZzMzNGkzM0AuMmE2NC1fXjUxLS5iMWI2YSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=9cee4ce0100c4f88afb60b7199da5e16&sign=6576bf0118b8657576a4a4a046ba0989&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 849069,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3195261,
                            "file_cs": "c:0-26169-6bb8|d:0-1597629-cdee,1597630-3195260-3851|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "file_hash": "cb815faaf6526fd2d8d192014dce0eb0",
                            "height": 800,
                            "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_540p_849069",
                            "url_list": [
                                "http://v3-web.douyinvod.com/2d44eace252f2b819fe703cd93be4987/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/d4750d150fcb4f8d9fe947bb687856d3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=829&bt=829&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZjQ0aTg4NDM0N2Q8OzM2NUBpMzc6PDU6Zm1wZzMzNGkzM0BjLTYzM2A2NTQxYy4uYmExYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/7a2b411ba059a34f5a7fef54ef8e3dd2/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/d4750d150fcb4f8d9fe947bb687856d3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=829&bt=829&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZjQ0aTg4NDM0N2Q8OzM2NUBpMzc6PDU6Zm1wZzMzNGkzM0BjLTYzM2A2NTQxYy4uYmExYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=42d3e01819fa44718091c5656f9101fc&sign=cb815faaf6526fd2d8d192014dce0eb0&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 540
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 640833,
                        "gear_name": "normal_480_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2411617,
                            "file_cs": "c:0-26233-f756|d:0-1205807-df37,1205808-2411616-2e51|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "file_hash": "4fc85a2b0f5ee9d43d49f4eabc523daf",
                            "height": 712,
                            "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_480p_640833",
                            "url_list": [
                                "http://v3-web.douyinvod.com/0d6aa60a8fdac3b307ff1ad87644e439/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/269e0d29a3bd4066af9d41bf98f9d783/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=625&bt=625&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDU6NmY5Njw3Zjg8OmhoZEBpMzc6PDU6Zm1wZzMzNGkzM0AzL2IwXzYvNl8xXzE0NWEuYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/5185c88d28b5939f7583d67e83a5b10c/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/269e0d29a3bd4066af9d41bf98f9d783/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=625&bt=625&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDU6NmY5Njw3Zjg8OmhoZEBpMzc6PDU6Zm1wZzMzNGkzM0AzL2IwXzYvNl8xXzE0NWEuYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=1ade8e7749b54cb4992396bc33e72269&sign=4fc85a2b0f5ee9d43d49f4eabc523daf&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 480
                        },
                        "quality_type": 30,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 598815,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2262026,
                            "file_cs": "c:0-20359-06fa|d:0-1131012-115d,1131013-2262025-cf83|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "file_hash": "a3bc6beb696a1bbbcbafa3d7771d3098",
                            "height": 854,
                            "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                            "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_540p_598815",
                            "url_list": [
                                "http://v3-web.douyinvod.com/0409f173d145f7a98c895703024a58a5/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/c333ba177bad45ac9e21b5960807fb6f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=584&bt=584&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZGc1O2RlPDQ0NDc5ZzU3NEBpMzc6PDU6Zm1wZzMzNGkzM0BfX2AtYGNeXmAxLV4uNi5eYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/e35c083f2c5221363f5669bea2959b59/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/c333ba177bad45ac9e21b5960807fb6f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=584&bt=584&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZGc1O2RlPDQ0NDc5ZzU3NEBpMzc6PDU6Zm1wZzMzNGkzM0BfX2AtYGNeXmAxLV4uNi5eYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=a114921da60441c1a1a9fbca08c2bdba&sign=a3bc6beb696a1bbbcbafa3d7771d3098&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/48afeaf4e5e94a49aa389b4f73c709a0_1665887474",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/48afeaf4e5e94a49aa389b4f73c709a0_1665887474~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=2wfGQb3pP83vc1H%2FAStVGIq%2F6xk%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/48afeaf4e5e94a49aa389b4f73c709a0_1665887474?x-expires=2000278800&x-signature=Gy63l68BzqYhdFFVKabruoBtxfg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/48afeaf4e5e94a49aa389b4f73c709a0_1665887474?x-expires=2000278800&x-signature=UElYJw6UEg0vD1Z9Tg6svSKi%2BlY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/48afeaf4e5e94a49aa389b4f73c709a0_1665887474?x-expires=2000278800&x-signature=L2Fhx8OkpDShqiwpeK2IbKo%2FKws%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 4616717,
                    "height": 720,
                    "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                    "url_list": [
                        "http://v3-web.douyinvod.com/18fca7f054c637ba9f1cafc594739e8a/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/0d9310591f63497594e56f2f91013709/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1088&bt=1088&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=M2c6aDppaTtpNTZkNTloOUBpMzc6PDU6Zm1wZzMzNGkzM0AtNmIuY2M0XzMxYi8xMF8zYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/0cadd0572f14799eb46b56fa5853e214/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/0d9310591f63497594e56f2f91013709/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1088&bt=1088&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=M2c6aDppaTtpNTZkNTloOUBpMzc6PDU6Zm1wZzMzNGkzM0AtNmIuY2M0XzMxYi8xMF8zYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHH89Mkfm-8HccpW5gInZ0apqCE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 30106,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/bf6a73e148874f769d3596181a15d54b_1665887477",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bf6a73e148874f769d3596181a15d54b_1665887477?x-expires=1686128400&x-signature=0G67BzPJHdX8Arz9ifFsaYrER4I%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bf6a73e148874f769d3596181a15d54b_1665887477?x-expires=1686128400&x-signature=l0x9Hbpu0GAhNq3Gr9LC6Nwi4Cw%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bf6a73e148874f769d3596181a15d54b_1665887477?x-expires=1686128400&x-signature=98pQja9ykzHnWaqJ8LyUjLFXZzw%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1600,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"bright_ratio_mean\":\"0.0305\",\"brightness_mean\":\"177.9631\",\"diff_overexposure_ratio\":\"0.0232\",\"fullscreen_max_crop\":\"{\\\"maxcrop_left\\\": -1.0, \\\"maxcrop_right\\\": -1.0, \\\"maxcrop_top\\\": -1.0, \\\"version\\\": \\\"v1.0\\\"}\",\"loudness\":\"-23.2\",\"overexposure_ratio_mean\":\"0.092\",\"peak\":\"0.43152\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\",\"std_brightness\":\"7.1731\",\"title_info\":\"{\\\"ratio_br_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], \\\"ratio_edge_l\\\": [0.04, 0.02, 0.02, 0.04, 0.03, 0.03], \\\"version\\\": \\\"v1.0\\\"}\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fg10000cd5mpjrc77u2a9m7m4t0\",\"url_list\":[\"http://v3-web.douyinvod.com/dc6cdb5bd42552399828dbf487dae637/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/6ba6f60116f8492e889c02e38c2888cd/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1024\&bt=1024\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ZTs3NDppOjZlOmVkaTg4NkBpMzc6PDU6Zm1wZzMzNGkzM0AyNWAyMGMxNTYxXy5gMDIuYSNxampecjRvbTJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00018000\",\"http://v26-web.douyinvod.com/2172ffa1b5e59f533e8e8ddfcc4bf157/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/6ba6f60116f8492e889c02e38c2888cd/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1024\&bt=1024\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ZTs3NDppOjZlOmVkaTg4NkBpMzc6PDU6Zm1wZzMzNGkzM0AyNWAyMGMxNTYxXy5gMDIuYSNxampecjRvbTJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00018000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHH89Mkfm-8HccpW5gInZ0apqCE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":4342809}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-dy/6ec6378b8480447297464c1059344fdd",
                    "url_list": [
                        "https://p26-sign.douyinpic.com/tos-cn-i-dy/6ec6378b8480447297464c1059344fdd~noop.jpeg?x-expires=1686128400&x-signature=EzBkfOC8a1eAFwjgv6t9sUHxkGo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-dy/6ec6378b8480447297464c1059344fdd~noop.jpeg?x-expires=1686128400&x-signature=y4GR17NKdQRXMDxzGI6O5GDNqac%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-sign.douyinpic.com/tos-cn-i-dy/6ec6378b8480447297464c1059344fdd~noop.jpeg?x-expires=1686128400&x-signature=gakAxjpi%2FCsstD%2F4Nzd7PM%2BUdVo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/272333e7e5714a4983c60706b04504a3_1665887475",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/272333e7e5714a4983c60706b04504a3_1665887475~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=%2BvBn9oWBhD6IXWWaiZbvhIPdzQI%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/272333e7e5714a4983c60706b04504a3_1665887475~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=rxTuh3awRKXLiQPo%2F4yD8Yeot2M%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/272333e7e5714a4983c60706b04504a3_1665887475~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=GiWTux7UM4uxT4b6KMK5hZNWq4s%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 7906936,
                    "file_cs": "c:0-26449-b29f|d:0-3953467-9091,3953468-7906935-d2da|a:v0200fg10000cd5mpjrc77u2a9m7m4t0",
                    "file_hash": "8dd449124a85bdbc325cfd8939677753",
                    "height": 1600,
                    "uri": "v0200fg10000cd5mpjrc77u2a9m7m4t0",
                    "url_key": "v0200fg10000cd5mpjrc77u2a9m7m4t0_h264_1080p_2101092",
                    "url_list": [
                        "http://v3-web.douyinvod.com/bc317698a7d2077cad247abd1bfd58e2/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/1eec98fc3ca3407c86cd0a9b85ce7577/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2051&bt=2051&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDlpPDVlNDg2M2k1PDZoaEBpMzc6PDU6Zm1wZzMzNGkzM0BiMDE0YjJgNjExMF8xYDVgYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/60f45b14cd4b6e952afb9513ab5170f9/646dee42/video/tos/cn/tos-cn-ve-15c001-alinc2/1eec98fc3ca3407c86cd0a9b85ce7577/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2051&bt=2051&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDlpPDVlNDg2M2k1PDZoaEBpMzc6PDU6Zm1wZzMzNGkzM0BiMDE0YjJgNjExMF8xYDVgYSNxampecjRvbTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5mpjrc77u2a9m7m4t0&line=0&file_id=ce8ec349b23f404395c15be2794f36e1&sign=8dd449124a85bdbc325cfd8939677753&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018004,
                    "tag_name": "时政新闻"
                },
                {
                    "level": 3,
                    "tag_id": 2018004004,
                    "tag_name": "国内时政"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAQpTyS-Yc9qayy5uxulAGhp-QeyPmgTXlBqz-v717oYherofLqariB5Ysh8DL5HGGaPW3m7xeP3p2Glll0fohVlZkoqfWukqAWHTNvwggiPDtKA7aEGpNmMgbzsrUIqh21ehEStqRJSu-4aSkmctgY-_OVK_yE2pbh_rHBHilZFIrvJj2pkjMcAp9sIxRRP0kqLehV7v3CPMRKbynP24nU9GqwHQN79EtZPg_M6ObHdU",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7154958229108247839",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7154958229108247839,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1665893563,
            "desc": "习近平：解决台湾问题是中国人自己的事，要由中国人来决定。祖国完全统一一定要实现，也一定能够实现！  ",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 76378,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7154958229108247839",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7154958229108247839
                ],
                "similar_id_list_a": [
                    7154958229108247839
                ],
                "similar_id_list_b": [
                    7154958229108247839
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 76,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 76,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"douyin_beats_info\":{},\"hotsoon_review_time\":-1,\"aggregate_exempt_conf\":[],\"with_aed_model\":1,\"review_unshelve_reason\":0,\"beats\":{},\"is_red\":0,\"music_label_id\":null,\"is_aed_music\":0,\"dsp_switch\":0,\"is_subsidy_exp\":false,\"original_song_uri\":\"ies-music/7154958374933252900.mp3\",\"extract_item_id\":7154958229108247839,\"schedule_search_time\":0,\"reviewed\":1,\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"original_song_url\":\"https://sf6-sign.douyinstatic.com/ies-music/7154958374933252900.mp3?x-expires=1685008788&x-signature=DIiOZ0w%2BJU2lDXsG%2FINcXgoTmfs%3D\",\"filter_reason\":\"gov_takedown\",\"has_edited\":0}",
                "id": 7154958373992434440,
                "id_str": "7154958373992434440",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7154958373992434440",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7154958373992434440",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7154958373992434440"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 76,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf9-sign.douyinstatic.com/ies-music/pattern/fd4245e89f0161f322c3f276d8562947.json?x-expires=1685008788&x-signature=V6kFQp0s9XBOM%2BCI3pbC0RZdLjI%3D",
                    "url_list": [
                        "https://sf9-sign.douyinstatic.com/ies-music/pattern/fd4245e89f0161f322c3f276d8562947.json?x-expires=1685008788&x-signature=V6kFQp0s9XBOM%2BCI3pbC0RZdLjI%3D",
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/fd4245e89f0161f322c3f276d8562947.json?x-expires=1685008788&x-signature=vLddUw1iSyAqGqT5AS5iZ0SXuKU%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 76
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "2.53 DuF:/ 习近平：解决台湾问题是中国人自己的事，要由中国人来决定。祖国完全统一一定要实现，也一定能够实现！   %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7154958229108247839/?region=CN&mid=7154958373992434440&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7154958229108247839/?region=CN&mid=7154958373992434440&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7154958229108247839",
                "collect_count": 179123,
                "comment_count": 201042,
                "digg_count": 4477145,
                "play_count": 0,
                "share_count": 249644
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7154958229108247839",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [
                    {
                        "duration": 76.32,
                        "fext": "jpg",
                        "img_num": 76,
                        "img_url": "http://p3-sign.douyinpic.com/tos-cn-p-0015/f7f636b19f6f411ab6ee6812a605e57f_1665893574~tplv-noop.image?x-expires=1684926064&x-signature=UUQa19%2FzLxCcC1j2Pb8L51qLRmQ%3D",
                        "img_x_len": 10,
                        "img_x_size": 136,
                        "img_y_len": 8,
                        "img_y_size": 236,
                        "interval": 1,
                        "uri": "tos-cn-p-0015/f7f636b19f6f411ab6ee6812a605e57f_1665893574"
                    }
                ],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1507051,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 14388201,
                            "file_cs": "c:0-65430-d82c|a:v0200fg10000cd5o833c77ueumh3oadg",
                            "file_hash": "fc882136a33a2adc43cc4aa58cfa8765",
                            "height": 1870,
                            "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                            "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_1080p_1507051",
                            "url_list": [
                                "http://v3-web.douyinvod.com/c6b285af9af0a45714f1f554e4594d56/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/5d9697e0b87f415b9bb5a642b61107bb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1471&bt=1471&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmdoNzRlZTtkaTs7ZWZoNkBpamQ2cGg6ZjZyZzMzNGkzM0A2MS9hYV9iNTExNTYwNTRhYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/0b32a6ed8ed71b01442c395bf10ef8b3/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/5d9697e0b87f415b9bb5a642b61107bb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1471&bt=1471&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmdoNzRlZTtkaTs7ZWZoNkBpamQ2cGg6ZjZyZzMzNGkzM0A2MS9hYV9iNTExNTYwNTRhYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=d37e8c3b98884f4a88ebbbd1d42e4d9c&sign=fc882136a33a2adc43cc4aa58cfa8765&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 629962,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 6014406,
                            "file_cs": "c:0-65413-c0ae|a:v0200fg10000cd5o833c77ueumh3oadg",
                            "file_hash": "1c98e4caac6a480b45e08801d426fba4",
                            "height": 1246,
                            "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                            "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_720p_629962",
                            "url_list": [
                                "http://v3-web.douyinvod.com/805fa493eff073b5fa2036c7b5d8bdd0/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/c9aa954cb7134039bd82e8d51bd77bdb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=615&bt=615&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=MzhpZWc0N2Y3aWY2MzMzOkBpamQ2cGg6ZjZyZzMzNGkzM0BiMi00NGM2NmExYDZfLV81YSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/a9c86c14b59e2dd2aa31b16fe7b74412/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/c9aa954cb7134039bd82e8d51bd77bdb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=615&bt=615&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=MzhpZWc0N2Y3aWY2MzMzOkBpamQ2cGg6ZjZyZzMzNGkzM0BiMi00NGM2NmExYDZfLV81YSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=87b000b093cc4fd49c94f17d7b0f55e0&sign=1c98e4caac6a480b45e08801d426fba4&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 462048,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4411294,
                            "file_cs": "c:0-65324-b093|a:v0200fg10000cd5o833c77ueumh3oadg",
                            "file_hash": "653bf972715843cba4b7caf49fd53eb9",
                            "height": 936,
                            "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                            "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_540p_462048",
                            "url_list": [
                                "http://v3-web.douyinvod.com/898814f079951dca94f4d7b77785eb9d/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/d8b65fc3fd174ad48d6a17de6d9dcd91/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=451&bt=451&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTtkZmk4PDs1NWZlaDQ6ZEBpamQ2cGg6ZjZyZzMzNGkzM0AzNGNgLS0tNjMxY2M0MzUuYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/5e797373033e5ff0c018eba1654350cc/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/d8b65fc3fd174ad48d6a17de6d9dcd91/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=451&bt=451&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTtkZmk4PDs1NWZlaDQ6ZEBpamQ2cGg6ZjZyZzMzNGkzM0AzNGNgLS0tNjMxY2M0MzUuYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=1a87617efbfc42629809050fccfa786f&sign=653bf972715843cba4b7caf49fd53eb9&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 540
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 343314,
                        "gear_name": "normal_480_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3277710,
                            "file_cs": "c:0-65260-ced4|a:v0200fg10000cd5o833c77ueumh3oadg",
                            "file_hash": "53e2691f3febb56fb3e4d49eeaaca9c4",
                            "height": 832,
                            "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                            "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_480p_343314",
                            "url_list": [
                                "http://v3-web.douyinvod.com/bc58e4a732d087c967a9c76f20bc1868/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/1c6570f5410b4bbba4ea0b916a00f6c6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=335&bt=335&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZjQ6N2k1NTo3ZzQ0PDY0NkBpamQ2cGg6ZjZyZzMzNGkzM0BeNjAuMzMxNWMxM2M2NjIwYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/ccfafc93bf1afbb4e4772d98c85e688b/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/1c6570f5410b4bbba4ea0b916a00f6c6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=335&bt=335&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZjQ6N2k1NTo3ZzQ0PDY0NkBpamQ2cGg6ZjZyZzMzNGkzM0BeNjAuMzMxNWMxM2M2NjIwYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=33519399f1614df48742626f143791ac&sign=53e2691f3febb56fb3e4d49eeaaca9c4&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 480
                        },
                        "quality_type": 30,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 315598,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3017592,
                            "file_cs": "c:0-50339-ec2e|a:v0200fg10000cd5o833c77ueumh3oadg",
                            "file_hash": "2259f416a59adbdde3c06617ff1450d6",
                            "height": 998,
                            "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                            "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_540p_315598",
                            "url_list": [
                                "http://v3-web.douyinvod.com/276b8b50d8af1877c14f086bbe0a44a7/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/7b8c8f1c3a6c4170b565df1063b57784/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=308&bt=308&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=aTZlOmQ0MzU3OTtpNGQ1OUBpamQ2cGg6ZjZyZzMzNGkzM0AzMmFfLWNfX14xYmFiMF41YSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/fdee1be477be1cf9d6c0e03eb94f4059/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/7b8c8f1c3a6c4170b565df1063b57784/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=308&bt=308&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=aTZlOmQ0MzU3OTtpNGQ1OUBpamQ2cGg6ZjZyZzMzNGkzM0AzMmFfLWNfX14xYmFiMF41YSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=86a23ae1dfe846a4b2b0f10ab7db536f&sign=2259f416a59adbdde3c06617ff1450d6&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/bffc70fb0e8549aa9184cd89825941da_1665893567",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/bffc70fb0e8549aa9184cd89825941da_1665893567~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=5Iu0q8IiQrQNwqrO5U4AiBRgoRE%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bffc70fb0e8549aa9184cd89825941da_1665893567?x-expires=2000278800&x-signature=QZ1rMaojysgoRJR5lRdV6vC%2Fq1w%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bffc70fb0e8549aa9184cd89825941da_1665893567?x-expires=2000278800&x-signature=CYkkW1EqtJEnx8I5alq0B9UI5vs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bffc70fb0e8549aa9184cd89825941da_1665893567?x-expires=2000278800&x-signature=HebQ4KbPOAg1i0afliV25dnIxC8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 6920698,
                    "height": 720,
                    "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/5e9a007736ce2413e2d65ede7fe921e0/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/9caac50668984002bdfc32473ece7081/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=680&bt=680&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODpmZDdkZWY0NDs3ODQ0NUBpamQ2cGg6ZjZyZzMzNGkzM0A1MjZgXy8uXzIxLS1gYS8xYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/913750c7c010cd8eab83dcb32163d56a/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/9caac50668984002bdfc32473ece7081/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=680&bt=680&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODpmZDdkZWY0NDs3ODQ0NUBpamQ2cGg6ZjZyZzMzNGkzM0A1MjZgXy8uXzIxLS1gYS8xYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHH89FsJy68HccpDIxcmJkY87DT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 76378,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/190b5dab99854f8c8905d3417fd3a74f_1665893569",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/190b5dab99854f8c8905d3417fd3a74f_1665893569?x-expires=1686128400&x-signature=j3QsXCjQojyr4nIjuG5oH%2BtLijc%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/190b5dab99854f8c8905d3417fd3a74f_1665893569?x-expires=1686128400&x-signature=mKOQRY61nvd%2BFsLYiQxNZi56jik%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/190b5dab99854f8c8905d3417fd3a74f_1665893569?x-expires=1686128400&x-signature=9VX%2F1l66qIF2M9yPQ78xFfA2NxA%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_long_video": 1,
                "is_source_HDR": 0,
                "meta": "{\"bright_ratio_mean\":\"0.0262\",\"brightness_mean\":\"176.2612\",\"diff_overexposure_ratio\":\"0.0029\",\"fullscreen_max_crop\":\"{\\\"maxcrop_left\\\": -1.0, \\\"maxcrop_right\\\": -1.0, \\\"maxcrop_top\\\": -1.0, \\\"version\\\": \\\"v1.0\\\"}\",\"loudness\":\"-18\",\"overexposure_ratio_mean\":\"0.23\",\"peak\":\"0.96605\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\",\"std_brightness\":\"0.7397\",\"title_info\":\"{\\\"ratio_br_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.03], \\\"ratio_edge_l\\\": [0.04, 0.06, 0.06, 0.09, 0.2, 0.2], \\\"progress_bar\\\": [0.0, 0.0, 0.0], \\\"bullet_zone\\\": 0.36, \\\"version\\\": \\\"v1.0\\\"}\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fg10000cd5o833c77ueumh3oadg\",\"url_list\":[\"http://v3-web.douyinvod.com/eb8431bef478bd403ff3cb0386c10e82/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/f355193359064b5a971d09e5a16c49c0/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=660\&bt=660\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=Zzk2O2c3OjQ4ZzhkaWZpZUBpamQ2cGg6ZjZyZzMzNGkzM0BeMjVfMGI0XmMxYTQ0MmEvYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"http://v26-web.douyinvod.com/da5a89ae4b373ba62033ded545de6d6d/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/f355193359064b5a971d09e5a16c49c0/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=660\&bt=660\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=Zzk2O2c3OjQ4ZzhkaWZpZUBpamQ2cGg6ZjZyZzMzNGkzM0BeMjVfMGI0XmMxYTQ0MmEvYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHH89FsJy68HccpDIxcmJkY87DT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":6715889}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-dy/3692e5d6121e46b0af30546aab0be5f4",
                    "url_list": [
                        "https://p9-sign.douyinpic.com/tos-cn-i-dy/3692e5d6121e46b0af30546aab0be5f4~noop.jpeg?x-expires=1686128400&x-signature=f8N2I4Rm5n91abSxYNAgZ3Sn9GM%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-dy/3692e5d6121e46b0af30546aab0be5f4~noop.jpeg?x-expires=1686128400&x-signature=elNU1sj1HrycSNdODhQ3piFZg7w%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p26-sign.douyinpic.com/tos-cn-i-dy/3692e5d6121e46b0af30546aab0be5f4~noop.jpeg?x-expires=1686128400&x-signature=woHCLS05%2Bdke9HWS%2FUILVHM%2F3Dw%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/1716b9190daa427788172b66c6fb8a20_1665893568",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/1716b9190daa427788172b66c6fb8a20_1665893568~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=%2BBBo6LcU8tWWuxqby%2FOFd8hLN5o%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/1716b9190daa427788172b66c6fb8a20_1665893568~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=%2BHtiL7h%2FFZ5c48lopagoVFVSxKw%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/1716b9190daa427788172b66c6fb8a20_1665893568~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=JBJxgOOtjEYRR2lV2Lz5xEeQdFk%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 14388201,
                    "file_cs": "c:0-65430-d82c|a:v0200fg10000cd5o833c77ueumh3oadg",
                    "file_hash": "fc882136a33a2adc43cc4aa58cfa8765",
                    "height": 1870,
                    "uri": "v0200fg10000cd5o833c77ueumh3oadg",
                    "url_key": "v0200fg10000cd5o833c77ueumh3oadg_h264_1080p_1507051",
                    "url_list": [
                        "http://v3-web.douyinvod.com/c6b285af9af0a45714f1f554e4594d56/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/5d9697e0b87f415b9bb5a642b61107bb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1471&bt=1471&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmdoNzRlZTtkaTs7ZWZoNkBpamQ2cGg6ZjZyZzMzNGkzM0A2MS9hYV9iNTExNTYwNTRhYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/0b32a6ed8ed71b01442c395bf10ef8b3/646dee70/video/tos/cn/tos-cn-ve-15c001-alinc2/5d9697e0b87f415b9bb5a642b61107bb/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1471&bt=1471&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmdoNzRlZTtkaTs7ZWZoNkBpamQ2cGg6ZjZyZzMzNGkzM0A2MS9hYV9iNTExNTYwNTRhYSNhbGVycjQwNTJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd5o833c77ueumh3oadg&line=0&file_id=d37e8c3b98884f4a88ebbbd1d42e4d9c&sign=fc882136a33a2adc43cc4aa58cfa8765&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018004,
                    "tag_name": "时政新闻"
                },
                {
                    "level": 3,
                    "tag_id": 2018004002,
                    "tag_name": "港澳台地区"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAA3sUUn3SVxVCc3SYt5mbVWRTCdLBw72pWUssGHM-EYzE2XCPiCLbEtbwXKZa51Ro_S3zd9IqQ80bvlymSvfEcVg0qtFnaJCP8gDBmAbU4sl3-KuBULnSApBWnEN-q1roiU6th3N8Y0y7THO1BaGyktYcyWAp_AYoPP9uo6d4APY_YE2yqOPBP04C_bOUD73v-WtjhwH_omjmfsy60Fk1_FOL5Xgl--a-IFLTSxoly8v0",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7153632346107890952",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7153632346107890952,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1665619260,
            "desc": "祖国的领土，寸土不让！感受“卫国戍边英雄团长”祁发宝的铁汉柔情与铮铮誓言。#领航 ",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 25967,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7153632346107890952",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7153632346107890952
                ],
                "similar_id_list_a": [
                    7153632346107890952
                ],
                "similar_id_list_b": [
                    7153632346107890952
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 25,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 25,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"dsp_switch\":0,\"douyin_beats_info\":{},\"schedule_search_time\":0,\"music_label_id\":null,\"is_aed_music\":0,\"hotsoon_review_time\":-1,\"is_subsidy_exp\":false,\"original_song_url\":\"https://sf6-sign.douyinstatic.com/ies-music/7153632393306458917.mp3?x-expires=1685008788&x-signature=lEs9k7LdP59ozGoPFaufr3FLZVE%3D\",\"aggregate_exempt_conf\":[],\"filter_reason\":\"gov_takedown\",\"extract_item_id\":7153632346107890952,\"has_edited\":0,\"beats\":{},\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"original_song_uri\":\"ies-music/7153632393306458917.mp3\",\"reviewed\":1,\"review_unshelve_reason\":0,\"is_red\":0,\"with_aed_model\":1}",
                "id": 7153632400999435021,
                "id_str": "7153632400999435021",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7153632400999435021",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7153632400999435021",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7153632400999435021"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 25,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 25
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "0.74 CUl:/ 祖国的领土，寸土不让！感受“卫国戍边英雄团长”祁发宝的铁汉柔情与铮铮誓言。# 领航   %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7153632346107890952/?region=CN&mid=7153632400999435021&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7153632346107890952/?region=CN&mid=7153632400999435021&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7153632346107890952",
                "collect_count": 87702,
                "comment_count": 316252,
                "digg_count": 4818200,
                "play_count": 0,
                "share_count": 56347
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7153632346107890952",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [
                {
                    "end": 40,
                    "hashtag_id": "1627705646074892",
                    "hashtag_name": "领航",
                    "is_commerce": false,
                    "start": 37,
                    "type": 1
                }
            ],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2023607,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 6568377,
                            "file_cs": "c:0-23117-3791|d:0-3284187-4207,3284188-6568376-2eab|a:v0200fg10000cd3csmjc77u0556hut3g",
                            "file_hash": "8e40be720be20e0d16bc57cd746363e7",
                            "height": 1440,
                            "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                            "url_key": "v0200fg10000cd3csmjc77u0556hut3g_h264_1080p_2023607",
                            "url_list": [
                                "http://v3-web.douyinvod.com/61d89ace045d399b5ce7686496082f8c/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/b65a2e3b36a940bd84f38005c26009e5/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1976&bt=1976&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs4MzY6ZDY4ZDQ2aTVoOEBpandrODM6ZnBmZzMzNGkzM0AwNDQ2My0yNjAxMGBhX2BhYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/2b3897286535a4e5fc9e4e935783fe9d/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/b65a2e3b36a940bd84f38005c26009e5/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1976&bt=1976&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs4MzY6ZDY4ZDQ2aTVoOEBpandrODM6ZnBmZzMzNGkzM0AwNDQ2My0yNjAxMGBhX2BhYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&file_id=d5ceb2dfc3314a35935a076390757838&sign=8e40be720be20e0d16bc57cd746363e7&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1250600,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4059293,
                            "file_cs": "c:0-23067-5e5c|d:0-2029645-6945,2029646-4059292-b631|a:v0200fg10000cd3csmjc77u0556hut3g",
                            "file_hash": "3326d0e6c6c50e342dfa12b4fe402026",
                            "height": 960,
                            "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                            "url_key": "v0200fg10000cd3csmjc77u0556hut3g_h264_720p_1250600",
                            "url_list": [
                                "http://v3-web.douyinvod.com/2b2a019a5fbb03de8d3815a7534fc7e6/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/c35a8244550440bd8a31192a0ad75f45/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1221&bt=1221&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZTw0aGU3OGk5ZTtpM2U1NkBpandrODM6ZnBmZzMzNGkzM0AwXzM1LmJfXzQxYS8xX2AvYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/167703f0ad8af3e5f2e991da4973ea13/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/c35a8244550440bd8a31192a0ad75f45/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1221&bt=1221&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZTw0aGU3OGk5ZTtpM2U1NkBpandrODM6ZnBmZzMzNGkzM0AwXzM1LmJfXzQxYS8xX2AvYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&file_id=23c2bb402fd84b76bfb5e41b8e61b93b&sign=3326d0e6c6c50e342dfa12b4fe402026&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1172467,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3805682,
                            "file_cs": "c:0-23028-1c96|d:0-1902840-ed08,1902841-3805681-9fdf|a:v0200fg10000cd3csmjc77u0556hut3g",
                            "file_hash": "afe6fa7212fefce6390d8b8e85d79c46",
                            "height": 768,
                            "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                            "url_key": "v0200fg10000cd3csmjc77u0556hut3g_h264_540p_1172467",
                            "url_list": [
                                "http://v3-web.douyinvod.com/02fa5148b2b0702417c9ddff6622d7f1/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/5c13a69755b24a0dabcf992ed18ab42d/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1144&bt=1144&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NjU4ZTNoNzM6NDU3Nzw1aEBpandrODM6ZnBmZzMzNGkzM0AwMjVhYDUyNTQxNF5gNTE2YSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/c7dc2a272d7f6f437fd499d5f5222f06/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/5c13a69755b24a0dabcf992ed18ab42d/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1144&bt=1144&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NjU4ZTNoNzM6NDU3Nzw1aEBpandrODM6ZnBmZzMzNGkzM0AwMjVhYDUyNTQxNF5gNTE2YSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&file_id=9e4289c4a472417780548ec0db855233&sign=afe6fa7212fefce6390d8b8e85d79c46&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 781964,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2549400,
                            "file_cs": "c:0-18158-b8ad|d:0-1274699-6334,1274700-2549399-db25|a:v0200fg10000cd3csmjc77u0556hut3g",
                            "file_hash": "1d49bf491a24b183ce897272ada3ffe1",
                            "height": 768,
                            "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                            "url_key": "v0200fg10000cd3csmjc77u0556hut3g_h264_540p_781964",
                            "url_list": [
                                "http://v3-web.douyinvod.com/1007f437be2b46ac68cdc3818c2ad110/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/705d6be3ce9b4467999a077a5f5c2f18/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=763&bt=763&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZzRmNzQzZWdnaWc7NjZoZEBpandrODM6ZnBmZzMzNGkzM0A2L2ItMzQuNmMxY19fNGJgYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/caa2d4ba10a48fc9ef211b3e04f6d586/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/705d6be3ce9b4467999a077a5f5c2f18/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=763&bt=763&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZzRmNzQzZWdnaWc7NjZoZEBpandrODM6ZnBmZzMzNGkzM0A2L2ItMzQuNmMxY19fNGJgYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&file_id=caee73b3b8fd4ffd9d1b706104ec219d&sign=1d49bf491a24b183ce897272ada3ffe1&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/53a934c7c96a42ffa718aa167d4c847c_1665584839",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/53a934c7c96a42ffa718aa167d4c847c_1665584839~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=E%2FcGVVMtI0WwyiylDZIwr4tlmF8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/53a934c7c96a42ffa718aa167d4c847c_1665584839?x-expires=2000278800&x-signature=jvQQUtJwOpvo1vTFFgBSFVt%2BmP0%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/53a934c7c96a42ffa718aa167d4c847c_1665584839?x-expires=2000278800&x-signature=zVblU0q7Qlwz0pVcmsjLopq3L8I%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/53a934c7c96a42ffa718aa167d4c847c_1665584839?x-expires=2000278800&x-signature=sMLPpa0khD82gGDJ6n8yiSatJcs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 5481835,
                    "height": 720,
                    "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                    "url_list": [
                        "http://v3-web.douyinvod.com/178d5f8b0d39b527e8c8cd5e7549cbf5/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/e525fe1d1354431ca63a2e8126c1bae8/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1477&bt=1477&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2PDRoZjdmPDo7OmlnO0BpandrODM6ZnBmZzMzNGkzM0BeNGMuLy8uNTUxLWM1MV40YSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/63adc6260dca6a60e16deb7a2d1dab92/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/e525fe1d1354431ca63a2e8126c1bae8/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1477&bt=1477&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2PDRoZjdmPDo7OmlnO0BpandrODM6ZnBmZzMzNGkzM0BeNGMuLy8uNTUxLWM1MV40YSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHH9d0neXe8HccpWcwExsIC5ufT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 25967,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/f7369265aa5c4697b9dba52ebaa517a4_1665584844",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/f7369265aa5c4697b9dba52ebaa517a4_1665584844?x-expires=1686128400&x-signature=CZCKszSNI0x5xxtioA%2F0mL7KrJ0%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/f7369265aa5c4697b9dba52ebaa517a4_1665584844?x-expires=1686128400&x-signature=DQyg4xxSlX%2Bj9Z%2Fi7Gv0AvFPSh0%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/f7369265aa5c4697b9dba52ebaa517a4_1665584844?x-expires=1686128400&x-signature=ZYNQrYJLzuVDiaS7FVnG%2BFICTTk%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1440,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"bright_ratio_mean\":\"0.0756\",\"brightness_mean\":\"137.2229\",\"diff_overexposure_ratio\":\"0.0069\",\"fullscreen_max_crop\":\"{\\\"maxcrop_left\\\": -1.0, \\\"maxcrop_right\\\": -1.0, \\\"maxcrop_top\\\": -1.0, \\\"version\\\": \\\"v1.0\\\"}\",\"loudness\":\"-11.2\",\"overexposure_ratio_mean\":\"0.0133\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\",\"std_brightness\":\"21.1219\",\"title_info\":\"{\\\"ratio_br_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], \\\"ratio_edge_l\\\": [0.0, 0.14, 0.33, 0.42, 0.49, 0.44], \\\"version\\\": \\\"v1.0\\\"}\"}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-dy/ebec7fbf33e145d4bf12f8b16002b331",
                    "url_list": [
                        "https://p26-sign.douyinpic.com/tos-cn-i-dy/ebec7fbf33e145d4bf12f8b16002b331~noop.jpeg?x-expires=1686128400&x-signature=nVWaxMJuwkL9Q6WJddsKzImM%2FoQ%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-sign.douyinpic.com/tos-cn-i-dy/ebec7fbf33e145d4bf12f8b16002b331~noop.jpeg?x-expires=1686128400&x-signature=j76qd0JF03hFicZUINeMPrcviB0%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-dy/ebec7fbf33e145d4bf12f8b16002b331~noop.jpeg?x-expires=1686128400&x-signature=%2FrxFquccpaTxb2kPMEyKNcv5orI%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/f4a56b49603c42eb96a6a5e0990004cf_1665584840",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/f4a56b49603c42eb96a6a5e0990004cf_1665584840~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=nZMxv7KryEebnMqe8n6OpUreXZY%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/f4a56b49603c42eb96a6a5e0990004cf_1665584840~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=eWj45WkVzfZeKfSlW0gGwUDeMoE%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/f4a56b49603c42eb96a6a5e0990004cf_1665584840~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=cqPT9wUqVKAB2sr83YjTLo7dGoY%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 6568377,
                    "file_cs": "c:0-23117-3791|d:0-3284187-4207,3284188-6568376-2eab|a:v0200fg10000cd3csmjc77u0556hut3g",
                    "file_hash": "8e40be720be20e0d16bc57cd746363e7",
                    "height": 1440,
                    "uri": "v0200fg10000cd3csmjc77u0556hut3g",
                    "url_key": "v0200fg10000cd3csmjc77u0556hut3g_h264_1080p_2023607",
                    "url_list": [
                        "http://v3-web.douyinvod.com/61d89ace045d399b5ce7686496082f8c/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/b65a2e3b36a940bd84f38005c26009e5/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1976&bt=1976&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs4MzY6ZDY4ZDQ2aTVoOEBpandrODM6ZnBmZzMzNGkzM0AwNDQ2My0yNjAxMGBhX2BhYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/2b3897286535a4e5fc9e4e935783fe9d/646dee3d/video/tos/cn/tos-cn-ve-15c001-alinc2/b65a2e3b36a940bd84f38005c26009e5/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1976&bt=1976&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs4MzY6ZDY4ZDQ2aTVoOEBpandrODM6ZnBmZzMzNGkzM0AwNDQ2My0yNjAxMGBhX2BhYSMwcjMycjRncDBgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000cd3csmjc77u0556hut3g&line=0&file_id=d5ceb2dfc3314a35935a076390757838&sign=8e40be720be20e0d16bc57cd746363e7&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018006,
                    "tag_name": "政务宣传"
                },
                {
                    "level": 3,
                    "tag_id": 2018006001,
                    "tag_name": "宣教科普"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAA6SisZos7sIoKYVH3fuAv5Ee8jCk9-dL1-QVyJYn3cgnNtihY9z9w8RhARfPCAymbAtCw61VYuc7Bnykku6_moTM8zUklpw_0b23GW2b04_qP8IGyfnEPFomRxjLWxILAj31B_ywidop0h98ocUD_nEqBf0NVjSjSbNzFsmS3SEhqDcIu7xZ-i5aSUhD9itC-hYROZJ3Mc3xRAocSOkHGxUvGreFoHH8Lhb7nfhpAjj0",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7149315274058091807",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7149315274058091807,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1664579716,
            "desc": " 完整版！天安门广场举行2022年国庆升旗仪式。祝福祖国！ ",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 213935,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7035428400386919684",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7013890000278408482,
                    7035428400386919684,
                    7149299458579254535,
                    7013872489084341517,
                    7149299098179489039,
                    7149300165046734095,
                    7149299322192989481,
                    7149300524712545576,
                    7149301547938188578,
                    7149299900226850080,
                    7149303552563905039,
                    7149300555297377543,
                    7149299900226850080,
                    7149300524712545576,
                    7149300555297377543,
                    7149301547938188578
                ],
                "similar_id_list_a": [
                    7149315274058091807
                ],
                "similar_id_list_b": [
                    7149315274058091807
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 213,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 213,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"dsp_switch\":0,\"schedule_search_time\":0,\"hotsoon_review_time\":-1,\"music_label_id\":null,\"extract_item_id\":7149315274058091807,\"with_aed_model\":1,\"beats\":{},\"douyin_beats_info\":{},\"original_song_uri\":\"ies-music/7149315453490449188.mp3\",\"filter_reason\":\"gov_takedown\",\"has_edited\":0,\"reviewed\":1,\"is_red\":0,\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/7149315453490449188.mp3?x-expires=1685008788&x-signature=k41zJjpS%2BLLY28ALuT8yF8eJuw0%3D\",\"aggregate_exempt_conf\":[],\"is_aed_music\":0,\"review_unshelve_reason\":0,\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_subsidy_exp\":false}",
                "id": 7149315454400547614,
                "id_str": "7149315454400547614",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7149315454400547614",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7149315454400547614",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7149315454400547614"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 213,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf3-sign.douyinstatic.com/ies-music/pattern/f1e9c6ce3e247c6b043912c916b6003f.json?x-expires=1685008788&x-signature=xw8wjSf1yC3Jj%2BPJGHwmBZNGdl0%3D",
                    "url_list": [
                        "https://sf3-sign.douyinstatic.com/ies-music/pattern/f1e9c6ce3e247c6b043912c916b6003f.json?x-expires=1685008788&x-signature=xw8wjSf1yC3Jj%2BPJGHwmBZNGdl0%3D",
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/f1e9c6ce3e247c6b043912c916b6003f.json?x-expires=1685008788&x-signature=zG8p5tET5wrSVc3nuImJk%2FQYO3s%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 213
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "5.15 iPk:/  完整版！天安门广场举行2022年国庆升旗仪式。祝福祖国！   %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7149315274058091807/?region=CN&mid=7149315454400547614&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7149315274058091807/?region=CN&mid=7149315454400547614&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7149315274058091807",
                "collect_count": 495291,
                "comment_count": 563136,
                "digg_count": 9010670,
                "play_count": 0,
                "share_count": 761543
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7149315274058091807",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "大家都在搜：",
                        "icon_url": "",
                        "scene": "comment_top_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "外国人看天安门升旗仪式",
                                "word_id": "6583122800377074947"
                            }
                        ]
                    },
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "阅兵",
                                "word_id": "6537267702241711367"
                            }
                        ]
                    },
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "外国人看天安门升旗仪式",
                                "word_id": "6583122800377074947"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [
                    {
                        "duration": 213.88,
                        "fext": "jpg",
                        "img_num": 214,
                        "img_url": "http://p3-sign.douyinpic.com/tos-cn-p-0015/8fb90d43439842f0876da93b5386f137_1664579738~tplv-noop.image?x-expires=1684926201&x-signature=xTQV%2Bi5Dsh8D9NWQ75m85ljKZgs%3D",
                        "img_x_len": 10,
                        "img_x_size": 136,
                        "img_y_len": 22,
                        "img_y_size": 182,
                        "interval": 1,
                        "uri": "tos-cn-p-0015/8fb90d43439842f0876da93b5386f137_1664579738"
                    }
                ],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2154292,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 57609834,
                            "file_cs": "c:0-179949-ba67|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "file_hash": "69a94327d4c0de52edf2ea227b01756c",
                            "height": 1440,
                            "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_1080p_2154292",
                            "url_list": [
                                "http://v3-web.douyinvod.com/7824920b174b467de4d6575fb3daef3d/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/fca21134256544d9b36f89422927968c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2103&bt=2103&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTNkOzs3PDVkZjtlMzloOEBpajl0Zzc6ZnBxZjMzNGkzM0AyMy0uX2IwNjMxLWAwLi8zYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/f82b27da1faee67377d0d42689be157d/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/fca21134256544d9b36f89422927968c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2103&bt=2103&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTNkOzs3PDVkZjtlMzloOEBpajl0Zzc6ZnBxZjMzNGkzM0AyMy0uX2IwNjMxLWAwLi8zYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=652e1630cb084c6a9239e4b8180a605f&sign=69a94327d4c0de52edf2ea227b01756c&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 998970,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 26714346,
                            "file_cs": "c:0-179900-6507|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "file_hash": "ccfe3b1f7646c16cd120d5b264d65703",
                            "height": 960,
                            "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_720p_998970",
                            "url_list": [
                                "http://v3-web.douyinvod.com/6b2db9127aeff6dff8b554f87d4918f4/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/7f19fd016663496d807fa6509178df2f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=975&bt=975&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OGQ8OWc7NDRpNzc3PGgzOkBpajl0Zzc6ZnBxZjMzNGkzM0BeNWEzYmE1Ni0xLi0uXy9fYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/89286caa8e5b94f734a7d0b5beecb150/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/7f19fd016663496d807fa6509178df2f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=975&bt=975&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OGQ8OWc7NDRpNzc3PGgzOkBpajl0Zzc6ZnBxZjMzNGkzM0BeNWEzYmE1Ni0xLi0uXy9fYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=b720be190414440f9181d8ed66d98aa5&sign=ccfe3b1f7646c16cd120d5b264d65703&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 791142,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 21156647,
                            "file_cs": "c:0-179693-dee1|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "file_hash": "c6ec83a3d593530bd4edb6b55b827ec1",
                            "height": 720,
                            "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_540p_791142",
                            "url_list": [
                                "http://v3-web.douyinvod.com/14846f0dee1136ca0d05792a9d607c8b/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/76a9176aba274ee7a754e51c684c9fe2/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=772&bt=772&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Nzg1Zzk5NjpmNDU0OGU4M0Bpajl0Zzc6ZnBxZjMzNGkzM0BgXzQwYmIvNmIxXzUxMV82YSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/8de748f4d31e3858b20434fbe34e3681/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/76a9176aba274ee7a754e51c684c9fe2/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=772&bt=772&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Nzg1Zzk5NjpmNDU0OGU4M0Bpajl0Zzc6ZnBxZjMzNGkzM0BgXzQwYmIvNmIxXzUxMV82YSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=90b54b4581b241ec9723e6e63d72b5c4&sign=c6ec83a3d593530bd4edb6b55b827ec1&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 540
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 591586,
                        "gear_name": "normal_480_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 15820130,
                            "file_cs": "c:0-179756-6ee6|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "file_hash": "a8c66e27d226320873960b2346e1e992",
                            "height": 640,
                            "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_480p_591586",
                            "url_list": [
                                "http://v3-web.douyinvod.com/4603c4cae90e464a6ca7e44fc32cef7b/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/73a9e3feafaf4eb888868e2d3db0392f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=577&bt=577&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDg8M2g2Zmg3OzY6aTo3NkBpajl0Zzc6ZnBxZjMzNGkzM0BfNGJeX2ItXy8xNjYwYzAxYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/b6b801284a224be3b4b4f357b16fc8a9/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/73a9e3feafaf4eb888868e2d3db0392f/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=577&bt=577&cs=0&ds=2&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDg8M2g2Zmg3OzY6aTo3NkBpajl0Zzc6ZnBxZjMzNGkzM0BfNGJeX2ItXy8xNjYwYzAxYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=4334f73f97934824be0ce3bea0e975b1&sign=a8c66e27d226320873960b2346e1e992&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 480
                        },
                        "quality_type": 30,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 554335,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 14831933,
                            "file_cs": "c:0-137670-8616|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "file_hash": "48a18d7fd8339ae8bc9ab492dff43dcb",
                            "height": 768,
                            "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                            "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_540p_554335",
                            "url_list": [
                                "http://v3-web.douyinvod.com/c0b7370d10172f75adad52b623ddb9e9/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/7526066021fc41afaa99ebe44626cb99/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=541&bt=541&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZWk7ZGYzOGg2ZTw6NWdmZEBpajl0Zzc6ZnBxZjMzNGkzM0A2Mi5gMC8zXzAxLzZhYjYxYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/8551f2cb400c3fc475d0b2b5230a788f/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/7526066021fc41afaa99ebe44626cb99/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=541&bt=541&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZWk7ZGYzOGg2ZTw6NWdmZEBpajl0Zzc6ZnBxZjMzNGkzM0A2Mi5gMC8zXzAxLzZhYjYxYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=4a9cedd297294b33be65203cca185f9b&sign=48a18d7fd8339ae8bc9ab492dff43dcb&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/5df9af74278e43a0b355e92b88b3d316_1664579724",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/5df9af74278e43a0b355e92b88b3d316_1664579724~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=7RGDM6EsH%2BpenyR5RtKmThMc1gQ%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/5df9af74278e43a0b355e92b88b3d316_1664579724?x-expires=2000278800&x-signature=9hkVuZ9yxPkCV3ZsURT%2Bhaz8bqA%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/5df9af74278e43a0b355e92b88b3d316_1664579724?x-expires=2000278800&x-signature=QByQ8I9feer39HuA00AkkYaLPzY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/5df9af74278e43a0b355e92b88b3d316_1664579724?x-expires=2000278800&x-signature=Dv5l8IkYDA3bew8xolEQkAwhRS4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 30253091,
                    "height": 720,
                    "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/e91ae427c9cbd17c63cc9fc7117cb8b0/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/de7082d9681748a68c0e0658b7bd761e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1089&bt=1089&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODo4ZDRnZjk2NGQ8ZWg2NUBpajl0Zzc6ZnBxZjMzNGkzM0BiNjReMl4yNV4xMzA0LzQ0YSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/a6c6cb8dc50695c9cffe09a433ff3acc/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/de7082d9681748a68c0e0658b7bd761e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1089&bt=1089&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODo4ZDRnZjk2NGQ8ZWg2NUBpajl0Zzc6ZnBxZjMzNGkzM0BiNjReMl4yNV4xMzA0LzQ0YSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHAtNAyeX-8HccpXYtVltsSpKTT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 213935,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/bae458f8c0b543b4be5fa133727d9173_1664579723",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bae458f8c0b543b4be5fa133727d9173_1664579723?x-expires=1686128400&x-signature=x0LocCrYm6GBOyxTavyRM4DJ6FQ%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bae458f8c0b543b4be5fa133727d9173_1664579723?x-expires=1686128400&x-signature=WSho8mZlaBEQJTuwt0SHsCODSbw%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/bae458f8c0b543b4be5fa133727d9173_1664579723?x-expires=1686128400&x-signature=qgVzGOirjeBwLdCljvz6f1D2K6w%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1440,
                "is_h265": 0,
                "is_long_video": 1,
                "is_source_HDR": 0,
                "meta": "{\"bright_ratio_mean\":\"0.0678\",\"brightness_mean\":\"78.1183\",\"diff_overexposure_ratio\":\"0.0672\",\"fullscreen_max_crop\":\"{\\\"maxcrop_left\\\": -1.0, \\\"maxcrop_right\\\": -1.0, \\\"maxcrop_top\\\": -1.0, \\\"version\\\": \\\"v1.0\\\"}\",\"loudness\":\"-22.1\",\"overexposure_ratio_mean\":\"0.1362\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sandwich_info\":\"{\\\"version\\\":\\\"v1.7\\\",\\\"top\\\":0.24514,\\\"bottom\\\":0.66875,\\\"right\\\":1}\",\"sr_score\":\"1.000\",\"std_brightness\":\"8.3395\",\"title_info\":\"{\\\"ratio_br_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], \\\"ratio_edge_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], \\\"progress_bar\\\": [0.0, 0.0, 0.0], \\\"bullet_zone\\\": 35.96, \\\"version\\\": \\\"v1.0\\\"}\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fg10000ccrnfmbc77u4rdfqe6pg\",\"url_list\":[\"http://v3-web.douyinvod.com/0ee915f08d4cb00c6dff5864638e6b4f/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/e328992eee624020bcb40833169d65e1/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1061\&bt=1061\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ODw3ZmgzaTdkZzo3NDg1O0Bpajl0Zzc6ZnBxZjMzNGkzM0AxMTYxXjMvNjUxYjI0Ll4yYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"http://v26-web.douyinvod.com/c98b19ccd8d8eeaf428287af3731d780/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/e328992eee624020bcb40833169d65e1/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1061\&bt=1061\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ODw3ZmgzaTdkZzo3NDg1O0Bpajl0Zzc6ZnBxZjMzNGkzM0AxMTYxXjMvNjUxYjI0Ll4yYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuHAtNAyeX-8HccpXYtVltsSpKTT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":29469023}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-dy/5bf1a938328a4d38bce39243c3395f6a",
                    "url_list": [
                        "https://p3-sign.douyinpic.com/tos-cn-i-dy/5bf1a938328a4d38bce39243c3395f6a~noop.jpeg?x-expires=1686128400&x-signature=PFSoJIoIzTZ3NzUfFFR1kDqYUVU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-sign.douyinpic.com/tos-cn-i-dy/5bf1a938328a4d38bce39243c3395f6a~noop.jpeg?x-expires=1686128400&x-signature=qJf4IJj5V4opaQB30FEf%2FcAJur8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-sign.douyinpic.com/tos-cn-i-dy/5bf1a938328a4d38bce39243c3395f6a~noop.jpeg?x-expires=1686128400&x-signature=neLsnQ%2F2CYuN8GLGZPnSIui%2BKkg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/2c592385b0844d65935e1590c1b58802_1664579721",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/2c592385b0844d65935e1590c1b58802_1664579721~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=F7Hi%2FoIoddg7ogjLzY8wbDqeVaw%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/2c592385b0844d65935e1590c1b58802_1664579721~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=urHldVdggdf5H%2Bk009uxee3WfXo%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/2c592385b0844d65935e1590c1b58802_1664579721~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=GZRET6Qviw0HzBUW%2BF99idXnoaQ%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 57609834,
                    "file_cs": "c:0-179949-ba67|a:v0200fg10000ccrnfmbc77u4rdfqe6pg",
                    "file_hash": "69a94327d4c0de52edf2ea227b01756c",
                    "height": 1440,
                    "uri": "v0200fg10000ccrnfmbc77u4rdfqe6pg",
                    "url_key": "v0200fg10000ccrnfmbc77u4rdfqe6pg_h264_1080p_2154292",
                    "url_list": [
                        "http://v3-web.douyinvod.com/7824920b174b467de4d6575fb3daef3d/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/fca21134256544d9b36f89422927968c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2103&bt=2103&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTNkOzs3PDVkZjtlMzloOEBpajl0Zzc6ZnBxZjMzNGkzM0AyMy0uX2IwNjMxLWAwLi8zYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/f82b27da1faee67377d0d42689be157d/646deef9/video/tos/cn/tos-cn-ve-15c001-alinc2/fca21134256544d9b36f89422927968c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2103&bt=2103&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTNkOzs3PDVkZjtlMzloOEBpajl0Zzc6ZnBxZjMzNGkzM0AyMy0uX2IwNjMxLWAwLi8zYSNtYmNvcjRfY29gLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000ccrnfmbc77u4rdfqe6pg&line=0&file_id=652e1630cb084c6a9239e4b8180a605f&sign=69a94327d4c0de52edf2ea227b01756c&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018006,
                    "tag_name": "政务宣传"
                },
                {
                    "level": 3,
                    "tag_id": 2018006001,
                    "tag_name": "宣教科普"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAuC2F9BdH7Enr_Fi7j83xYN8f6IgJPv64bM-5KXdpenjTruPR8caY4WCDpmA03TS1cl9czSa7MjxFE2vd4cP8pd0It-H-jr6zXn87ptghqK8RNvA8YX0adhWbr0imbClTZtk8dhxE_LoBQThCZaRFigmutIRizAM6wqRYyKa-vCs1KBA-tkVBKTYQQppO4eN8Vwx_Eql3qOLgHylEPVlgFKH5le771QlMDLDZ1Ysl9QM",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7031016280752770312",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7031016280752770312,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1637036216,
            "desc": "中美元首会晤上半场延长近半小时，现场气氛如何？一起看 #康辉Vlog ",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 56943,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7031016280752770312",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7031016280752770312
                ],
                "similar_id_list_a": [
                    7031016280752770312
                ],
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 56,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 56,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"filter_reason\":\"gov_takedown\",\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"hotsoon_review_time\":-1,\"is_subsidy_exp\":false,\"original_song_url\":\"https://sf6-sign.douyinstatic.com/ies-music/7031017045223394085.mp3?x-expires=1685008788&x-signature=BqngxETyVnWHN9V0Vt5z3%2FxrED4%3D\",\"reviewed\":1,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"original_song_uri\":\"ies-music/7031017045223394085.mp3\",\"music_label_id\":null,\"aggregate_exempt_conf\":[],\"extract_item_id\":7031016280752770312,\"is_aed_music\":0,\"with_aed_model\":1,\"dsp_switch\":0,\"has_edited\":0,\"schedule_search_time\":0,\"cover_colors\":null,\"is_red\":0,\"beats\":{}}",
                "id": 7031017062717836069,
                "id_str": "7031017062717836069",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7031017062717836069",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7031017062717836069",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7031017062717836069"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 56,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 56
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "8.28 bAt:/ 中美元首会晤上半场延长近半小时，现场气氛如何？一起看 # 康辉Vlog   %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7031016280752770312/?region=CN&mid=7031017062717836069&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7031016280752770312/?region=CN&mid=7031017062717836069&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7031016280752770312",
                "collect_count": 38452,
                "comment_count": 132739,
                "digg_count": 5424054,
                "play_count": 0,
                "share_count": 76561
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7031016280752770312",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "康辉",
                                "word_id": "6595888347086853380"
                            }
                        ]
                    },
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "康辉",
                                "word_id": "6595888347086853380"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [
                {
                    "end": 34,
                    "hashtag_id": "1649978702995459",
                    "hashtag_name": "康辉Vlog",
                    "is_commerce": false,
                    "start": 27,
                    "type": 1
                }
            ],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1965490,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 13990117,
                            "file_cs": "c:0-49077-af4b|d:0-6995057-530b,6995058-13990116-6491|a:v0200fg10000c69j0qjc77u1ai94hgug",
                            "file_hash": "df4a3151040887b9021a5f96fc812524",
                            "height": 1600,
                            "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                            "url_key": "v0200fg10000c69j0qjc77u1ai94hgug_h264_1080p_1965490",
                            "url_list": [
                                "http://v3-web.douyinvod.com/615cba55c1d770ac8e789add3e2bc336/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/22dbdc81b4124ffeacec11c69886066c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1919&bt=1919&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2g5ZmUzaTQ4aGhlMzplO0Bpamo3bDQ6ZnRtOTMzNGkzM0AtLmIuM140XjYxX2EvYGFiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "http://v26-web.douyinvod.com/cb88d632f558912b3f6e71d8ce9d1767/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/22dbdc81b4124ffeacec11c69886066c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1919&bt=1919&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2g5ZmUzaTQ4aGhlMzplO0Bpamo3bDQ6ZnRtOTMzNGkzM0AtLmIuM140XjYxX2EvYGFiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&file_id=e8dbc720dbbe4e95a17fa06b1ce61e0d&sign=df4a3151040887b9021a5f96fc812524&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1271512,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 9050464,
                            "file_cs": "c:0-48995-db3b|d:0-4525231-df63,4525232-9050463-9cee|a:v0200fg10000c69j0qjc77u1ai94hgug",
                            "file_hash": "f50bf7049378c91229b7ffdc8130d8fd",
                            "height": 1066,
                            "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                            "url_key": "v0200fg10000c69j0qjc77u1ai94hgug_h264_720p_1271512",
                            "url_list": [
                                "http://v3-web.douyinvod.com/d02a055ae99c1679d36e027ad47ecc0e/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/a85a36839c554b64a76dd5dd2d99cb42/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1241&bt=1241&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OzY7NTM0PDRmODdmaDk8M0Bpamo3bDQ6ZnRtOTMzNGkzM0A2YTA0YzQvXjMxL2EtXl4uYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "http://v26-web.douyinvod.com/51dff15ebb639df6c7c47463eaa495e0/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/a85a36839c554b64a76dd5dd2d99cb42/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1241&bt=1241&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OzY7NTM0PDRmODdmaDk8M0Bpamo3bDQ6ZnRtOTMzNGkzM0A2YTA0YzQvXjMxL2EtXl4uYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&file_id=10a9a60edc24456ca12971f07238d398&sign=f50bf7049378c91229b7ffdc8130d8fd&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1165853,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 8298398,
                            "file_cs": "c:0-48957-9dfb|d:0-4149198-2d65,4149199-8298397-428c|a:v0200fg10000c69j0qjc77u1ai94hgug",
                            "file_hash": "2f07789e13c2b6a60616e2aa24070f61",
                            "height": 854,
                            "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                            "url_key": "v0200fg10000c69j0qjc77u1ai94hgug_h264_540p_1165853",
                            "url_list": [
                                "http://v3-web.douyinvod.com/bc4de44dd6532c6775d19bf352d6dcb8/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/1fdc8f47ea4c49719dcba322703bc54e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1138&bt=1138&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs3ZWRmOmg6NjZkZDU6O0Bpamo3bDQ6ZnRtOTMzNGkzM0BfNmEyMWNhXmIxMTM2YzNiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "http://v26-web.douyinvod.com/4dda23dac19d455bee083ec2dc6e6c8e/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/1fdc8f47ea4c49719dcba322703bc54e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1138&bt=1138&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozs3ZWRmOmg6NjZkZDU6O0Bpamo3bDQ6ZnRtOTMzNGkzM0BfNmEyMWNhXmIxMTM2YzNiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&file_id=e867f29a6a4343e7aed7fc4a5bd498b8&sign=2f07789e13c2b6a60616e2aa24070f61&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 770598,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 5496098,
                            "file_cs": "c:0-37867-16a4|d:0-2748048-c016,2748049-5496097-7f7b|a:v0200fg10000c69j0qjc77u1ai94hgug",
                            "file_hash": "f86d1267d36a6379d8694a61bc6876d1",
                            "height": 854,
                            "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                            "url_key": "v0200fg10000c69j0qjc77u1ai94hgug_h264_540p_770598",
                            "url_list": [
                                "http://v3-web.douyinvod.com/b9c8a48218e296d5a9de29d7c8323d5d/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/7b5513e9c4344eb4ab3c1c19d70a52da/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=752&bt=752&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZzVmaDc0aWU1ZTllZ2QzaEBpamo3bDQ6ZnRtOTMzNGkzM0A1XmAxNGNfX2ExLy0yLS9fYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "http://v26-web.douyinvod.com/69f8d8b95cf170c6587e04f289691240/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/7b5513e9c4344eb4ab3c1c19d70a52da/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=752&bt=752&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZzVmaDc0aWU1ZTllZ2QzaEBpamo3bDQ6ZnRtOTMzNGkzM0A1XmAxNGNfX2ExLy0yLS9fYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&file_id=be200a5d0b264bd2bbbff1744ecca28d&sign=f86d1267d36a6379d8694a61bc6876d1&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/9f04ca92dcc04202b69aa479c77ffdbc_1637036223",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/9f04ca92dcc04202b69aa479c77ffdbc_1637036223~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=NR7nPBTxKVyoWzW4meaTGWDTKfY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9f04ca92dcc04202b69aa479c77ffdbc_1637036223?x-expires=2000278800&x-signature=26YpeMzRPS0rAkdyWbqVRXKd6SI%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9f04ca92dcc04202b69aa479c77ffdbc_1637036223?x-expires=2000278800&x-signature=Su1XJ96Ulpm9lJsJ1u%2FiAnyQh5c%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9f04ca92dcc04202b69aa479c77ffdbc_1637036223?x-expires=2000278800&x-signature=i%2FQOGFYqcgQCxlYSaj1Df0tr5ls%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 12277966,
                    "height": 720,
                    "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                    "url_list": [
                        "http://v3-web.douyinvod.com/535853c58d7be1f85fc982a1416caddd/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/d2fbe272b1a74d28b9c58b018f8f6df4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1599&bt=1599&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ojo6ZzQ0ZWY2Zjo1aWRlOkBpamo3bDQ6ZnRtOTMzNGkzM0AxXy4vNDUzXjQxMzY2LjAyYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                        "http://v26-web.douyinvod.com/fcf9a5206ea195b0e28fbc9f35f9aa46/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/d2fbe272b1a74d28b9c58b018f8f6df4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1599&bt=1599&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ojo6ZzQ0ZWY2Zjo1aWRlOkBpamo3bDQ6ZnRtOTMzNGkzM0AxXy4vNDUzXjQxMzY2LjAyYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuGV_9RkZXe8HccpWJhYyZ4f9aHT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 56943,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/335959f7b1184b0b89af65e81093c280_1637036222",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/335959f7b1184b0b89af65e81093c280_1637036222?x-expires=1686128400&x-signature=MG%2Bh8Ie1sO6GONSTMnTXFuRqQ2E%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/335959f7b1184b0b89af65e81093c280_1637036222?x-expires=1686128400&x-signature=kQoKCAD8Uquco%2BNu%2BjltStDpEBE%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/335959f7b1184b0b89af65e81093c280_1637036222?x-expires=1686128400&x-signature=9pAwfiwGyyxMl9UTpBPy4M0hX7U%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1600,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"loudness\":\"-10.9\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fg10000c69j0qjc77u1ai94hgug\",\"url_list\":[\"http://v3-web.douyinvod.com/70b37f969aa21e1615c322145d92aa80/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/95eca954e483411090e1f5c038772aaf/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1527\&bt=1527\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=NTc4aDo5ZzZoN2k6ZjZlN0Bpamo3bDQ6ZnRtOTMzNGkzM0AzLzUyLTExNWMxMGI1X19gYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00020000\",\"http://v26-web.douyinvod.com/b4041188bbfa9d0daacb70a9db2c8fc2/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/95eca954e483411090e1f5c038772aaf/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1527\&bt=1527\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=NTc4aDo5ZzZoN2k6ZjZlN0Bpamo3bDQ6ZnRtOTMzNGkzM0AzLzUyLTExNWMxMGI1X19gYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00020000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuGV_9RkZXe8HccpWJhYyZ4f9aHT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":11727349}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-dy/a7c4fb3b0028494691322448b7cfea1c",
                    "url_list": [
                        "https://p3-sign.douyinpic.com/tos-cn-i-dy/a7c4fb3b0028494691322448b7cfea1c~noop.jpeg?x-expires=1686128400&x-signature=HZAHU6lqCcHscLSA3yoIvhkwA0Y%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p26-sign.douyinpic.com/tos-cn-i-dy/a7c4fb3b0028494691322448b7cfea1c~noop.jpeg?x-expires=1686128400&x-signature=edrDIfr2mEkgzQv3qULUSQdF5sA%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-sign.douyinpic.com/tos-cn-i-dy/a7c4fb3b0028494691322448b7cfea1c~noop.jpeg?x-expires=1686128400&x-signature=Bgl7PrhByIEzFgkcQ7p2HsFMkCg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/d5696ab3333d45e5adb9a42a4f065774_1637036219",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/d5696ab3333d45e5adb9a42a4f065774_1637036219~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=VtXAE%2Bqw2tDuPZrHLwuZouxpkO4%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/d5696ab3333d45e5adb9a42a4f065774_1637036219~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=UeY%2BYKQFcxSNMH%2FHM%2Fyyy%2B8mqOs%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/d5696ab3333d45e5adb9a42a4f065774_1637036219~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=SJV7G9OsxrvIBPST4ltQZ2BYcqk%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 13990117,
                    "file_cs": "c:0-49077-af4b|d:0-6995057-530b,6995058-13990116-6491|a:v0200fg10000c69j0qjc77u1ai94hgug",
                    "file_hash": "df4a3151040887b9021a5f96fc812524",
                    "height": 1600,
                    "uri": "v0200fg10000c69j0qjc77u1ai94hgug",
                    "url_key": "v0200fg10000c69j0qjc77u1ai94hgug_h264_1080p_1965490",
                    "url_list": [
                        "http://v3-web.douyinvod.com/615cba55c1d770ac8e789add3e2bc336/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/22dbdc81b4124ffeacec11c69886066c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1919&bt=1919&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2g5ZmUzaTQ4aGhlMzplO0Bpamo3bDQ6ZnRtOTMzNGkzM0AtLmIuM140XjYxX2EvYGFiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                        "http://v26-web.douyinvod.com/cb88d632f558912b3f6e71d8ce9d1767/646dee5c/video/tos/cn/tos-cn-ve-15-alinc2/22dbdc81b4124ffeacec11c69886066c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1919&bt=1919&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2g5ZmUzaTQ4aGhlMzplO0Bpamo3bDQ6ZnRtOTMzNGkzM0AtLmIuM140XjYxX2EvYGFiYSNyZTZecjRnLTZgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00020000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c69j0qjc77u1ai94hgug&line=0&file_id=e8dbc720dbbe4e95a17fa06b1ce61e0d&sign=df4a3151040887b9021a5f96fc812524&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018004,
                    "tag_name": "时政新闻"
                },
                {
                    "level": 3,
                    "tag_id": 2018004001,
                    "tag_name": "外交"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAx3c0hzt7HKXn5eBjkc1csF97Lk9UDjWEDcsIGgcerfo8YEcvgMLgt6wcQWkwYsk1PnIDcbKnVUshHzOeVGtW_TwuR5YIYTdsY3wt3VgurplD-jYc-yc3S9smNDMAiKTkoJRHvBnOfpIf_24ef3vw5RVOGp-jKJPP0EriVl8sAdxL6_-M_I8xAXCoD876xG0EvmrDtq_BlkJ0ptfGH5OkcHnbwiy_piYcOR2ICS5A26Q",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7006677314532691213",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7006677314532691213,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1631369209,
            "desc": "有的视频，不需要太多描述，也可以感受到那份温暖和爱。祝福这群有爱的孩子！致敬每一位无私奉献的乡村教师！ #中国正能量",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 63940,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7006677314532691213",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7006677314532691213
                ],
                "similar_id_list_a": [
                    7006677314532691213
                ],
                "similar_id_list_b": [
                    7006677314532691213
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 63,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 63,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"with_aed_model\":1,\"douyin_beats_info\":{},\"music_label_id\":null,\"extract_item_id\":7006677314532691213,\"is_subsidy_exp\":false,\"dsp_switch\":0,\"has_edited\":0,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"filter_reason\":\"gov_takedown\",\"cover_colors\":null,\"is_red\":0,\"aggregate_exempt_conf\":[],\"schedule_search_time\":0,\"hotsoon_review_time\":-1,\"original_song_url\":\"https://sf3-sign.douyinstatic.com/ies-music/7006677456959195918.mp3?x-expires=1685008788&x-signature=XXzWdevspJvqICQ4SHS7uZmXHOo%3D\",\"original_song_uri\":\"ies-music/7006677456959195918.mp3\",\"is_aed_music\":0,\"reviewed\":1,\"review_unshelve_reason\":0,\"beats\":{}}",
                "id": 7006677436134607624,
                "id_str": "7006677436134607624",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7006677436134607624",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7006677436134607624",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7006677436134607624"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 63,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 63
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "3.89 Wzt:/ 有的视频，不需要太多描述，也可以感受到那份温暖和爱。祝福这群有爱的孩子！致敬每一位无私奉献的乡村教师！ # 中国正能量  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7006677314532691213/?region=CN&mid=7006677436134607624&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7006677314532691213/?region=CN&mid=7006677436134607624&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7006677314532691213",
                "collect_count": 77376,
                "comment_count": 546782,
                "digg_count": 9834637,
                "play_count": 0,
                "share_count": 468857
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7006677314532691213",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "大家都在搜：",
                        "icon_url": "",
                        "scene": "comment_top_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "张鹏程校长",
                                "word_id": "6653086406610523395"
                            }
                        ]
                    },
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "张鹏程校长",
                                "word_id": "6653086406610523395"
                            }
                        ]
                    },
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "张鹏程校长",
                                "word_id": "6653086406610523395"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [
                {
                    "end": 58,
                    "hashtag_id": "1608959134995463",
                    "hashtag_name": "中国正能量",
                    "is_commerce": false,
                    "start": 52,
                    "type": 1
                }
            ],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [
                    {
                        "duration": 63.88,
                        "fext": "jpg",
                        "img_num": 64,
                        "img_url": "http://p3-sign.douyinpic.com/tos-cn-p-0015/d4c3bc9a1e554ee1b4a0fa57a7b4d84c_1631369219~tplv-noop.image?x-expires=1684926051&x-signature=%2FN5Gh3SgUGBrYvQB1VIkSJ3UzNc%3D",
                        "img_x_len": 10,
                        "img_x_size": 162,
                        "img_y_len": 7,
                        "img_y_size": 240,
                        "interval": 1,
                        "uri": "tos-cn-p-0015/d4c3bc9a1e554ee1b4a0fa57a7b4d84c_1631369219"
                    }
                ],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1412813,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 11291910,
                            "file_cs": "c:0-54941-3c3e|a:v0200fg10000c4ubdebc77ufn11jb6b0",
                            "file_hash": "b38ac80b41196522b2fb9f466e0dd6f7",
                            "height": 1600,
                            "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                            "url_key": "v0200fg10000c4ubdebc77ufn11jb6b0_h264_1080p_1412813",
                            "url_list": [
                                "http://v3-web.douyinvod.com/feb514de676bbdcbfd3403c3fbd0bcc8/646dee63/video/tos/cn/tos-cn-ve-15/030a99e0ccdd484ab373181b6ff6d3e3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1379&bt=1379&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk3NmVmaWRnPDM7ZGRmZkBpMzltNGk6ZmhlNzMzNGkzM0BeLy0uMy1fXmIxMF82LjZeYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/97d9311165977788f97dd13a8245c6cf/646dee63/video/tos/cn/tos-cn-ve-15/030a99e0ccdd484ab373181b6ff6d3e3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1379&bt=1379&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk3NmVmaWRnPDM7ZGRmZkBpMzltNGk6ZmhlNzMzNGkzM0BeLy0uMy1fXmIxMF82LjZeYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&file_id=ac9c1a9ab83049edaabf0c6b130426a8&sign=b38ac80b41196522b2fb9f466e0dd6f7&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 910669,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 7278529,
                            "file_cs": "c:0-54935-206f|a:v0200fg10000c4ubdebc77ufn11jb6b0",
                            "file_hash": "1f6b9f513f577b8cf3a3bb61ac82ab3d",
                            "height": 1066,
                            "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                            "url_key": "v0200fg10000c4ubdebc77ufn11jb6b0_h264_720p_910669",
                            "url_list": [
                                "http://v3-web.douyinvod.com/9fd0f394140f83d95cb22f7bda41e617/646dee63/video/tos/cn/tos-cn-ve-15/2f15a90066fe4163985f2f19926b5dc9/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=889&bt=889&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ojs2Mzc6ZmY5NjRnNWhnM0BpMzltNGk6ZmhlNzMzNGkzM0BgLjNjYDI0XjUxLmMtMWExYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/d352219ab815a115619a78c6332b127e/646dee63/video/tos/cn/tos-cn-ve-15/2f15a90066fe4163985f2f19926b5dc9/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=889&bt=889&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ojs2Mzc6ZmY5NjRnNWhnM0BpMzltNGk6ZmhlNzMzNGkzM0BgLjNjYDI0XjUxLmMtMWExYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&file_id=40dd4e02fd114386ac7c57c4f06318c7&sign=1f6b9f513f577b8cf3a3bb61ac82ab3d&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 834619,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 6670694,
                            "file_cs": "c:0-54933-aa25|a:v0200fg10000c4ubdebc77ufn11jb6b0",
                            "file_hash": "f6764fc754f192b13298aace74f01184",
                            "height": 854,
                            "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                            "url_key": "v0200fg10000c4ubdebc77ufn11jb6b0_h264_540p_834619",
                            "url_list": [
                                "http://v3-web.douyinvod.com/5be0b2cba960346748705d9acb199836/646dee63/video/tos/cn/tos-cn-ve-15/1f554e3168d34b04857c34c7ee07a580/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=815&bt=815&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGhmMzg0ZDY5Zzg1M2g7OkBpMzltNGk6ZmhlNzMzNGkzM0BeLTY0M2JeXjMxMS4zNWI1YSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/e7a3a4a0c95a0bc8c175d8195b832703/646dee63/video/tos/cn/tos-cn-ve-15/1f554e3168d34b04857c34c7ee07a580/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=815&bt=815&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGhmMzg0ZDY5Zzg1M2g7OkBpMzltNGk6ZmhlNzMzNGkzM0BeLTY0M2JeXjMxMS4zNWI1YSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&file_id=87e88e6012454d66a3aae165709c0eaa&sign=f6764fc754f192b13298aace74f01184&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 565135,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4524969,
                            "file_cs": "c:0-42367-9877|a:v0200fg10000c4ubdebc77ufn11jb6b0",
                            "file_hash": "28d42a12cee0e9803a8478e67de62db0",
                            "height": 854,
                            "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                            "url_key": "v0200fg10000c4ubdebc77ufn11jb6b0_h264_540p_565135",
                            "url_list": [
                                "http://v3-web.douyinvod.com/4751ff70feddaa43e6ba3ee49fe23d3c/646dee63/video/tos/cn/tos-cn-ve-15/2e89d44eb5a546e98c460096694642ba/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=551&bt=551&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=Zzg1OGdnOzQ1M2U2aTVmN0BpMzltNGk6ZmhlNzMzNGkzM0BiNDUvLl82NjUxYjQwYzE0YSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "http://v26-web.douyinvod.com/c82c5a3169d17f98ba887f11d0cbfe5e/646dee63/video/tos/cn/tos-cn-ve-15/2e89d44eb5a546e98c460096694642ba/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=551&bt=551&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=Zzg1OGdnOzQ1M2U2aTVmN0BpMzltNGk6ZmhlNzMzNGkzM0BiNDUvLl82NjUxYjQwYzE0YSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&file_id=744cf23f73eb40829198bd1d258275ed&sign=28d42a12cee0e9803a8478e67de62db0&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/a56195c4e12b4e26b6774519d2e8b5f5_1631369215",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/a56195c4e12b4e26b6774519d2e8b5f5_1631369215~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=DPCN1gvvUWrPG6anxTEZeblsOh8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/a56195c4e12b4e26b6774519d2e8b5f5_1631369215?x-expires=2000278800&x-signature=0T3lfWlZt4Sc8lAlwLbD47u6p%2B0%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/a56195c4e12b4e26b6774519d2e8b5f5_1631369215?x-expires=2000278800&x-signature=y4yGBBNpZ6Dy%2Fbe3TINwlCg80aE%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/a56195c4e12b4e26b6774519d2e8b5f5_1631369215?x-expires=2000278800&x-signature=bShGvUK%2BKcvBGcO1fVcToxyP8ho%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 9974953,
                    "height": 720,
                    "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                    "url_list": [
                        "http://v3-web.douyinvod.com/61b293dd64229c779d3450475bf3bdd2/646dee63/video/tos/cn/tos-cn-ve-15/a28d56bd03174ae5a1e96675f1ee1df9/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1163&bt=1163&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODc2OjZnOzNkMzk4aTQ0aUBpMzltNGk6ZmhlNzMzNGkzM0AuYTE1My0zXjUxNS5eNDZgYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/94d04a50f1722e50f8bb9239909a25b6/646dee63/video/tos/cn/tos-cn-ve-15/a28d56bd03174ae5a1e96675f1ee1df9/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1163&bt=1163&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODc2OjZnOzNkMzk4aTQ0aUBpMzltNGk6ZmhlNzMzNGkzM0AuYTE1My0zXjUxNS5eNDZgYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&ratio=720p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuGXs9wwcX-8HccpD5cAwcAVpLaE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 63940,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/78c61e45c8fd4821b75c122bf13867be_1631369214",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/78c61e45c8fd4821b75c122bf13867be_1631369214?x-expires=1686128400&x-signature=z7u6%2BB%2FTspzBZNorB0mDH78IZzU%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/78c61e45c8fd4821b75c122bf13867be_1631369214?x-expires=1686128400&x-signature=fQEyg%2BUro%2F8K6R1yWO%2BHO2CT3Eo%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/78c61e45c8fd4821b75c122bf13867be_1631369214?x-expires=1686128400&x-signature=Oo9mjJwZO6HMHtNQDayd780ikEU%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1600,
                "is_h265": 0,
                "is_long_video": 1,
                "is_source_HDR": 0,
                "meta": "{\"loudness\":\"-22.4\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fg10000c4ubdebc77ufn11jb6b0\",\"url_list\":[\"http://v3-web.douyinvod.com/23ade356ef23096bff865945dd92aac3/646dee63/video/tos/cn/tos-cn-ve-15-alinc2/3edeb9aaaff446fda180db73a49c684a/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1094\&bt=1094\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=aGc6ODkzPDw5MzY7OzRkZkBpMzltNGk6ZmhlNzMzNGkzM0AtNGIuMWIxNjIxLi1iYmBiYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"http://v26-web.douyinvod.com/d8644943569f54c29f645f493e8aa35b/646dee63/video/tos/cn/tos-cn-ve-15-alinc2/3edeb9aaaff446fda180db73a49c684a/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1094\&bt=1094\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=aGc6ODkzPDw5MzY7OzRkZkBpMzltNGk6ZmhlNzMzNGkzM0AtNGIuMWIxNjIxLi1iYmBiYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00028000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0\&line=0\&ratio=720p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESRKvePEcuGXs9wwcX-8HccpD5cAwcAVpLaE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":9384829}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-0813/cd701d5588ca40fa8045e4686e3b24f0",
                    "url_list": [
                        "https://p26-sign.douyinpic.com/tos-cn-i-0813/cd701d5588ca40fa8045e4686e3b24f0~noop.jpeg?x-expires=1686128400&x-signature=rIZSCLWhCniQJNfY2v35cUmXC5E%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-0813/cd701d5588ca40fa8045e4686e3b24f0~noop.jpeg?x-expires=1686128400&x-signature=9B%2BYG%2FeXtBbahl%2BOhQgblZDZ1f8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-sign.douyinpic.com/tos-cn-i-0813/cd701d5588ca40fa8045e4686e3b24f0~noop.jpeg?x-expires=1686128400&x-signature=Pe017UJL3YqBqtUUWqYUNZynd1s%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/0346409ecefd4dd3a64f20ff5eb4b186_1631369215",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/0346409ecefd4dd3a64f20ff5eb4b186_1631369215~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=TXzKRRkjmZWK6cCvaM%2BWev1Zr5g%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/0346409ecefd4dd3a64f20ff5eb4b186_1631369215~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=3b7nlXSenBaMhkLgJ9xNDnKPhA8%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/0346409ecefd4dd3a64f20ff5eb4b186_1631369215~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=jtxmbE%2BhK0gvMSg92Ukx1yq2%2Bgc%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 11291910,
                    "file_cs": "c:0-54941-3c3e|a:v0200fg10000c4ubdebc77ufn11jb6b0",
                    "file_hash": "b38ac80b41196522b2fb9f466e0dd6f7",
                    "height": 1600,
                    "uri": "v0200fg10000c4ubdebc77ufn11jb6b0",
                    "url_key": "v0200fg10000c4ubdebc77ufn11jb6b0_h264_1080p_1412813",
                    "url_list": [
                        "http://v3-web.douyinvod.com/feb514de676bbdcbfd3403c3fbd0bcc8/646dee63/video/tos/cn/tos-cn-ve-15/030a99e0ccdd484ab373181b6ff6d3e3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1379&bt=1379&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk3NmVmaWRnPDM7ZGRmZkBpMzltNGk6ZmhlNzMzNGkzM0BeLy0uMy1fXmIxMF82LjZeYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "http://v26-web.douyinvod.com/97d9311165977788f97dd13a8245c6cf/646dee63/video/tos/cn/tos-cn-ve-15/030a99e0ccdd484ab373181b6ff6d3e3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1379&bt=1379&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk3NmVmaWRnPDM7ZGRmZkBpMzltNGk6ZmhlNzMzNGkzM0BeLy0uMy1fXmIxMF82LjZeYSNfXy5rcjRfYXJgLS1kLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00028000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fg10000c4ubdebc77ufn11jb6b0&line=0&file_id=ac9c1a9ab83049edaabf0c6b130426a8&sign=b38ac80b41196522b2fb9f466e0dd6f7&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2007,
                    "tag_name": "校园教育"
                },
                {
                    "level": 2,
                    "tag_id": 2007006,
                    "tag_name": "中小学校园"
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAXhhbjZsV_S68u0ZPi6JHBz7mAbwCmVwKSTweO0YPVpTGUpXo8B43kzCTVJxz603N-E17a2Fo7bSYwt-0IFh5VpArM8RLuPaLdGb9HIq8wxxF3l2GmIcuopEhmWdc4v-1XkTXJr7KPphC3mE6XBuUSNmlJk9zT_Yygkl5VHJ2BMf3mY0WBJlwh3lPih2HdHibdyP0pD1treJAyeFpDlDYXh5pB-U5LL8NDnRN6mLKwUw",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7003955808660622623",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7003955808660622623,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1630735575,
            "desc": "太甜了！八年的等待，退伍军人在重庆机场求婚。“我会像守护祖国一样守护你一人”，感动！祝福！ #中国正能量",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 20847,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7003955808660622623",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7003955808660622623
                ],
                "similar_id_list_a": [
                    7003955808660622623
                ],
                "similar_id_list_b": [
                    7003955808660622623
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 20,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 20,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"has_edited\":0,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_subsidy_exp\":false,\"with_aed_model\":1,\"douyin_beats_info\":{},\"original_song_uri\":\"ies-music/7003955978265840392.mp3\",\"aggregate_exempt_conf\":[],\"extract_item_id\":7003955808660622623,\"filter_reason\":\"gov_takedown\",\"hotsoon_review_time\":-1,\"cover_colors\":null,\"original_song_url\":\"https://sf9-sign.douyinstatic.com/ies-music/7003955978265840392.mp3?x-expires=1685008788&x-signature=k8FseEFbVoBZtr9Tf%2B9XuuFtcAI%3D\",\"is_aed_music\":0,\"dsp_switch\":0,\"reviewed\":1,\"review_unshelve_reason\":0,\"beats\":{},\"schedule_search_time\":0,\"is_red\":0,\"music_label_id\":null}",
                "id": 7003955984049703717,
                "id_str": "7003955984049703717",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7003955984049703717",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7003955984049703717",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7003955984049703717"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 20,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 20
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "6.17 wsE:/ 太甜了！八年的等待，退伍军人在重庆机场求婚。“我会像守护祖国一样守护你一人”，感动！祝福！ # 中国正能量  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7003955808660622623/?region=CN&mid=7003955984049703717&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7003955808660622623/?region=CN&mid=7003955984049703717&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7003955808660622623",
                "collect_count": 77741,
                "comment_count": 531188,
                "digg_count": 12839648,
                "play_count": 0,
                "share_count": 848781
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7003955808660622623",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "退伍季",
                                "word_id": "6548204229155099912"
                            }
                        ]
                    },
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "退伍军人在机场求婚",
                                "word_id": "6871588961057166596"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [
                {
                    "end": 52,
                    "hashtag_id": "1608959134995463",
                    "hashtag_name": "中国正能量",
                    "is_commerce": false,
                    "start": 46,
                    "type": 1
                }
            ],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2124702,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 5536710,
                            "file_cs": "c:0-18559-051a|d:0-2768354-33ce,2768355-5536709-b8d0|a:v0300fg10000c4pgorbc77u2pejn1750",
                            "file_hash": "84143c774f461237fde03abc70a743dd",
                            "height": 1066,
                            "uri": "v0300fg10000c4pgorbc77u2pejn1750",
                            "url_key": "v0300fg10000c4pgorbc77u2pejn1750_h264_720p_2124702",
                            "url_list": [
                                "http://v3-web.douyinvod.com/751cd75e58064a1171b9d711dd792125/646dee38/video/tos/cn/tos-cn-ve-15/8b19947d3ed14ab592ca72aade832bc3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2074&bt=2074&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWRpNzYzN2kzN2U5OjlnaEBpMzpxaDU6ZnVqNzMzNGkzM0A2YV82YTAtNjMxMzFiXjNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/0d0bc6524c0429e7e4632f0ba7f0f2ae/646dee38/video/tos/cn/tos-cn-ve-15/8b19947d3ed14ab592ca72aade832bc3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2074&bt=2074&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWRpNzYzN2kzN2U5OjlnaEBpMzpxaDU6ZnVqNzMzNGkzM0A2YV82YTAtNjMxMzFiXjNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750&line=0&file_id=fe6da6e7466b44609f0430d394bfda96&sign=84143c774f461237fde03abc70a743dd&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1923798,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 5013178,
                            "file_cs": "c:0-18477-0165|d:0-2506588-1610,2506589-5013177-785f|a:v0300fg10000c4pgorbc77u2pejn1750",
                            "file_hash": "5e692d6cc56031fca3ce728d06ad5167",
                            "height": 854,
                            "uri": "v0300fg10000c4pgorbc77u2pejn1750",
                            "url_key": "v0300fg10000c4pgorbc77u2pejn1750_h264_540p_1923798",
                            "url_list": [
                                "http://v3-web.douyinvod.com/3f491f7068f074e878a1b2b97b283c60/646dee38/video/tos/cn/tos-cn-ve-15/337b6cac414c48b1b2f2fa72b2716ff0/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1878&bt=1878&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDY0NDM8aTRnNjg3OTxmO0BpMzpxaDU6ZnVqNzMzNGkzM0AyMGE0Ly1hNjExMGFfYGNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/05735823b044fe1e07789d7b1b989d55/646dee38/video/tos/cn/tos-cn-ve-15/337b6cac414c48b1b2f2fa72b2716ff0/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1878&bt=1878&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDY0NDM8aTRnNjg3OTxmO0BpMzpxaDU6ZnVqNzMzNGkzM0AyMGE0Ly1hNjExMGFfYGNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750&line=0&file_id=f8fcc9b6d435434d91df092071d13351&sign=5e692d6cc56031fca3ce728d06ad5167&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1308902,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3429651,
                            "file_cs": "c:0-14651-d806|d:0-1714824-e5aa,1714825-3429650-f8df|a:v0300fg10000c4pgorbc77u2pejn1750",
                            "file_hash": "c8ec34e87598fcc3bee4581e36572b5f",
                            "height": 854,
                            "uri": "v0300fg10000c4pgorbc77u2pejn1750",
                            "url_key": "v0300fg10000c4pgorbc77u2pejn1750_h264_540p_1308902",
                            "url_list": [
                                "http://v3-web.douyinvod.com/a9dce48984a89d41aac491159b992b90/646dee38/video/tos/cn/tos-cn-ve-15/66ae46201dfc433e9fc613d83ce71c6c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1278&bt=1278&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZTc8O2k2ZDozaGY6Nzw4M0BpMzpxaDU6ZnVqNzMzNGkzM0BhLjIvXjMxXjMxXl81MTBeYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/2d1ba0c6987110beea4c1de634ad1e50/646dee38/video/tos/cn/tos-cn-ve-15/66ae46201dfc433e9fc613d83ce71c6c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1278&bt=1278&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZTc8O2k2ZDozaGY6Nzw4M0BpMzpxaDU6ZnVqNzMzNGkzM0BhLjIvXjMxXjMxXl81MTBeYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750&line=0&file_id=a0354984b7ac4e60a74a63af285914db&sign=c8ec34e87598fcc3bee4581e36572b5f&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/d4b452d1511643be8dbc0235a8ee1755_1630735577",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/d4b452d1511643be8dbc0235a8ee1755_1630735577~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=cLcy%2BSEQ0BXmOd6%2BFiS8CN%2FueXg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/d4b452d1511643be8dbc0235a8ee1755_1630735577?x-expires=2000278800&x-signature=EHzkuRqILVExEtzW38bhs%2BU2jM8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/d4b452d1511643be8dbc0235a8ee1755_1630735577?x-expires=2000278800&x-signature=RAIi9zNHudJmUXDxnWj1aBr1iXM%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/d4b452d1511643be8dbc0235a8ee1755_1630735577?x-expires=2000278800&x-signature=hgYYpCvPVACIV5OK9qkUOitx5qo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 7112977,
                    "height": 720,
                    "uri": "v0300fg10000c4pgorbc77u2pejn1750",
                    "url_list": [
                        "http://v3-web.douyinvod.com/558cbd596f17502dcd794d87ae823ebd/646dee38/video/tos/cn/tos-cn-ve-15/a44eb44bd54249fb924cb648532cf88a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2328&bt=2328&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Zzs3NWVoZ2k7ZDo3ODZlZEBpMzpxaDU6ZnVqNzMzNGkzM0AvLTBfMzJgXmIxX14uYTIxYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/4de2826815049e2716f89c15fc43a516/646dee38/video/tos/cn/tos-cn-ve-15/a44eb44bd54249fb924cb648532cf88a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2328&bt=2328&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Zzs3NWVoZ2k7ZDo3ODZlZEBpMzpxaDU6ZnVqNzMzNGkzM0AvLTBfMzJgXmIxX14uYTIxYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGXttk7Zn-8HccpW4lUmsRGpeGE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 20847,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/6fb92f0627764c84a7319a8ecda63b76_1630735579",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/6fb92f0627764c84a7319a8ecda63b76_1630735579?x-expires=1686128400&x-signature=3UE2jtRagGnRBmFJvXJurCXwHFA%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/6fb92f0627764c84a7319a8ecda63b76_1630735579?x-expires=1686128400&x-signature=9HthOjdkZecgDbcxJBA%2BZqN8YGc%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/6fb92f0627764c84a7319a8ecda63b76_1630735579?x-expires=1686128400&x-signature=K1HhGtvfmSOZm3%2F6yKeC8vsJp80%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1600,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"loudness\":\"-8.6\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0300fg10000c4pgorbc77u2pejn1750\",\"url_list\":[\"http://v3-web.douyinvod.com/9e3690e5a05f047f17c1974a472ce00b/646dee38/video/tos/cn/tos-cn-ve-15/7b2f4d33f97641b69c3b34fc1b16cf86/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=2296\&bt=2296\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=M2dlZTRpaTs4OjY2ZjVnZkBpMzpxaDU6ZnVqNzMzNGkzM0AuMDI0NjA2NV8xXzQzLy8yYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"http://v26-web.douyinvod.com/a504ba3ef8bde016a23ac549f1d17489/646dee38/video/tos/cn/tos-cn-ve-15/7b2f4d33f97641b69c3b34fc1b16cf86/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=2296\&bt=2296\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=M2dlZTRpaTs4OjY2ZjVnZkBpMzpxaDU6ZnVqNzMzNGkzM0AuMDI0NjA2NV8xXzQzLy8yYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGXttk7Zn-8HccpW4lUmsRGpeGE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":7015309}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-0813/aa7f4ffd413041dc8528ac327750b180",
                    "url_list": [
                        "https://p3-sign.douyinpic.com/tos-cn-i-0813/aa7f4ffd413041dc8528ac327750b180~noop.jpeg?x-expires=1686128400&x-signature=wEWKMuMrZTEGJIwlJnjj%2FnYu1t8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p26-sign.douyinpic.com/tos-cn-i-0813/aa7f4ffd413041dc8528ac327750b180~noop.jpeg?x-expires=1686128400&x-signature=9LlUrKqtQsewPSLRf0vgsw7ChBs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-sign.douyinpic.com/tos-cn-i-0813/aa7f4ffd413041dc8528ac327750b180~noop.jpeg?x-expires=1686128400&x-signature=mq9vAuiuk1OZCOozVoi5%2FEZ%2FgcY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/5dc90027deef42d1831eb60a0ce2519c_1630735577",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/5dc90027deef42d1831eb60a0ce2519c_1630735577~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=ggKThwCkIxwCdr4RPgXePD3lc0g%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/5dc90027deef42d1831eb60a0ce2519c_1630735577~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=C1x%2BGzhyDwc7WUX6mYHLXw1CtIo%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/5dc90027deef42d1831eb60a0ce2519c_1630735577~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=YaHSZAw%2FN%2B%2BkNPVqMIPZYPc72JM%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 5536710,
                    "file_cs": "c:0-18559-051a|d:0-2768354-33ce,2768355-5536709-b8d0|a:v0300fg10000c4pgorbc77u2pejn1750",
                    "file_hash": "84143c774f461237fde03abc70a743dd",
                    "height": 1066,
                    "uri": "v0300fg10000c4pgorbc77u2pejn1750",
                    "url_key": "v0300fg10000c4pgorbc77u2pejn1750_h264_720p_2124702",
                    "url_list": [
                        "http://v3-web.douyinvod.com/751cd75e58064a1171b9d711dd792125/646dee38/video/tos/cn/tos-cn-ve-15/8b19947d3ed14ab592ca72aade832bc3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2074&bt=2074&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWRpNzYzN2kzN2U5OjlnaEBpMzpxaDU6ZnVqNzMzNGkzM0A2YV82YTAtNjMxMzFiXjNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/0d0bc6524c0429e7e4632f0ba7f0f2ae/646dee38/video/tos/cn/tos-cn-ve-15/8b19947d3ed14ab592ca72aade832bc3/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2074&bt=2074&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OWRpNzYzN2kzN2U5OjlnaEBpMzpxaDU6ZnVqNzMzNGkzM0A2YV82YTAtNjMxMzFiXjNjYSMyLmdtcjRfbG1gLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c4pgorbc77u2pejn1750&line=0&file_id=fe6da6e7466b44609f0430d394bfda96&sign=84143c774f461237fde03abc70a743dd&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2029,
                    "tag_name": "随拍"
                },
                {
                    "level": 2,
                    "tag_id": 2029003,
                    "tag_name": "生活记录"
                },
                {
                    "level": 3,
                    "tag_id": 2029003001,
                    "tag_name": "日常vlog"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAfijLF0iVvZZlfd8ezgs0_DhjokBBPVT0UlRAsypE-p3DyaQa3bHsOrdIpWqkAeEVpryqNIJSe1eiT6u67q7Mlu4sT8GaIhQP7__b7hSOrFw_RsO_22TvX5HMYopsRKzFOa2VCEmIHqbhgzaMnpjfjfm2P_pqYCtWuRLyn_uIxIYiWbWv4PZ6p9B24VgNyWRUxojqCB6Mp7gIQqwJB8hYFFCC5d42xAhSchZPgCtqKAE",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6979747605198753060",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6979747605198753060,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1625099137,
            "desc": "100响礼炮，声声震寰宇；国旗护卫队，步步坚定有力！百年大党，生日快乐！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 19887,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6979747605198753060",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6963625205512047885,
                    6838346382219283719,
                    6979744533349190946,
                    6850958255217282319
                ],
                "similar_id_list_a": [
                    6979747605198753060
                ],
                "similar_id_list_b": [
                    6979747605198753060
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 19,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 19,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"has_edited\":0,\"music_tagging\":{\"Languages\":[\"non_vocal\"],\"Moods\":[\"Inspirational\"],\"Genres\":[\"BGM\",\"Others\"],\"Themes\":[\"Sport\",\"Game\"],\"AEDs\":[\"non_vocal\"],\"SingingVersions\":null,\"Instruments\":null},\"is_red\":0,\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/6979747644738767623.mp3?x-expires=1685008788&x-signature=dpMHxotHG8afWVMiOkIbW5GbusM%3D\",\"music_label_id\":null,\"filter_reason\":\"gov_takedown\",\"reviewed\":1,\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"schedule_search_time\":0,\"aggregate_exempt_conf\":[],\"extract_item_id\":6979747605198753060,\"activities\":[10006],\"dsp_switch\":0,\"hotsoon_review_time\":-1,\"with_aed_model\":1,\"beats\":{\"audio_effect_onset\":\"https://sf6-sign.douyinstatic.com/ies-music/strong_beat/v3/1708082603231310?x-expires=1685008788&x-signature=Cg4m7mo1nH1InMTEreDV2g7V9oY%3D\",\"beats_tracker\":\"https://sf26-sign.douyinstatic.com/ies-music/strong_beat/v3/1708082604184589?x-expires=1685008788&x-signature=X9xtcZktIhmlkcXIZTwnwtoP09k%3D\",\"energy_trace\":\"https://sf9-sign.douyinstatic.com/ies-music/strong_beat/v3/1708082603124749?x-expires=1685008788&x-signature=qtdeUBBKvv1M9A%2BmpH8XD0Fgy4c%3D\",\"merged_beats\":\"https://sf3-sign.douyinstatic.com/ies-music/strong_beat/v3/1708082604460039?x-expires=1685008788&x-signature=JiSSXdb0oJEl6Rbafjo8Iesd59w%3D\"},\"cover_colors\":null,\"is_subsidy_exp\":false,\"original_song_uri\":\"ies-music/6979747644738767623.mp3\",\"is_aed_music\":1}",
                "id": 6979747653114612488,
                "id_str": "6979747653114612488",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6979747653114612488",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6979747653114612488",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6979747653114612488"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 19,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf6-sign.douyinstatic.com/ies-music/pattern/f9bce64d1759a5408a11948e79783d51.json?x-expires=1685008788&x-signature=mmg1wIpcIRWpeKEUzrH%2FSoriog0%3D",
                    "url_list": [
                        "https://sf6-sign.douyinstatic.com/ies-music/pattern/f9bce64d1759a5408a11948e79783d51.json?x-expires=1685008788&x-signature=mmg1wIpcIRWpeKEUzrH%2FSoriog0%3D",
                        "https://sf3-sign.douyinstatic.com/ies-music/pattern/f9bce64d1759a5408a11948e79783d51.json?x-expires=1685008788&x-signature=tPb9F32yrtARtbrfFmBmRTBH6GQ%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 19
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "7.46 Mjc:/ 100响礼炮，声声震寰宇；国旗护卫队，步步坚定有力！百年大党，生日快乐！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6979747605198753060/?region=CN&mid=6979747653114612488&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6979747605198753060/?region=CN&mid=6979747653114612488&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6979747605198753060",
                "collect_count": 34354,
                "comment_count": 427360,
                "digg_count": 13799914,
                "play_count": 0,
                "share_count": 288358
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6979747605198753060",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "央视新闻",
                                "word_id": "6527565534144238862"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1300161,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3232039,
                            "file_cs": "c:0-17740-9e56|d:0-1616018-e1f5,1616019-3232038-b9ff|a:v0300fg10000c3egmrrc77ufino0e1t0",
                            "file_hash": "59cd55ab6efa04a1682a73826c6f2f83",
                            "height": 1246,
                            "uri": "v0300fg10000c3egmrrc77ufino0e1t0",
                            "url_key": "v0300fg10000c3egmrrc77ufino0e1t0_h264_720p_1300161",
                            "url_list": [
                                "http://v3-web.douyinvod.com/6b073a1d777d8ad2eb1f8da16bf04a85/646dee37/video/tos/cn/tos-cn-ve-15/abc33b2db92745b9beef1b5883ca5c76/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1269&bt=1269&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk0Ojg4ZDU5NWdnaWY0NEBpMzQzcWk6ZnVqNjMzNGkzM0A1Ly9fLl8zXl4xNGMxX14xYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/3cef7fe1f845b275f9d3a641588dcaba/646dee37/video/tos/cn/tos-cn-ve-15/abc33b2db92745b9beef1b5883ca5c76/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1269&bt=1269&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk0Ojg4ZDU5NWdnaWY0NEBpMzQzcWk6ZnVqNjMzNGkzM0A1Ly9fLl8zXl4xNGMxX14xYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0&line=0&file_id=41a1bc4ffd7d42a6a26ab515b7212688&sign=59cd55ab6efa04a1682a73826c6f2f83&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1201226,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2986098,
                            "file_cs": "c:0-17757-838c|d:0-1493048-df6d,1493049-2986097-d456|a:v0300fg10000c3egmrrc77ufino0e1t0",
                            "file_hash": "d478287f76baefbcc6d9155b878ccfc6",
                            "height": 998,
                            "uri": "v0300fg10000c3egmrrc77ufino0e1t0",
                            "url_key": "v0300fg10000c3egmrrc77ufino0e1t0_h264_540p_1201226",
                            "url_list": [
                                "http://v3-web.douyinvod.com/ae299be20ffa0e19c77e02529b941518/646dee37/video/tos/cn/tos-cn-ve-15/1b7e188e25f84eebaff6b3b2f81a58b6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1173&bt=1173&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OGg7aWY8NzNoZjxmZ2Q5PEBpMzQzcWk6ZnVqNjMzNGkzM0AxMV5gXjQ2NWIxMDVfY2IxYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/7d21fd910a739b9af66721d1d2253164/646dee37/video/tos/cn/tos-cn-ve-15/1b7e188e25f84eebaff6b3b2f81a58b6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1173&bt=1173&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OGg7aWY8NzNoZjxmZ2Q5PEBpMzQzcWk6ZnVqNjMzNGkzM0AxMV5gXjQ2NWIxMDVfY2IxYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0&line=0&file_id=49e6fabd8c394cee809479accfa84e45&sign=d478287f76baefbcc6d9155b878ccfc6&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 818384,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2046165,
                            "file_cs": "c:0-13883-028d|d:0-1023081-c245,1023082-2046164-39b4|a:v0300fg10000c3egmrrc77ufino0e1t0",
                            "file_hash": "0b6ae0a9ee5e592305b5a5819eb2c9cb",
                            "height": 998,
                            "uri": "v0300fg10000c3egmrrc77ufino0e1t0",
                            "url_key": "v0300fg10000c3egmrrc77ufino0e1t0_h264_540p_818384",
                            "url_list": [
                                "http://v3-web.douyinvod.com/78b5ce761e5f66ed92c7afc922e2df8b/646dee37/video/tos/cn/tos-cn-ve-15/23b65af819c24a50bbb8483e40a2196c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=799&bt=799&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZWdmZjdoNzM0O2YzZzo7ZUBpMzQzcWk6ZnVqNjMzNGkzM0AyYGJfYV8uXy8xLmAtMS8vYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/f1606ac83875d9ac3be19523768a7a5e/646dee37/video/tos/cn/tos-cn-ve-15/23b65af819c24a50bbb8483e40a2196c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=799&bt=799&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=ZWdmZjdoNzM0O2YzZzo7ZUBpMzQzcWk6ZnVqNjMzNGkzM0AyYGJfYV8uXy8xLmAtMS8vYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0&line=0&file_id=2b28470dc01c4821b014bed4bceccd5b&sign=0b6ae0a9ee5e592305b5a5819eb2c9cb&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/dfe084289fdf405284fb5f8e2e30ff78_1625099140",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/dfe084289fdf405284fb5f8e2e30ff78_1625099140~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=VT%2By8ODvfsPRYA2KkRzBpQWErUo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/dfe084289fdf405284fb5f8e2e30ff78_1625099140?x-expires=2000278800&x-signature=UjGqcs2v6WlFcgJ0dkrojI%2Fb%2FG4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/dfe084289fdf405284fb5f8e2e30ff78_1625099140?x-expires=2000278800&x-signature=aSvTQDIIHqCGkiRPp0hymXMBxqU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/dfe084289fdf405284fb5f8e2e30ff78_1625099140?x-expires=2000278800&x-signature=eEWe%2BL3Yq9%2B90UUP5RwroOuw6eg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 4286433,
                    "height": 720,
                    "uri": "v0300fg10000c3egmrrc77ufino0e1t0",
                    "url_list": [
                        "http://v3-web.douyinvod.com/d8c30750d8d68154528d162eed37fce8/646dee37/video/tos/cn/tos-cn-ve-15/7bd07e0f59df4705a93f8e078eb59843/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1461&bt=1461&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OTppN2VoaTtmOmk7NTtmNEBpMzQzcWk6ZnVqNjMzNGkzM0BiMzBiXzZjX2ExYzE0MzMzYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/fed67d6f548c1580d40a913bc001f34c/646dee37/video/tos/cn/tos-cn-ve-15/7bd07e0f59df4705a93f8e078eb59843/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1461&bt=1461&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OTppN2VoaTtmOmk7NTtmNEBpMzQzcWk6ZnVqNjMzNGkzM0BiMzBiXzZjX2ExYzE0MzMzYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGQo9k5Zm-8HccpD5Bfn5oSo6CE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 19887,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/00827b819dab4a959a42f5cf7731a755_1625099140",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/00827b819dab4a959a42f5cf7731a755_1625099140?x-expires=1686128400&x-signature=GJVN01M3yDXxjzIhxuMJqwRfjCM%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/00827b819dab4a959a42f5cf7731a755_1625099140?x-expires=1686128400&x-signature=8mVXqFWupp4R%2FXOi4SEqc%2FmFnwI%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/00827b819dab4a959a42f5cf7731a755_1625099140?x-expires=1686128400&x-signature=AZE%2FUooX1jmEljpKmiiBP4wWX7I%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"loudness\":\"-5.9\",\"peak\":\"1\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0300fg10000c3egmrrc77ufino0e1t0\",\"url_list\":[\"http://v3-web.douyinvod.com/26b23a6529ca3bad287de58dd4278072/646dee37/video/tos/cn/tos-cn-ve-15-alinc2/b03fab9396974ee6b2cb2003f3db7105/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1427\&bt=1427\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=aDhpMzw3NjMzaWg2Z2hnO0BpMzQzcWk6ZnVqNjMzNGkzM0AzMDVjXy4vNjYxLTM0YzJhYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"http://v26-web.douyinvod.com/f1129a2757b64a2e36f710ac742fb91c/646dee37/video/tos/cn/tos-cn-ve-15-alinc2/b03fab9396974ee6b2cb2003f3db7105/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1427\&bt=1427\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=aDhpMzw3NjMzaWg2Z2hnO0BpMzQzcWk6ZnVqNjMzNGkzM0AzMDVjXy4vNjYxLTM0YzJhYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGQo9k5Zm-8HccpD5Bfn5oSo6CE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":4184084}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-0813/196c701721224448b343d0bef9efe947",
                    "url_list": [
                        "https://p26-sign.douyinpic.com/tos-cn-i-0813/196c701721224448b343d0bef9efe947~noop.jpeg?x-expires=1686128400&x-signature=zpnUlMvDnN6MXTlcS2FJcmuWVTo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-0813/196c701721224448b343d0bef9efe947~noop.jpeg?x-expires=1686128400&x-signature=QdAVqb%2BRmk3SbxyGFKpTAy92F%2BA%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-sign.douyinpic.com/tos-cn-i-0813/196c701721224448b343d0bef9efe947~noop.jpeg?x-expires=1686128400&x-signature=Y8YOoDkgN5RNLYyCLxVUEVy%2Fxy0%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/e5c1ba4e26764e8ba9b3cc0fadae8344_1625099139",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/e5c1ba4e26764e8ba9b3cc0fadae8344_1625099139~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=pn%2FRBB0MtNUEgrJJ6zs9jbsitBA%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/e5c1ba4e26764e8ba9b3cc0fadae8344_1625099139~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=ilbMmWiF0CHAOotvasHe29MpPXA%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/e5c1ba4e26764e8ba9b3cc0fadae8344_1625099139~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=25AYj7X4mQN99HQDq0yqrGMVnfA%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 3232039,
                    "file_cs": "c:0-17740-9e56|d:0-1616018-e1f5,1616019-3232038-b9ff|a:v0300fg10000c3egmrrc77ufino0e1t0",
                    "file_hash": "59cd55ab6efa04a1682a73826c6f2f83",
                    "height": 1246,
                    "uri": "v0300fg10000c3egmrrc77ufino0e1t0",
                    "url_key": "v0300fg10000c3egmrrc77ufino0e1t0_h264_720p_1300161",
                    "url_list": [
                        "http://v3-web.douyinvod.com/6b073a1d777d8ad2eb1f8da16bf04a85/646dee37/video/tos/cn/tos-cn-ve-15/abc33b2db92745b9beef1b5883ca5c76/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1269&bt=1269&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk0Ojg4ZDU5NWdnaWY0NEBpMzQzcWk6ZnVqNjMzNGkzM0A1Ly9fLl8zXl4xNGMxX14xYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/3cef7fe1f845b275f9d3a641588dcaba/646dee37/video/tos/cn/tos-cn-ve-15/abc33b2db92745b9beef1b5883ca5c76/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1269&bt=1269&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Ozk0Ojg4ZDU5NWdnaWY0NEBpMzQzcWk6ZnVqNjMzNGkzM0A1Ly9fLl8zXl4xNGMxX14xYSNxYmxmcjRvamJgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c3egmrrc77ufino0e1t0&line=0&file_id=41a1bc4ffd7d42a6a26ab515b7212688&sign=59cd55ab6efa04a1682a73826c6f2f83&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAVqQU66WjNvsMCXmRQTtn4YYCo_iMGobtVgnGQ-d3iLcvkIV8TQvocN6CG4USGjq7zFrHpesnuGzJHjhKnRxnaMMVPzUxY3kMcDEArNcvA5egj2QxcLWwAonkx06jdSvYJJs3Bi5_gAj0gnpaQDlZFW_JKeEiL0V4JpsSYai2gjt2YRKGJAykkaJYpuLtDoj-4Yqyi1kZRnrXvQrBQ2_0CR4G4n1ZgjCo6vkukZNJB-g",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "7016897343140285732",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 7016897343140285732,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1633748765,
            "desc": "“背叛祖国、分裂国家的人，从来没有好下场，必将遭到人民的唾弃和历史的审判！”总书记说完这句话，现场掌声经久不息！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 31300,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "7016897343140285732",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    7016893219195669760,
                    6886640332398660868,
                    7016889190352686373,
                    6933028503558442247,
                    6933029821966568711,
                    7016897452276010281
                ],
                "similar_id_list_a": [
                    7016897343140285732
                ],
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 31,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 31,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"douyin_beats_info\":{},\"schedule_search_time\":0,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"original_song_uri\":\"ies-music/7016897509612178213.mp3\",\"has_edited\":0,\"review_unshelve_reason\":0,\"beats\":{},\"aggregate_exempt_conf\":[],\"extract_item_id\":7016897343140285732,\"is_aed_music\":0,\"filter_reason\":\"gov_takedown\",\"hotsoon_review_time\":-1,\"cover_colors\":null,\"is_subsidy_exp\":false,\"dsp_switch\":0,\"with_aed_model\":1,\"music_label_id\":null,\"reviewed\":1,\"is_red\":0,\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/7016897509612178213.mp3?x-expires=1685008788&x-signature=R6uTwIA%2BCzFVoQzDu%2BUGdnSVVX0%3D\"}",
                "id": 7016897521222044429,
                "id_str": "7016897521222044429",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "7016897521222044429",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "7016897521222044429",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "7016897521222044429"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 31,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 31
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "4.12 HIV:/ “背叛祖国、分裂国家的人，从来没有好下场，必将遭到人民的唾弃和历史的审判！”总书记说完这句话，现场掌声经久不息！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/7016897343140285732/?region=CN&mid=7016897521222044429&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/7016897343140285732/?region=CN&mid=7016897521222044429&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "7016897343140285732",
                "collect_count": 10779,
                "comment_count": 72546,
                "digg_count": 1424726,
                "play_count": 0,
                "share_count": 45683
            },
            "status": {
                "allow_share": true,
                "aweme_id": "7016897343140285732",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "辛亥革命",
                                "word_id": "6537460537691755780"
                            }
                        ]
                    },
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "辛亥革命",
                                "word_id": "6537460537691755780"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1430152,
                        "gear_name": "normal_1080_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 5595472,
                            "file_cs": "c:0-27645-e617|d:0-2797735-c117,2797736-5595471-e220|a:v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "file_hash": "4145036deb79afa8a3f1f7518023d703",
                            "height": 1600,
                            "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "url_key": "v0300fg10000c5ggdrjc77uc8shpn8o0_h264_1080p_1430152",
                            "url_list": [
                                "http://v3-web.douyinvod.com/81685362140301553f0749adc84ffd6d/646dee43/video/tos/cn/tos-cn-ve-15/5090007467bb4f3494b7898a8750d0ed/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1396&bt=1396&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGY8NDQ7PDYzZTkzOjdkM0BpMztzdmY6ZnVqODMzNGkzM0AwM2FgYmNjNmAxYjAyXzU2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/2bac2f7546b91d88eac1ef3e7ddcf2dd/646dee43/video/tos/cn/tos-cn-ve-15/5090007467bb4f3494b7898a8750d0ed/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1396&bt=1396&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGY8NDQ7PDYzZTkzOjdkM0BpMztzdmY6ZnVqODMzNGkzM0AwM2FgYmNjNmAxYjAyXzU2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&file_id=908ab45730e64bc093f9f8e1c1d96c3a&sign=4145036deb79afa8a3f1f7518023d703&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1080
                        },
                        "quality_type": 1,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 923820,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3614448,
                            "file_cs": "c:0-27627-a498|d:0-1807223-0a12,1807224-3614447-a25b|a:v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "file_hash": "19285a6a6cabbb44cd37cff7a15e6647",
                            "height": 1066,
                            "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "url_key": "v0300fg10000c5ggdrjc77uc8shpn8o0_h264_720p_923820",
                            "url_list": [
                                "http://v3-web.douyinvod.com/fccc72335193f2a873ec55a1fc0e90a1/646dee43/video/tos/cn/tos-cn-ve-15/1915936590334185a9e230d59ffb3995/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=902&bt=902&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OmlkZ2RlZDQ8ZmQ5ZmVmZEBpMztzdmY6ZnVqODMzNGkzM0A0LWAtMDEzNjIxLmI2MDI0YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/2b3b0ba73e1a864d3c94eba88ba160a6/646dee43/video/tos/cn/tos-cn-ve-15/1915936590334185a9e230d59ffb3995/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=902&bt=902&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OmlkZ2RlZDQ8ZmQ5ZmVmZEBpMztzdmY6ZnVqODMzNGkzM0A0LWAtMDEzNjIxLmI2MDI0YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&file_id=7a5c3b9ce61a4c59916a4b3a0dca0f77&sign=19285a6a6cabbb44cd37cff7a15e6647&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 866489,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3390139,
                            "file_cs": "c:0-27605-f82c|d:0-1695068-d97b,1695069-3390138-af7a|a:v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "file_hash": "61a0098bf282edc278ad2238010fe55d",
                            "height": 854,
                            "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "url_key": "v0300fg10000c5ggdrjc77uc8shpn8o0_h264_540p_866489",
                            "url_list": [
                                "http://v3-web.douyinvod.com/960543d4be4647915d5ff40af1539c48/646dee43/video/tos/cn/tos-cn-ve-15/de45c926ae3c4c43b93510ab7a4a48ac/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=846&bt=846&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDU4NjQ2ZmVmOzo4aGVoZ0BpMztzdmY6ZnVqODMzNGkzM0AuYy4yYS5jNTIxNi1jMzQtYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/812a8f61ed944d070d582317b16f760c/646dee43/video/tos/cn/tos-cn-ve-15/de45c926ae3c4c43b93510ab7a4a48ac/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=846&bt=846&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDU4NjQ2ZmVmOzo4aGVoZ0BpMztzdmY6ZnVqODMzNGkzM0AuYy4yYS5jNTIxNi1jMzQtYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&file_id=0d7e6bfe0597485c8bfc13d15315f211&sign=61a0098bf282edc278ad2238010fe55d&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 553527,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2173632,
                            "file_cs": "c:0-21495-c1e2|d:0-1086815-ee18,1086816-2173631-6049|a:v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "file_hash": "1a65afe47a7f4021690ce6fffb5273af",
                            "height": 854,
                            "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                            "url_key": "v0300fg10000c5ggdrjc77uc8shpn8o0_h264_540p_553527",
                            "url_list": [
                                "http://v3-web.douyinvod.com/91bec4ddf15ca0fcaa3e27780ea979fb/646dee43/video/tos/cn/tos-cn-ve-15/534b5c9646ff4c1bb6eddfdec9d8fec0/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=540&bt=540&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=NjQ4NTM2OmdlNDw4NWQ2M0BpMztzdmY6ZnVqODMzNGkzM0BeYS1hLjAyNmAxNmAzMWJfYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/711b29f23da250745c89034a21dccf83/646dee43/video/tos/cn/tos-cn-ve-15/534b5c9646ff4c1bb6eddfdec9d8fec0/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=540&bt=540&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=NjQ4NTM2OmdlNDw4NWQ2M0BpMztzdmY6ZnVqODMzNGkzM0BeYS1hLjAyNmAxNmAzMWJfYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&file_id=b0e34a62c59941cb9d573310d205d1a3&sign=1a65afe47a7f4021690ce6fffb5273af&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/e47ac5349ba0457893be4320896c738d_1633748775",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/e47ac5349ba0457893be4320896c738d_1633748775~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=6u01aIQGYu2a8pyZ8SaopvTauHU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e47ac5349ba0457893be4320896c738d_1633748775?x-expires=2000278800&x-signature=3rNYMNaenZU%2B2VDDashcEBjJp8c%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e47ac5349ba0457893be4320896c738d_1633748775?x-expires=2000278800&x-signature=lUDD7j708h9Mc4AcwFtpXf3gTpU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e47ac5349ba0457893be4320896c738d_1633748775?x-expires=2000278800&x-signature=JUCxj3WzxzLKPA0nc5d9gunupUs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 5020866,
                    "height": 720,
                    "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                    "url_list": [
                        "http://v3-web.douyinvod.com/42b3dd8b6f420fd6f2dc4789ee9fe0ec/646dee43/video/tos/cn/tos-cn-ve-15/a05a500e17104262bb76e26772139635/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1142&bt=1142&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTs1ZTdpNzg7Zzc5MzY6ZUBpMztzdmY6ZnVqODMzNGkzM0A1MDMwY2MyXl8xLjUyYC8tYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/1a4f3eb205508ee08b7e34925da25b90/646dee43/video/tos/cn/tos-cn-ve-15/a05a500e17104262bb76e26772139635/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1142&bt=1142&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTs1ZTdpNzg7Zzc5MzY6ZUBpMztzdmY6ZnVqODMzNGkzM0A1MDMwY2MyXl8xLjUyYC8tYSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGWodkwZne8HccpCsFCmNoZqruE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 31300,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/1b6f2361446c4901ab9b105b803249dd_1633748770",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1b6f2361446c4901ab9b105b803249dd_1633748770?x-expires=1686128400&x-signature=r7A0E3kI5w7FPQqKa1Fuwov0KYI%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1b6f2361446c4901ab9b105b803249dd_1633748770?x-expires=1686128400&x-signature=YlDWGarD61D3ZcTUjh0jI3rnWa4%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1b6f2361446c4901ab9b105b803249dd_1633748770?x-expires=1686128400&x-signature=WUmnSUmf0OHPNkSdTa5JMnA7g3E%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1600,
                "is_h265": 0,
                "is_source_HDR": 0,
                "meta": "{\"loudness\":\"-14.8\",\"peak\":\"0.95499\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0300fg10000c5ggdrjc77uc8shpn8o0\",\"url_list\":[\"http://v3-web.douyinvod.com/20f555c6057b77a61de91a0c6dc7b354/646dee43/video/tos/cn/tos-cn-ve-15/be88eac3d9bf4522acfaa7cc35560ca7/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1059\&bt=1059\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=O2VkZzg6Z2lmZjlnZzk6PEBpMztzdmY6ZnVqODMzNGkzM0AwYTUvMWEvNTIxNTJfYDI2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00018000\",\"http://v26-web.douyinvod.com/e3097a2d91b445bf53e442953b06e5fe/646dee43/video/tos/cn/tos-cn-ve-15/be88eac3d9bf4522acfaa7cc35560ca7/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1059\&bt=1059\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=O2VkZzg6Z2lmZjlnZzk6PEBpMztzdmY6ZnVqODMzNGkzM0AwYTUvMWEvNTIxNTJfYDI2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00018000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESRKvePEcuGWodkwZne8HccpCsFCmNoZqruE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":4653136}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-0813/bea94aa185b04cfcbe55e901ce9e10f7",
                    "url_list": [
                        "https://p26-sign.douyinpic.com/tos-cn-i-0813/bea94aa185b04cfcbe55e901ce9e10f7~noop.jpeg?x-expires=1686128400&x-signature=uEeHdxaEhdr%2BGHmoBDMJS5pu3jQ%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-0813/bea94aa185b04cfcbe55e901ce9e10f7~noop.jpeg?x-expires=1686128400&x-signature=7cxrFeoRJSvTf%2BRNMYqustmgdwU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-sign.douyinpic.com/tos-cn-i-0813/bea94aa185b04cfcbe55e901ce9e10f7~noop.jpeg?x-expires=1686128400&x-signature=KS0X%2FLcbztmcqUzYVTr%2F4wtAIxM%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/3ec6d40609b246dabe4efaa8ebe250cf_1633748768",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/3ec6d40609b246dabe4efaa8ebe250cf_1633748768~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=xwXNMtEadb%2Bo8unmx3eL%2FzJfao4%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/3ec6d40609b246dabe4efaa8ebe250cf_1633748768~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=M%2B068sv%2FPJ9ufFXDG4qOfCxemss%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/3ec6d40609b246dabe4efaa8ebe250cf_1633748768~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=YeA8yB7KaDwaefTFWt3Pls7eXmA%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 5595472,
                    "file_cs": "c:0-27645-e617|d:0-2797735-c117,2797736-5595471-e220|a:v0300fg10000c5ggdrjc77uc8shpn8o0",
                    "file_hash": "4145036deb79afa8a3f1f7518023d703",
                    "height": 1600,
                    "uri": "v0300fg10000c5ggdrjc77uc8shpn8o0",
                    "url_key": "v0300fg10000c5ggdrjc77uc8shpn8o0_h264_1080p_1430152",
                    "url_list": [
                        "http://v3-web.douyinvod.com/81685362140301553f0749adc84ffd6d/646dee43/video/tos/cn/tos-cn-ve-15/5090007467bb4f3494b7898a8750d0ed/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1396&bt=1396&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGY8NDQ7PDYzZTkzOjdkM0BpMztzdmY6ZnVqODMzNGkzM0AwM2FgYmNjNmAxYjAyXzU2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/2bac2f7546b91d88eac1ef3e7ddcf2dd/646dee43/video/tos/cn/tos-cn-ve-15/5090007467bb4f3494b7898a8750d0ed/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1396&bt=1396&cs=0&ds=4&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGY8NDQ7PDYzZTkzOjdkM0BpMztzdmY6ZnVqODMzNGkzM0AwM2FgYmNjNmAxYjAyXzU2YSNsa2U1cjRnYWRgLS1kLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fg10000c5ggdrjc77uc8shpn8o0&line=0&file_id=908ab45730e64bc093f9f8e1c1d96c3a&sign=4145036deb79afa8a3f1f7518023d703&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1080
                },
                "ratio": "1080p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018006,
                    "tag_name": "政务宣传"
                },
                {
                    "level": 3,
                    "tag_id": 2018006001,
                    "tag_name": "宣教科普"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAFz9tsah4n9rCuPUgYkAyFH7VRCebdD9ptZ21taxmJcqtii8m-ssLyXG3tNBCfT8CRPjM86oSfFRInRCb5MvF2jNZR_AZAglUS6LBI9EJKhr78BENPPDURMaWb39kq69CBPxqWfCHZf-nJ-3fJojTd7ymY9UwPK31qrur6JHaEUagyog44fldc4JG4FqjyMkkM-JEzSclBqDXovu19nMcQ2uCxKV10j_9cdVMTf7UV1Q",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6964986350747585828",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6964986350747585828,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1621662290,
            "desc": "痛别！“杂交水稻之父”袁隆平于今日13时07分在长沙逝世，享年91岁。多想再看到您的笑容，袁老千古！送别！ #袁老我们想你了",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 15130,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6964986350747585828",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6776183451734396171
                ],
                "similar_id_list_a": [
                    6964986350747585828
                ],
                "similar_id_list_b": [
                    6964986350747585828
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 15,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 15,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"music_tagging\":{\"Languages\":[\"non_vocal\"],\"Moods\":null,\"Genres\":[\"Pop\"],\"Themes\":null,\"AEDs\":[\"non_vocal\"],\"SingingVersions\":null,\"Instruments\":null},\"is_red\":0,\"original_song_uri\":\"ies-music/6964986478904625957.mp3\",\"extract_item_id\":6964986350747585828,\"hotsoon_review_time\":-1,\"reviewed\":1,\"is_subsidy_exp\":false,\"has_edited\":0,\"douyin_beats_info\":{},\"schedule_search_time\":0,\"aggregate_exempt_conf\":[],\"is_aed_music\":1,\"filter_reason\":\"gov_takedown\",\"review_unshelve_reason\":0,\"beats\":{\"audio_effect_onset\":\"https://sf9-sign.douyinstatic.com/ies-music/strong_beat/v3/1707359063015495?x-expires=1685008788&x-signature=H97Ff17Fb%2FYvD%2FcoyYOsmjgxmpM%3D\",\"beats_tracker\":\"https://sf3-sign.douyinstatic.com/ies-music/strong_beat/v3/1707359075381261?x-expires=1685008788&x-signature=6MCQyjjqVZvV2YUqkXfh63ELPcA%3D\",\"energy_trace\":\"https://sf26-sign.douyinstatic.com/ies-music/strong_beat/v3/1707359054516232?x-expires=1685008788&x-signature=R7PUzRCvNRXPfwFjmizvQMXd0K4%3D\",\"merged_beats\":\"https://sf26-sign.douyinstatic.com/ies-music/strong_beat/v3/1707359082670094?x-expires=1685008788&x-signature=k%2B2EQVvVKET2%2BMxA5iZGxdh%2BCvU%3D\"},\"cover_colors\":null,\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/6964986478904625957.mp3?x-expires=1685008788&x-signature=PfuFDSVw4UdD3%2BcomHRqk%2BMlNdM%3D\",\"music_label_id\":null,\"with_aed_model\":1,\"dsp_switch\":0}",
                "id": 6964986498621917988,
                "id_str": "6964986498621917988",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6964986498621917988",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6964986498621917988",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6964986498621917988"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 15,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf3-sign.douyinstatic.com/ies-music/pattern/a4b4c296318832d90cbd196bc3982c38.json?x-expires=1685008788&x-signature=DPRgoTryhr%2FnlTwwxb6GUX35ubU%3D",
                    "url_list": [
                        "https://sf3-sign.douyinstatic.com/ies-music/pattern/a4b4c296318832d90cbd196bc3982c38.json?x-expires=1685008788&x-signature=DPRgoTryhr%2FnlTwwxb6GUX35ubU%3D",
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/a4b4c296318832d90cbd196bc3982c38.json?x-expires=1685008788&x-signature=gWSYHQFNfu%2BntQY1VhNBhPRC4Dk%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 15
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "2.84 bnD:/ 痛别！“杂交水稻之父”袁隆平于今日13时07分在长沙逝世，享年91岁。多想再看到您的笑容，袁老千古！送别！ # 袁老我们想你了  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6964986350747585828/?region=CN&mid=6964986498621917988&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6964986350747585828/?region=CN&mid=6964986498621917988&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6964986350747585828",
                "collect_count": 112493,
                "comment_count": 4476490,
                "digg_count": 34581631,
                "play_count": 0,
                "share_count": 901037
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6964986350747585828",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "suggest_words": {
                "suggest_words": [
                    {
                        "hint_text": "",
                        "icon_url": "",
                        "scene": "detail_inbox_rex",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "袁隆平",
                                "word_id": "6538727517577073923"
                            }
                        ]
                    },
                    {
                        "hint_text": "大家都在搜：",
                        "icon_url": "",
                        "scene": "comment_top_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "袁隆平逝世当天的街道",
                                "word_id": "7088453325562221836"
                            }
                        ]
                    },
                    {
                        "hint_text": "气泡框词",
                        "icon_url": "",
                        "scene": "search_icon_rec",
                        "words": [
                            {
                                "info": "{\"word_suffix\":\"\",\"recommend_word_type\":\"\",\"history_word_tag\":\"\",\"qrec_for_search\":\"{\\\"video_ecom\\\":\\\"0\\\",\\\"query_ecom\\\":\\\"0\\\",\\\"is_purchase\\\":\\\"0\\\"}\"}",
                                "word": "袁隆平",
                                "word_id": "6538727517577073923"
                            }
                        ]
                    }
                ]
            },
            "text_extra": [
                {
                    "end": 62,
                    "hashtag_id": "1709880597358600",
                    "hashtag_name": "袁老我们想你了",
                    "is_commerce": false,
                    "start": 54,
                    "type": 1
                }
            ],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 680124,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 1286285,
                            "file_cs": "c:0-14052-1506|d:0-643141-ac12,643142-1286284-e591",
                            "file_hash": "a55f71f709f3f3342e2c7191bd206390",
                            "height": 1246,
                            "uri": "v0d00fg10000c2k9k5dmpn581fprh76g",
                            "url_key": "v0d00fg10000c2k9k5dmpn581fprh76g_h264_720p_680124",
                            "url_list": [
                                "http://v3-web.douyinvod.com/2cf5dde48216503bd76390a59126de39/646dee33/video/tos/cn/tos-cn-ve-15/6f1a5263e8c2494bac9e32f6b4b0b161/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=664&bt=664&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTtpNWRpOzc6OGdnNTw1OUBpajp1aTtxcDg8NTMzNGkzM0AwLTBfXjNeNTMxLmItXmFiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/9472db14fe0e18d7ed0c39e24341e9d7/646dee33/video/tos/cn/tos-cn-ve-15/6f1a5263e8c2494bac9e32f6b4b0b161/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=664&bt=664&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTtpNWRpOzc6OGdnNTw1OUBpajp1aTtxcDg8NTMzNGkzM0AwLTBfXjNeNTMxLmItXmFiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g&line=0&file_id=e6d2a902ed1d456784a86faab23f0832&sign=a55f71f709f3f3342e2c7191bd206390&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 631818,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 1194926,
                            "file_cs": "c:0-14053-5330|d:0-597462-c9ed,597463-1194925-24ad",
                            "file_hash": "992216bae4f879152cd54387fc67ec66",
                            "height": 998,
                            "uri": "v0d00fg10000c2k9k5dmpn581fprh76g",
                            "url_key": "v0d00fg10000c2k9k5dmpn581fprh76g_h264_540p_631818",
                            "url_list": [
                                "http://v3-web.douyinvod.com/1d9040ec9603bf1eff8aae4a4fb84e32/646dee33/video/tos/cn/tos-cn-ve-15/32ae87a7cd7b411588b7e5b65e961c41/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=617&bt=617&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODU6ZmQ8OTNlZWhoNjtoZkBpajp1aTtxcDg8NTMzNGkzM0BjMi4wYzEtXzAxYS4tYWAyYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/47c666759dd515955a216a976e8a2dc6/646dee33/video/tos/cn/tos-cn-ve-15/32ae87a7cd7b411588b7e5b65e961c41/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=617&bt=617&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ODU6ZmQ8OTNlZWhoNjtoZkBpajp1aTtxcDg8NTMzNGkzM0BjMi4wYzEtXzAxYS4tYWAyYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g&line=0&file_id=5cced8031ede4b3bb00649fa3c1752f5&sign=992216bae4f879152cd54387fc67ec66&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 407173,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 775870,
                            "file_cs": "c:0-11127-63ff|d:0-387934-a728,387935-775869-dbae",
                            "file_hash": "0da9f823650f0e1a08ae4430e2055532",
                            "height": 998,
                            "uri": "v0d00fg10000c2k9k5dmpn581fprh76g",
                            "url_key": "v0d00fg10000c2k9k5dmpn581fprh76g_h264_540p_407173",
                            "url_list": [
                                "http://v3-web.douyinvod.com/a0c36b864edbae0610791f40ea4211c1/646dee33/video/tos/cn/tos-cn-ve-15/de39bf8a60644ff0bae503ed235fbbb1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=397&bt=397&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=Omg5NzpmNDk5N2QzOWRlZUBpajp1aTtxcDg8NTMzNGkzM0AuMy5jXi40NTIxMi00MS5jYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/325cd8ab3b7607962d1a1675ec4c3013/646dee33/video/tos/cn/tos-cn-ve-15/de39bf8a60644ff0bae503ed235fbbb1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=397&bt=397&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=Omg5NzpmNDk5N2QzOWRlZUBpajp1aTtxcDg8NTMzNGkzM0AuMy5jXi40NTIxMi00MS5jYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g&line=0&file_id=fb1b4a76005a445686711ca7f4166e17&sign=0da9f823650f0e1a08ae4430e2055532&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/ae0ab9408702438b8eae129e4a608994_1621662294",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/ae0ab9408702438b8eae129e4a608994_1621662294~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=f%2B8Zj7vxbSUrEeKgaFJtJXa8Lxc%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/ae0ab9408702438b8eae129e4a608994_1621662294?x-expires=2000278800&x-signature=ZhXyX7Mu49jEwKjbfJYlF%2BDaCC8%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/ae0ab9408702438b8eae129e4a608994_1621662294?x-expires=2000278800&x-signature=laTeVGfM3reRDlFO3uipmBMzVUg%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/ae0ab9408702438b8eae129e4a608994_1621662294?x-expires=2000278800&x-signature=jZ2%2B8LTcm82VY%2BefsGShIwf%2Fb3k%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "height": 720,
                    "uri": "v0d00fg10000c2k9k5dmpn581fprh76g",
                    "url_list": [
                        "http://v3-web.douyinvod.com/9adef6821940d3823ec9f94aabe656d8/646dee33/video/cn/mps/logo/r/p/v0d00fg10000c2k9k5dmpn581fprh76g/e3e167ed3fac43778679f2c1a6142680/mp4/main.mp4?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=0&bt=0&cs=0&ds=3&eid=1280&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Mzk3OTQ1PDk6NmZpZzo0NkBpajp1aTtxcDg8NTMzNGkzM0A1Ly5eYGM0NTQxXjBiM2JiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000&definition=720p&item_id=6964986350747585828&l=2023052417594788E1736391CF0E03184A&logo_type=aweme_search_suffix",
                        "http://v26-web.douyinvod.com/0d940726484fe7890f9bd0e54cdc4e86/646dee33/video/cn/mps/logo/r/p/v0d00fg10000c2k9k5dmpn581fprh76g/e3e167ed3fac43778679f2c1a6142680/mp4/main.mp4?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=0&bt=0&cs=0&ds=3&eid=1280&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Mzk3OTQ1PDk6NmZpZzo0NkBpajp1aTtxcDg8NTMzNGkzM0A1Ly5eYGM0NTQxXjBiM2JiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000&definition=720p&item_id=6964986350747585828&l=2023052417594788E1736391CF0E03184A&logo_type=aweme_search_suffix",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JkfAfESRKvePEcuGRrYc_IXmyWp5pUchXgNgfpeLT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 15130,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/1c2937dea7bc44c8b4f40ad7753d55e8_1621662294",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1c2937dea7bc44c8b4f40ad7753d55e8_1621662294?x-expires=1686128400&x-signature=hSMpF38Mrj7gaqtNTDyHqWjSPE8%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1c2937dea7bc44c8b4f40ad7753d55e8_1621662294?x-expires=1686128400&x-signature=A7G4sWsO%2BDpJskMu%2BokhmzZZ%2FHY%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1c2937dea7bc44c8b4f40ad7753d55e8_1621662294?x-expires=1686128400&x-signature=ybrZl7dKlYCE9E6oNTL8ifs8fDU%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"loudness\":\"-22.1\",\"peak\":\"0.57544\",\"qprf\":\"1.000\",\"sr_score\":\"1.000\",\"title_info\":\"{\\\"ratio_br_l\\\": [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], \\\"ratio_edge_l\\\": [0.01, 0.01, 0.05, 0.18, 0.21, 0.28], \\\"progress_bar\\\": [0.0, 0.0, 0.0], \\\"version\\\": \\\"v1.0\\\"}\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0d00fg10000c2k9k5dmpn581fprh76g\",\"url_list\":[\"http://v3-web.douyinvod.com/199228d92b0f45dec164a3dd32736ae3/646dee33/video/tos/cn/tos-cn-ve-15/dd3f87280c3d490191bfdbaab720cdac/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=753\&bt=753\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ZmUzO2U4NTUzOGhlOjNkO0Bpajp1aTtxcDg8NTMzNGkzM0A1MF8uLzNiNTMxL2E2LjJjYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"http://v26-web.douyinvod.com/a135a5a0a9109a18499715c7cd8988b4/646dee33/video/tos/cn/tos-cn-ve-15/dd3f87280c3d490191bfdbaab720cdac/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=753\&bt=753\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=ZmUzO2U4NTUzOGhlOjNkO0Bpajp1aTtxcDg8NTMzNGkzM0A1MF8uLzNiNTMxL2E2LjJjYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g\&line=0\&ratio=540p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3JkfAfESRKvePEcuGRrYc_IXmyWp5pUchXgNgfpeLT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":1749481}}",
                "optimized_cover": {
                    "height": 720,
                    "uri": "tos-cn-i-0813/d5b803d90b804e37bf2f9f7de002e62b",
                    "url_list": [
                        "https://p6-sign.douyinpic.com/tos-cn-i-0813/d5b803d90b804e37bf2f9f7de002e62b~noop.jpeg?x-expires=1686128400&x-signature=tWaB5Kt2P5XTKNLeNSin4o8czCY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p26-sign.douyinpic.com/tos-cn-i-0813/d5b803d90b804e37bf2f9f7de002e62b~noop.jpeg?x-expires=1686128400&x-signature=CzQlCTqi66ehykKxu%2F0o2bZVSeY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-sign.douyinpic.com/tos-cn-i-0813/d5b803d90b804e37bf2f9f7de002e62b~noop.jpeg?x-expires=1686128400&x-signature=KfhIpVJTEdg1GpiLI4Hmxvdc63Y%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=optimized_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/d7143fe542fd44bfbbfb19f352f30282_1621662293",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/d7143fe542fd44bfbbfb19f352f30282_1621662293~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=3lPjZ9YUUWUVghRN71v5LavANdc%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/d7143fe542fd44bfbbfb19f352f30282_1621662293~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=lvQtSCKceIoyXkAkNue%2FEGf3So0%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/d7143fe542fd44bfbbfb19f352f30282_1621662293~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=WbgCh8efL%2BogMk%2BSQp0l%2FywKRKk%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 1286285,
                    "file_cs": "c:0-14052-1506|d:0-643141-ac12,643142-1286284-e591",
                    "file_hash": "a55f71f709f3f3342e2c7191bd206390",
                    "height": 1246,
                    "uri": "v0d00fg10000c2k9k5dmpn581fprh76g",
                    "url_key": "v0d00fg10000c2k9k5dmpn581fprh76g_h264_720p_680124",
                    "url_list": [
                        "http://v3-web.douyinvod.com/2cf5dde48216503bd76390a59126de39/646dee33/video/tos/cn/tos-cn-ve-15/6f1a5263e8c2494bac9e32f6b4b0b161/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=664&bt=664&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTtpNWRpOzc6OGdnNTw1OUBpajp1aTtxcDg8NTMzNGkzM0AwLTBfXjNeNTMxLmItXmFiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/9472db14fe0e18d7ed0c39e24341e9d7/646dee33/video/tos/cn/tos-cn-ve-15/6f1a5263e8c2494bac9e32f6b4b0b161/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=664&bt=664&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTtpNWRpOzc6OGdnNTw1OUBpajp1aTtxcDg8NTMzNGkzM0AwLTBfXjNeNTMxLmItXmFiYSMzZW0uMm1haGhgLS1kLWFzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0d00fg10000c2k9k5dmpn581fprh76g&line=0&file_id=e6d2a902ed1d456784a86faab23f0832&sign=a55f71f709f3f3342e2c7191bd206390&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 1,
                    "tag_id": 2018,
                    "tag_name": "时政社会"
                },
                {
                    "level": 2,
                    "tag_id": 2018006,
                    "tag_name": "政务宣传"
                },
                {
                    "level": 3,
                    "tag_id": 2018006001,
                    "tag_name": "宣教科普"
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAUIk6WfJYmvIMqK5zI9HyltM5Qo3tdcRZadFfu1f2IQLdjhFcr_KrBc9p2lEFyCur9NOdyxqB1-8Fj2cjVJfiOJ-YlQGugbm2LXrHU4MMX_Ex1mYCsqt9SuTZxgd8SAtoN5TQlEWOzEngvA5oCHvpBuGRChHWULFBMw8uBxIuKmJiTMejpJzljey4aKE-69Ssw-5NiSQ5GInhg0gbwlxns0OjUw73LB1sZcYkeUMs-eA",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6888147864006987016",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6888147864006987016,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1603771923,
            "desc": "感谢各位“亿中人”！今天会来一波奖品，下午见！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 18691,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6888147864006987016",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6888147864006987016
                ],
                "similar_id_list_a": null,
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 18,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 18,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"is_subsidy_exp\":false,\"original_song_uri\":\"ies-music/6888147944676100872.mp3\",\"music_label_id\":null,\"aggregate_exempt_conf\":[],\"has_edited\":0,\"schedule_search_time\":0,\"cover_colors\":null,\"is_red\":0,\"extract_item_id\":6888147864006987016,\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/6888147944676100872.mp3?x-expires=1685008788&x-signature=tgwbPnwZVw3Tg0S5f%2Be36QkI%2B0Y%3D\",\"with_aed_model\":1,\"dsp_switch\":0,\"reviewed\":1,\"beats\":{},\"hotsoon_review_time\":-1,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_aed_music\":0,\"filter_reason\":\"gov_takedown\"}",
                "id": 6888147975009241864,
                "id_str": "6888147975009241864",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6888147975009241864",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6888147975009241864",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6888147975009241864"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 18,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 18
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "5.17 XMw:/ 感谢各位“亿中人”！今天会来一波奖品，下午见！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6888147864006987016/?region=CN&mid=6888147975009241864&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6888147864006987016/?region=CN&mid=6888147975009241864&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6888147864006987016",
                "collect_count": 7947,
                "comment_count": 325488,
                "digg_count": 7828713,
                "play_count": 0,
                "share_count": 10320
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6888147864006987016",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1169074,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2731396,
                            "file_cs": "c:0-17017-dc5d|d:0-1365697-5145,1365698-2731395-06a9",
                            "file_hash": "ab5f32ce275802cb50b956d7bc4e5f53",
                            "height": 1246,
                            "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                            "url_key": "v0200fa50000bubpr4q0j24d8pvv2tjg_h264_720p_1169074",
                            "url_list": [
                                "http://v3-web.douyinvod.com/f0950d0858512acd6988ffe428267157/646dee36/video/tos/cn/tos-cn-ve-15/b3a078a66c814dc2892e6a2842d3a82c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1141&bt=1141&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2hoN2Q6MztkOjo3NGQ7NEBpand5c2c1MzdzeDMzOGkzM0AyYjEtNl4xNWMxLS9jNDQ1YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/5f461b4335b086d043fa52ae27c2cda3/646dee36/video/tos/cn/tos-cn-ve-15/b3a078a66c814dc2892e6a2842d3a82c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1141&bt=1141&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2hoN2Q6MztkOjo3NGQ7NEBpand5c2c1MzdzeDMzOGkzM0AyYjEtNl4xNWMxLS9jNDQ1YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&file_id=81787af1240747fa8840a79a044eee5d&sign=ab5f32ce275802cb50b956d7bc4e5f53&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 868203,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2028448,
                            "file_cs": "c:0-17025-b028|d:0-1014223-4766,1014224-2028447-c12f",
                            "file_hash": "acbd4cd1c272867b01e1da122e18c63f",
                            "height": 998,
                            "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                            "url_key": "v0200fa50000bubpr4q0j24d8pvv2tjg_h264_540p_868203",
                            "url_list": [
                                "http://v3-web.douyinvod.com/fa01dd13ee8e45dd5122be965650527e/646dee36/video/tos/cn/tos-cn-ve-15/2cfc803889944ae881c8b0d65084c3ae/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=847&bt=847&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDk8OGZpNTc7NzdkPDhlZkBpand5c2c1MzdzeDMzOGkzM0BiYDUvLzMyNjUxMDEyLy1iYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/61d9cac33925a2170da3a5f2d792457c/646dee36/video/tos/cn/tos-cn-ve-15/2cfc803889944ae881c8b0d65084c3ae/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=847&bt=847&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDk8OGZpNTc7NzdkPDhlZkBpand5c2c1MzdzeDMzOGkzM0BiYDUvLzMyNjUxMDEyLy1iYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&file_id=ec0b25594a34448894526f2c2589c6ee&sign=acbd4cd1c272867b01e1da122e18c63f&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 832846,
                        "gear_name": "adapt_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 1945841,
                            "file_cs": "c:0-17033-8e18|d:0-972919-4dc4,972920-1945840-682c|a:v0200fa50000bubpr4q0j24d8pvv2tjg",
                            "file_hash": "273d29d9bf5cd5ec9121b05dc1f9d478",
                            "height": 1246,
                            "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                            "url_key": "v0200fa50000bubpr4q0j24d8pvv2tjg_h264_720p_832846",
                            "url_list": [
                                "http://v3-web.douyinvod.com/f3d55d9a39edc174eef285265735da1d/646dee36/video/tos/cn/tos-cn-ve-15c001-alinc2/o4ezupJfAa2UdQOvn8CEE7xyIAPoBBo0VQxxAj/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=813&bt=813&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=11&rc=ZDlkO2Q0aWc3ZGg6NWdpOkBpand5c2c1MzdzeDMzOGkzM0AvMy1iNmIuNmAxYC0wNF8zYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/778a4ed8c0cb6de0c6b233bab57b5f71/646dee36/video/tos/cn/tos-cn-ve-15c001-alinc2/o4ezupJfAa2UdQOvn8CEE7xyIAPoBBo0VQxxAj/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=813&bt=813&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=11&rc=ZDlkO2Q0aWc3ZGg6NWdpOkBpand5c2c1MzdzeDMzOGkzM0AvMy1iNmIuNmAxYC0wNF8zYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&file_id=67bf7d3207ce4ac49d1fe19ae80a662a&sign=273d29d9bf5cd5ec9121b05dc1f9d478&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 18,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 572632,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 1346117,
                            "file_cs": "c:0-13383-839a|d:0-673057-1d59,673058-1346116-f54f",
                            "file_hash": "f04c36097b28d912c6b17caf48e3d4ce",
                            "height": 998,
                            "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                            "url_key": "v0200fa50000bubpr4q0j24d8pvv2tjg_h264_540p_572632",
                            "url_list": [
                                "http://v3-web.douyinvod.com/f123c5f95e7137a5b3973f243959e19e/646dee36/video/tos/cn/tos-cn-ve-15/acc15ac362b5448a9e5ea8bc2f5f0a8e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=559&bt=559&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=aWloNGk2ZWgzNDw1Ozw7OUBpand5c2c1MzdzeDMzOGkzM0A1NV9hMGNjX2MxXzYwMmMuYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/8921dfb111f60ac3bfa43fe5240f9e83/646dee36/video/tos/cn/tos-cn-ve-15/acc15ac362b5448a9e5ea8bc2f5f0a8e/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=559&bt=559&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=aWloNGk2ZWgzNDw1Ozw7OUBpand5c2c1MzdzeDMzOGkzM0A1NV9hMGNjX2MxXzYwMmMuYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&file_id=16f8593892b941f0befbf33fd1be8f8f&sign=f04c36097b28d912c6b17caf48e3d4ce&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/1af6bba376a8418faf169e2c338fdbdd_1603771931",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/1af6bba376a8418faf169e2c338fdbdd_1603771931~tplv-dmt-logomcc:tos-cn-i-0813/91f8757e9bf040fa88667c3c60d6752c:323:430.jpeg?x-expires=2000278800&x-signature=MUIUcgraZYJscmvhzZVXDtIlA20%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1af6bba376a8418faf169e2c338fdbdd_1603771931?x-expires=2000278800&x-signature=MUsd86ImuxYkUW3nTgeNxvn6SeM%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1af6bba376a8418faf169e2c338fdbdd_1603771931?x-expires=2000278800&x-signature=vo%2B1sjGoF263wf3o%2Bdlgd2D5FIs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/1af6bba376a8418faf169e2c338fdbdd_1603771931?x-expires=2000278800&x-signature=ZIzZE87JUBfh5AKLKOIoCOYMJPY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 2946455,
                    "height": 720,
                    "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/a642ff7891e598967706f4312c8151f2/646dee36/video/tos/cn/tos-cn-ve-15/163ff40bea494a969af013dc418b5578/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1060&bt=1060&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2k6Mzg1ODhkZjdpPDs6ZEBpand5c2c1MzdzeDMzOGkzM0BfYS5eNl8wXjMxYC0uMDRgYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/25da9c12beac9182ede19f0aa71478eb/646dee36/video/tos/cn/tos-cn-ve-15/163ff40bea494a969af013dc418b5578/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1060&bt=1060&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2k6Mzg1ODhkZjdpPDs6ZEBpand5c2c1MzdzeDMzOGkzM0BfYS5eNl8wXjMxYC0uMDRgYSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&ratio=720p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESJOvePEcuDWpM4mIGzvQMJoDcFBhtxF5r7T9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 18691,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/e94cd9af9e4840a88bea0c56e5be8eba_1603771926",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/e94cd9af9e4840a88bea0c56e5be8eba_1603771926~tplv-dmt-logom:tos-cn-i-0813/91f8757e9bf040fa88667c3c60d6752c.image?x-expires=1686128400&x-signature=qRK7CZmqypuVftG%2Fsq0KGyU%2B7co%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/e94cd9af9e4840a88bea0c56e5be8eba_1603771926~tplv-dmt-logom:tos-cn-i-0813/91f8757e9bf040fa88667c3c60d6752c.image?x-expires=1686128400&x-signature=dSTuw%2BKQDJ%2FstK9JbFAqGq2vEFM%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/e94cd9af9e4840a88bea0c56e5be8eba_1603771926~tplv-dmt-logom:tos-cn-i-0813/91f8757e9bf040fa88667c3c60d6752c.image?x-expires=1686128400&x-signature=8ybZcIbRAFNh3aqnhB%2B%2F2HQR4xc%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "misc_download_addrs":"{\"suffix_scene\":{\"uri\":\"v0200fa50000bubpr4q0j24d8pvv2tjg\",\"url_list\":[\"http://v3-web.douyinvod.com/4f64372791d09b4d151605bfcdd09003/646dee36/video/tos/cn/tos-cn-ve-15/c97185f2b5f247f2bb71aa112c77919a/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1019\&bt=1019\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=MzhkPDs0O2c1Mzw5ZDRmPEBpand5c2c1MzdzeDMzOGkzM0BjNl4xYTE2NmMxNGEyMjI0YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"http://v26-web.douyinvod.com/19b2543273c710e38d1cce3fa783b0cb/646dee36/video/tos/cn/tos-cn-ve-15/c97185f2b5f247f2bb71aa112c77919a/?a=6383\&ch=4\&cr=3\&dr=0\&lr=all\&cd=0%7C0%7C0%7C3\&cv=1\&br=1019\&bt=1019\&cs=0\&ds=3\&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE\&mime_type=video_mp4\&qs=0\&rc=MzhkPDs0O2c1Mzw5ZDRmPEBpand5c2c1MzdzeDMzOGkzM0BjNl4xYTE2NmMxNGEyMjI0YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D\&l=2023052417594788E1736391CF0E03184A\&btag=e00010000\",\"https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg\&line=0\&ratio=720p\&watermark=1\&media_type=4\&vr_type=0\&improve_bitrate=0\&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESJOvePEcuDWpM4mIGzvQMJoDcFBhtxF5r7T9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=\&logo_name=aweme_toutiao_dy_suffix\&quality_type=11\&source=PackSourceEnum_FAVORITE\"],\"width\":720,\"height\":720,\"data_size\":2831751}}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/ca0c1ee58c424d50b750f419450c2b68_1603771925",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/ca0c1ee58c424d50b750f419450c2b68_1603771925~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=IqfxrBqH21VQ0tlA9iJRp4IeUB8%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/ca0c1ee58c424d50b750f419450c2b68_1603771925~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=FSphczjIt47aE9e6fy8uGHLF7zo%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/ca0c1ee58c424d50b750f419450c2b68_1603771925~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=81lhCFRO3HeOoNYxitNtGjKBdCQ%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 2731396,
                    "file_cs": "c:0-17017-dc5d|d:0-1365697-5145,1365698-2731395-06a9",
                    "file_hash": "ab5f32ce275802cb50b956d7bc4e5f53",
                    "height": 1246,
                    "uri": "v0200fa50000bubpr4q0j24d8pvv2tjg",
                    "url_key": "v0200fa50000bubpr4q0j24d8pvv2tjg_h264_720p_1169074",
                    "url_list": [
                        "http://v3-web.douyinvod.com/f0950d0858512acd6988ffe428267157/646dee36/video/tos/cn/tos-cn-ve-15/b3a078a66c814dc2892e6a2842d3a82c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1141&bt=1141&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2hoN2Q6MztkOjo3NGQ7NEBpand5c2c1MzdzeDMzOGkzM0AyYjEtNl4xNWMxLS9jNDQ1YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/5f461b4335b086d043fa52ae27c2cda3/646dee36/video/tos/cn/tos-cn-ve-15/b3a078a66c814dc2892e6a2842d3a82c/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1141&bt=1141&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=Z2hoN2Q6MztkOjo3NGQ7NEBpand5c2c1MzdzeDMzOGkzM0AyYjEtNl4xNWMxLS9jNDQ1YSNnL3M1MWdub19fLS1eLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200fa50000bubpr4q0j24d8pvv2tjg&line=0&file_id=81787af1240747fa8840a79a044eee5d&sign=ab5f32ce275802cb50b956d7bc4e5f53&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAnms5CNT7qKZe3dSlFtm_AHOkOEixbgcewZEuhqcd-d3_3X06UFI65X12Ph3qmIDJhRXnw3zmq42QUYmj6UVGSP_3k4EpPEYjI6P67yaqEXsXZoLQbMk-RTNkE62ZOSfI_ZiBbocrRkUW30dLHqeNmXXQgZBq7fCWUjoClAXQc35J-FPaq-JdKB9cq305j1NQnSm6zGRiPgDQJJ2plMsMWSEdwZWOWGUTz6yg60kD2h8",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6888244349549677832",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6888244349549677832,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1603794392,
            "desc": "宠粉时刻！感谢您的长期支持，我们将从评论区抽选送出105份礼物。关注央视新闻，“亿”心有你！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 20250,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6888244349549677832",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6888244349549677832
                ],
                "similar_id_list_a": null,
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 20,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 20,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"filter_reason\":\"gov_takedown\",\"is_subsidy_exp\":false,\"review_unshelve_reason\":0,\"hotsoon_review_time\":-1,\"cover_colors\":null,\"is_red\":0,\"original_song_url\":\"https://sf3-sign.douyinstatic.com/ies-music/6888244453606853390.mp3?x-expires=1685008788&x-signature=%2F8bja4xSI8lvFWH7lVtczk8pvXg%3D\",\"original_song_uri\":\"ies-music/6888244453606853390.mp3\",\"is_aed_music\":1,\"has_edited\":0,\"reviewed\":1,\"beats\":{},\"music_tagging\":{\"Languages\":[\"English\"],\"Moods\":[\"Dynamic\"],\"Genres\":[\"Electronic\",\"Pop\"],\"Themes\":[\"Love\",\"Danceable\"],\"AEDs\":[\"Vocal\"],\"SingingVersions\":[\"Cover\"],\"Instruments\":null},\"with_aed_model\":1,\"dsp_switch\":0,\"schedule_search_time\":0,\"music_label_id\":null,\"aggregate_exempt_conf\":[],\"extract_item_id\":6888244349549677832,\"activities\":[10006],\"douyin_beats_info\":{}}",
                "id": 6888244475194313486,
                "id_str": "6888244475194313486",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6888244475194313486",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6888244475194313486",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6888244475194313486"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 20,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 20
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "6.17 Ljc:/ 宠粉时刻！感谢您的长期支持，我们将从评论区抽选送出105份礼物。关注央视新闻，“亿”心有你！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6888244349549677832/?region=CN&mid=6888244475194313486&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6888244349549677832/?region=CN&mid=6888244475194313486&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6888244349549677832",
                "collect_count": 3350,
                "comment_count": 2482631,
                "digg_count": 2446726,
                "play_count": 0,
                "share_count": 7844
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6888244349549677832",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1682725,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4259398,
                            "file_cs": "c:0-17969-3f56|d:0-2129698-a8d3,2129699-4259397-2c5d",
                            "file_hash": "4db0155f9110baf3dbb744d7cc141f95",
                            "height": 1246,
                            "uri": "v0300fa10000bubvasdh22s30tdtpt90",
                            "url_key": "v0300fa10000bubvasdh22s30tdtpt90_h264_720p_1682725",
                            "url_list": [
                                "http://v3-web.douyinvod.com/9bd88588c34b941b6409570bb0512a06/646dee38/video/tos/cn/tos-cn-ve-15/cbf5908f56bf419a8d445680aa6f08e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1643&bt=1643&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2ZTZoaDU8NjlkPDMzZ0BpM3d3dzY1a3Z5eDMzNGkzM0BiX2JhMF8yXjUxM2AwXi81YSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/86ad0594fd903bb8113fae726bbf6647/646dee38/video/tos/cn/tos-cn-ve-15/cbf5908f56bf419a8d445680aa6f08e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1643&bt=1643&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2ZTZoaDU8NjlkPDMzZ0BpM3d3dzY1a3Z5eDMzNGkzM0BiX2JhMF8yXjUxM2AwXi81YSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fa10000bubvasdh22s30tdtpt90&line=0&file_id=8d20a039ca664389a25ebe33dbe3bfeb&sign=4db0155f9110baf3dbb744d7cc141f95&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1326701,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3358213,
                            "file_cs": "c:0-17969-0507|d:0-1679105-dc44,1679106-3358212-f8ab",
                            "file_hash": "89ce01bf709983a3fecaa1750140d9b9",
                            "height": 998,
                            "uri": "v0300fa10000bubvasdh22s30tdtpt90",
                            "url_key": "v0300fa10000bubvasdh22s30tdtpt90_h264_540p_1326701",
                            "url_list": [
                                "http://v3-web.douyinvod.com/93f735753fab95feeea769b855e08b3b/646dee38/video/tos/cn/tos-cn-ve-15/5f6ed5bcc69f4c51a8ae132b6e4ed090/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1295&bt=1295&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OmloNTU6Nmg3ZTQ6NWY6O0BpM3d3dzY1a3Z5eDMzNGkzM0A0XmBhYy9fXzIxMDUyNGBfYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/06ae2ac65f5bff9566cdd957df437dbe/646dee38/video/tos/cn/tos-cn-ve-15/5f6ed5bcc69f4c51a8ae132b6e4ed090/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1295&bt=1295&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OmloNTU6Nmg3ZTQ6NWY6O0BpM3d3dzY1a3Z5eDMzNGkzM0A0XmBhYy9fXzIxMDUyNGBfYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fa10000bubvasdh22s30tdtpt90&line=0&file_id=b8c77c5287314b54beb327f2d2ceaf77&sign=89ce01bf709983a3fecaa1750140d9b9&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 962742,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2450661,
                            "file_cs": "c:0-14051-a481|d:0-1225329-92c6,1225330-2450660-cd52",
                            "file_hash": "828e01f7f89fb4016dbe39e3edb1d912",
                            "height": 998,
                            "uri": "v0300fa10000bubvasdh22s30tdtpt90",
                            "url_key": "v0300fa10000bubvasdh22s30tdtpt90_h264_540p_962742",
                            "url_list": [
                                "http://v3-web.douyinvod.com/527ecd6ccd951909f37d163b0a719e88/646dee38/video/tos/cn/tos-cn-ve-15/e4dd4ba72ee84ab7b6671b39ba099bea/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=940&bt=940&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=NjlmNDk4ZjtpODU7Ozs8aUBpM3d3dzY1a3Z5eDMzNGkzM0BhNi9jMDFeXzAxNC82Y14tYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/53908ea3f2f795af5e654e716a74a3a7/646dee38/video/tos/cn/tos-cn-ve-15/e4dd4ba72ee84ab7b6671b39ba099bea/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=940&bt=940&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=NjlmNDk4ZjtpODU7Ozs8aUBpM3d3dzY1a3Z5eDMzNGkzM0BhNi9jMDFeXzAxNC82Y14tYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300fa10000bubvasdh22s30tdtpt90&line=0&file_id=0fa9f8982872453fb8ac4536f12c96d3&sign=828e01f7f89fb4016dbe39e3edb1d912&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/862d3a0ba2fe497fabbfa662565544d0_1603794397",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/862d3a0ba2fe497fabbfa662565544d0_1603794397~tplv-dmt-logomcc:tos-cn-i-0813/25bf0d82935545ceb53d207410fbe691:323:430.jpeg?x-expires=2000278800&x-signature=errJJVZNQLDUGJxCfV2WcA5W5Yw%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/862d3a0ba2fe497fabbfa662565544d0_1603794397?x-expires=2000278800&x-signature=BE3LHlyllLs6zZauugBF1H1TfN4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/862d3a0ba2fe497fabbfa662565544d0_1603794397?x-expires=2000278800&x-signature=gVuB6FHphKuja%2FZ3fICaQRTdEKo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/862d3a0ba2fe497fabbfa662565544d0_1603794397?x-expires=2000278800&x-signature=Yy%2BjV8XLfvqiDIWivHQBwi8s79E%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 4463228,
                    "height": 720,
                    "uri": "v0300fa10000bubvasdh22s30tdtpt90",
                    "url_list": [
                        "http://v3-web.douyinvod.com/dc268c3a76e18c2bed2ff6460328403f/646dee38/video/tos/cn/tos-cn-ve-15/b52467820550492fa93d8b9c1fb86651/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1498&bt=1498&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDRnNmhoM2YzOzk2OjRmM0BpM3d3dzY1a3Z5eDMzNGkzM0BjLl41MjU0XzMxM2JjNTBhYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/c1a75ecf8c2d30af7531424d00d022ac/646dee38/video/tos/cn/tos-cn-ve-15/b52467820550492fa93d8b9c1fb86651/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1498&bt=1498&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDRnNmhoM2YzOzk2OjRmM0BpM3d3dzY1a3Z5eDMzNGkzM0BjLl41MjU0XzMxM2JjNTBhYSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fa10000bubvasdh22s30tdtpt90&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfESJKvePEcuDWpMg1Z3m3GMIvWslFlN4H5u2E9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme_search_suffix&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 20250,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/511931bcdd5b49558e6adc7183c9d896_1603794395",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/511931bcdd5b49558e6adc7183c9d896_1603794395~tplv-dmt-logom:tos-cn-i-0813/25bf0d82935545ceb53d207410fbe691.image?x-expires=1686128400&x-signature=q7giupK8d%2BMfk48untDgeZPhn7U%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/511931bcdd5b49558e6adc7183c9d896_1603794395~tplv-dmt-logom:tos-cn-i-0813/25bf0d82935545ceb53d207410fbe691.image?x-expires=1686128400&x-signature=Nr%2B8%2F64DpmQoaCB6cbhL6WjoywI%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/511931bcdd5b49558e6adc7183c9d896_1603794395~tplv-dmt-logom:tos-cn-i-0813/25bf0d82935545ceb53d207410fbe691.image?x-expires=1686128400&x-signature=MF5g3vHQwjkAQaqAG4vwubzkxsA%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/56d766b3cf69462381d0b25d1a365958_1603794394",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/56d766b3cf69462381d0b25d1a365958_1603794394~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=TBm6Mzr6N8nEK316A9KwTnu9oOk%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/56d766b3cf69462381d0b25d1a365958_1603794394~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=VvBRakrdu4Ue%2BsCAID8KMPyHzAw%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/56d766b3cf69462381d0b25d1a365958_1603794394~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=c1iZ2AmP5GfZL03NWXO4wC%2BIquw%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 4259398,
                    "file_cs": "c:0-17969-3f56|d:0-2129698-a8d3,2129699-4259397-2c5d",
                    "file_hash": "4db0155f9110baf3dbb744d7cc141f95",
                    "height": 1246,
                    "uri": "v0300fa10000bubvasdh22s30tdtpt90",
                    "url_key": "v0300fa10000bubvasdh22s30tdtpt90_h264_720p_1682725",
                    "url_list": [
                        "http://v3-web.douyinvod.com/9bd88588c34b941b6409570bb0512a06/646dee38/video/tos/cn/tos-cn-ve-15/cbf5908f56bf419a8d445680aa6f08e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1643&bt=1643&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2ZTZoaDU8NjlkPDMzZ0BpM3d3dzY1a3Z5eDMzNGkzM0BiX2JhMF8yXjUxM2AwXi81YSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/86ad0594fd903bb8113fae726bbf6647/646dee38/video/tos/cn/tos-cn-ve-15/cbf5908f56bf419a8d445680aa6f08e7/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1643&bt=1643&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZWk2ZTZoaDU8NjlkPDMzZ0BpM3d3dzY1a3Z5eDMzNGkzM0BiX2JhMF8yXjUxM2AwXi81YSM2bWEtcC9hXl9fLS1eLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300fa10000bubvasdh22s30tdtpt90&line=0&file_id=8d20a039ca664389a25ebe33dbe3bfeb&sign=4db0155f9110baf3dbb744d7cc141f95&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAANrVE05V85dZviHqC22x3jfsx_g0QZpisuuQdBke12_m_OvFsPKeUtwMiEJhbK-4E0hYjU6fzESEA7LmDOjVPNSOZZS7UU1vCQ1ywb7jtaZnZPalQQML9W5VVg-6DmWwhYceV9oP2zSodrXTJF8bgiuLTeIp-BGAWZkNgltMjCPaJO5cIvWu2BRMxhtD_0ajqQES07nK3NL_jCvOdzKUOmX6KXGOHTzCWyzrtWnmmLAc",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6710826320617639179",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6710826320617639179,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1562546934,
            "desc": "“不可能了，不可能了” 说完这句话，即将90岁的袁隆平老人长舒了一口气。",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 29676,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6710826320617639179",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6710826320617639179
                ],
                "similar_id_list_a": null,
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 29,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 29,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"has_edited\":0,\"reviewed\":1,\"schedule_search_time\":0,\"is_aed_music\":0,\"with_aed_model\":1,\"review_unshelve_reason\":0,\"beats\":{\"audio_effect_onset\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640504333727757\",\"beats_tracker\":\"https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640504356827144\",\"energy_trace\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640504333710344\",\"merged_beats\":\"https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640504356848653\"},\"music_label_id\":null,\"dsp_switch\":0,\"douyin_beats_info\":{},\"is_red\":0,\"is_subsidy_exp\":false,\"extract_item_id\":6710826320617639179,\"hotsoon_review_time\":-1,\"cover_colors\":null,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"aggregate_exempt_conf\":[]}",
                "id": 6710941793569131272,
                "id_str": "6710941793569131272",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6710941793569131272",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 1,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1638444639225895.mp3",
                    "url_key": "6710941793569131272",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1638444639225895.mp3",
                        "https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/1638444639225895.mp3"
                    ],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 0,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6710941793569131272"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 29,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/f3dd30a615eb06efb4958640ba0612cc.json",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/f3dd30a615eb06efb4958640ba0612cc.json",
                        "https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/pattern/f3dd30a615eb06efb4958640ba0612cc.json"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 29
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "CN",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "5.82 gOk:/ “不可能了，不可能了” 说完这句话，即将90岁的袁隆平老人长舒了一口气。  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6710826320617639179/?region=CN&mid=6710941793569131272&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6710826320617639179/?region=CN&mid=6710941793569131272&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6710826320617639179",
                "collect_count": 22706,
                "comment_count": 324261,
                "digg_count": 10165505,
                "play_count": 0,
                "share_count": 62802
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6710826320617639179",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 30,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 801090,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2971645,
                            "file_hash": "ce00ebf0e52e125b7c7d240c6ae4c852",
                            "height": 854,
                            "uri": "v0200f520000bkh95rfeqk8d95lvabrg",
                            "url_key": "v0200f520000bkh95rfeqk8d95lvabrg_h264_540p_801090",
                            "url_list": [
                                "http://v3-web.douyinvod.com/02053fb173a9166d23bf52d1764f929e/646dee41/video/tos/cn/tos-cn-ve-15/1199e46ac3894394ba12021fcbb9488a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=782&bt=782&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTc6OjRkNjo1PDc3ZTo2NkBpamV5OGduaHU8bjMzNWkzM0AwMGE2XjVgNjUxMjEvMF9fYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "http://v26-web.douyinvod.com/e0d484c21f07a194bb8b4940a6b9fd30/646dee41/video/tos/cn/tos-cn-ve-15/1199e46ac3894394ba12021fcbb9488a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=782&bt=782&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTc6OjRkNjo1PDc3ZTo2NkBpamV5OGduaHU8bjMzNWkzM0AwMGE2XjVgNjUxMjEvMF9fYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f520000bkh95rfeqk8d95lvabrg&line=0&file_id=b3b3372b4454498297c38aa197d73432&sign=ce00ebf0e52e125b7c7d240c6ae4c852&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "2a02f0005bc19f02dfb87",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/2a02f0005bc19f02dfb87~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=T8zXuw84tZgID8xJiV4ywyEpKCs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/2a02f0005bc19f02dfb87?x-expires=2000278800&x-signature=dGNIdQoGuHMCvCz7CcSk3smxwLw%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/2a02f0005bc19f02dfb87?x-expires=2000278800&x-signature=BHsOCWKq09EmxelbXdLmmpaurAs%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/2a02f0005bc19f02dfb87?x-expires=2000278800&x-signature=9MU2cvmOGWkVaoP%2B0ge6S%2FSLLyI%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 3647294,
                    "height": 720,
                    "uri": "v0200f520000bkh95rfeqk8d95lvabrg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/1ef9ee437917f0cffb102b405d56b1ae/646dee41/video/tos/cn/tos-cn-ve-0015c800/220c9017d96679646889c53eba89cf35c201162c87880000babad3837860/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=960&bt=960&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGdlO2U8ZzQzNjY8OzZnOEBpamV5OGduaHU8bjMzNWkzM0A0Xi5hYzJhNjAxMi8tXzJhYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/79fe37abc278e4781fc015a921a19a5b/646dee41/video/tos/cn/tos-cn-ve-0015c800/220c9017d96679646889c53eba89cf35c201162c87880000babad3837860/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=960&bt=960&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZGdlO2U8ZzQzNjY8OzZnOEBpamV5OGduaHU8bjMzNWkzM0A0Xi5hYzJhNjAxMi8tXzJhYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f520000bkh95rfeqk8d95lvabrg&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfEXZJvePEcuDIrodhZnu6W5tkDcAEnNwW8KbT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 29676,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "29c1c0000fceb0b2b8067",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/obj/29c1c0000fceb0b2b8067?x-expires=1686128400&x-signature=NVLu0J%2BmFqCnD41VOEUrgRZzzg4%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/29c1c0000fceb0b2b8067?x-expires=1686128400&x-signature=HhcUZJXXEeVAddDhUmqlNQaRIXA%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/29c1c0000fceb0b2b8067?x-expires=1686128400&x-signature=V4fSJJvl8NUz9HZQB7YlXwetzlA%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 948,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "29f3a000366135a307f80",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/29f3a000366135a307f80~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=s4W3me%2BljZ1uX4ht2i%2B3WoyHzZM%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/29f3a000366135a307f80~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=yJxYJh%2BMakEoMmMGSBymveDKRHI%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/29f3a000366135a307f80~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=we7A0KWZQZu1cCTlmwwvprBwHUs%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 2971645,
                    "file_hash": "ce00ebf0e52e125b7c7d240c6ae4c852",
                    "height": 854,
                    "uri": "v0200f520000bkh95rfeqk8d95lvabrg",
                    "url_key": "v0200f520000bkh95rfeqk8d95lvabrg_h264_540p_801090",
                    "url_list": [
                        "http://v3-web.douyinvod.com/02053fb173a9166d23bf52d1764f929e/646dee41/video/tos/cn/tos-cn-ve-15/1199e46ac3894394ba12021fcbb9488a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=782&bt=782&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTc6OjRkNjo1PDc3ZTo2NkBpamV5OGduaHU8bjMzNWkzM0AwMGE2XjVgNjUxMjEvMF9fYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "http://v26-web.douyinvod.com/e0d484c21f07a194bb8b4940a6b9fd30/646dee41/video/tos/cn/tos-cn-ve-15/1199e46ac3894394ba12021fcbb9488a/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=782&bt=782&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NTc6OjRkNjo1PDc3ZTo2NkBpamV5OGduaHU8bjMzNWkzM0AwMGE2XjVgNjUxMjEvMF9fYSNvXmk2NW5jMmVfLS0yLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00018000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f520000bkh95rfeqk8d95lvabrg&line=0&file_id=b3b3372b4454498297c38aa197d73432&sign=ce00ebf0e52e125b7c7d240c6ae4c852&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 576
                },
                "ratio": "540p",
                "video_model": "",
                "width": 640
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAFrL24YpgUzosIDc2pxbpWiUwQqhRs5QTDHjOGw4wYzp0XkRw6r2QubSRMDYadvdOdjTlZhyb0JOH_50x1xhWsaRbZE0XGKEVTwIR6l5wAN4exqL4BIm1g1u5lb5T-ynffvH2uE-YALip1P5yCAz5zABWFJSTtwbfYg4v7ivaTkczXQTcETMAC7uN97YAbyWVBxYWn4pO17706Sx4bmav5BSM967Bkx0X0hQXVYf0rzA",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6810566367130045704",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6810566367130045704,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1585708582,
            "desc": "被暖到了！游客热情邀请总书记一起泛舟，总书记笑着说“我很想去，就是人太多了”。",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 17690,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6810566367130045704",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6810566367130045704
                ],
                "similar_id_list_a": [
                    6810566367130045704
                ],
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 17,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 17,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"dsp_switch\":0,\"reviewed\":1,\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"aggregate_exempt_conf\":[],\"extract_item_id\":6810566367130045704,\"is_aed_music\":0,\"with_aed_model\":1,\"has_edited\":0,\"cover_colors\":null,\"is_red\":0,\"original_song_url\":\"https://sf9-sign.douyinstatic.com/ies-music/1662734339017767.mp3?x-expires=1685008788&x-signature=%2FkMF6NeJlaARD0osBtp1GLneVJg%3D\",\"original_song_uri\":\"ies-music/1662734339017767.mp3\",\"filter_reason\":\"gov_takedown\",\"beats\":{},\"schedule_search_time\":0,\"is_subsidy_exp\":false,\"music_label_id\":null,\"hotsoon_review_time\":-1,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null}}",
                "id": 6810558085942283015,
                "id_str": "6810558085942283015",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6810558085942283015",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6810558085942283015",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6810558085942283015"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 17,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 17
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "1.23 jPk:/ 被暖到了！游客热情邀请总书记一起泛舟，总书记笑着说“我很想去，就是人太多了”。  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6810566367130045704/?region=CN&mid=6810558085942283015&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6810566367130045704/?region=CN&mid=6810558085942283015&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6810566367130045704",
                "collect_count": 75119,
                "comment_count": 146,
                "digg_count": 22660100,
                "play_count": 0,
                "share_count": 463080
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6810566367130045704",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1887234,
                        "gear_name": "normal_720_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4173147,
                            "file_hash": "0508db991fa48ca6737abe3a800affe8",
                            "height": 1246,
                            "uri": "v0200f920000bq1vrt91h1vsj6okis90",
                            "url_key": "v0200f920000bq1vrt91h1vsj6okis90_h264_720p_1887234",
                            "url_list": [
                                "http://v3-web.douyinvod.com/87bae2f10d11ed33f66e4e1c075645e4/646dee35/video/tos/cn/tos-cn-ve-15/ce3e3bcee2c74858a40eab0908e08ca6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1843&bt=1843&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2Q0ZTo0aTw3aTU3OGU8aUBpM3ZuOXY0NHd5dDMzNWkzM0A0LjRjMWFiX2IxYi1jMmFgYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/758f25e1bf952ae05839250f98ffb3d9/646dee35/video/tos/cn/tos-cn-ve-15/ce3e3bcee2c74858a40eab0908e08ca6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1843&bt=1843&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2Q0ZTo0aTw3aTU3OGU8aUBpM3ZuOXY0NHd5dDMzNWkzM0A0LjRjMWFiX2IxYi1jMmFgYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f920000bq1vrt91h1vsj6okis90&line=0&file_id=cfd95bf504e24fe4b9efd147fb711a78&sign=0508db991fa48ca6737abe3a800affe8&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 720
                        },
                        "quality_type": 10,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1387288,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3067641,
                            "file_cs": "c:0-16381-945d|d:0-1533819-437e,1533820-3067640-15ba",
                            "file_hash": "6c19ef9df80467af70d4add0e83392d5",
                            "height": 998,
                            "uri": "v0200f920000bq1vrt91h1vsj6okis90",
                            "url_key": "v0200f920000bq1vrt91h1vsj6okis90_h264_540p_1387288",
                            "url_list": [
                                "http://v3-web.douyinvod.com/d636df7cf67600cd5be1cafa813f5aa9/646dee35/video/tos/hxsy/tos-hxsy-ve-0015/a45dd98b293a49cfbc0d310d5ddf50a4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1354&bt=1354&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2hlN2g2NjRmZWVpM2c6ZEBpM3ZuOXY0NHd5dDMzNWkzM0A0X15iYWIzXzAxNS0zYmI0YSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/2712e0bc4ae9a164de1698254eb47460/646dee35/video/tos/hxsy/tos-hxsy-ve-0015/a45dd98b293a49cfbc0d310d5ddf50a4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1354&bt=1354&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2hlN2g2NjRmZWVpM2c6ZEBpM3ZuOXY0NHd5dDMzNWkzM0A0X15iYWIzXzAxNS0zYmI0YSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f920000bq1vrt91h1vsj6okis90&line=0&file_id=7ae7ed600f8b4b3cb163e3dee4abbe78&sign=6c19ef9df80467af70d4add0e83392d5&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    },
                    {
                        "FPS": 25,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 934891,
                        "gear_name": "lower_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 2080600,
                            "file_cs": "c:0-12951-6c0a",
                            "file_hash": "3dfe50b042dd7536a3b4b357b9f3fbb6",
                            "height": 998,
                            "uri": "v0200f920000bq1vrt91h1vsj6okis90",
                            "url_key": "v0200f920000bq1vrt91h1vsj6okis90_h264_540p_934891",
                            "url_list": [
                                "http://v3-web.douyinvod.com/661fbca5c9569a73a605d327d7bd16ba/646dee35/video/tos/cn/tos-cn-ve-15/1d27c0737ff743bd90d22f4c49e6aed2/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=912&bt=912&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=MzRpZTU7OzRoM2c2NzlkZ0BpM3ZuOXY0NHd5dDMzNWkzM0AxL2AtNDRgNjUxLWAyYzA2YSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/57504e1a5f12722a2674d1babb0e2b14/646dee35/video/tos/cn/tos-cn-ve-15/1d27c0737ff743bd90d22f4c49e6aed2/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=912&bt=912&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=4&rc=MzRpZTU7OzRoM2c2NzlkZ0BpM3ZuOXY0NHd5dDMzNWkzM0AxL2AtNDRgNjUxLWAyYzA2YSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f920000bq1vrt91h1vsj6okis90&line=0&file_id=9d3af654c30d408e91c878720bcf2140&sign=3dfe50b042dd7536a3b4b357b9f3fbb6&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 24,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/871410e3dfad4c348c22bffcbe83c22b",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/871410e3dfad4c348c22bffcbe83c22b~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=fIQCOa4HmXLtEA3md8Z1F8ND56U%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/871410e3dfad4c348c22bffcbe83c22b?x-expires=2000278800&x-signature=OtfoU40ZdRiVc5RycUXgYviVaPA%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/871410e3dfad4c348c22bffcbe83c22b?x-expires=2000278800&x-signature=kavmGF9UZhcVc4b3xmbC6h1qow0%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/871410e3dfad4c348c22bffcbe83c22b?x-expires=2000278800&x-signature=JYizQLckj%2BEsPxpeSGoMPISz2Ww%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 4121984,
                    "height": 720,
                    "uri": "v0200f920000bq1vrt91h1vsj6okis90",
                    "url_list": [
                        "http://v3-web.douyinvod.com/93b5cb583de1a8660cca670cecd2c1ed/646dee35/video/tos/hxsy/tos-hxsy-ve-0015/b7a40bb5bad142ce882a01429a51c3b8/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1820&bt=1820&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aGllZzlmOTs7NDxpZjU7PEBpM3ZuOXY0NHd5dDMzNWkzM0AyYl81XzA1NTUxYy0yL2BjYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/f1def4625bf04866e2b942107bb4b06a/646dee35/video/tos/hxsy/tos-hxsy-ve-0015/b7a40bb5bad142ce882a01429a51c3b8/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1820&bt=1820&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aGllZzlmOTs7NDxpZjU7PEBpM3ZuOXY0NHd5dDMzNWkzM0AyYl81XzA1NTUxYy0yL2BjYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f920000bq1vrt91h1vsj6okis90&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfEXpJvePEcuDS98gmYCTuQsEqGpMHn8Ee4e2E9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 17690,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/9666b0d25f1149b4bc1cf2b582f14bd6_1585708584",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9666b0d25f1149b4bc1cf2b582f14bd6_1585708584?x-expires=1686128400&x-signature=upWOHA6FMzH7FpOKFNgSFnShnIs%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9666b0d25f1149b4bc1cf2b582f14bd6_1585708584?x-expires=1686128400&x-signature=S2%2FU5ymYAU1G1yjjt7XkC9Kh%2F%2BA%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/9666b0d25f1149b4bc1cf2b582f14bd6_1585708584?x-expires=1686128400&x-signature=jmyO%2FVt3ARYa%2B1XX99NIxvtRLlg%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1870,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/6abf035439614648a28fd2025eb73772_1585708583",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/6abf035439614648a28fd2025eb73772_1585708583~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=bfJfGy6Sw8ROnyapRTJF%2BeQB7vU%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/6abf035439614648a28fd2025eb73772_1585708583~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=L8LLZr44dXKPkH%2BzVa2sXw%2B%2Fd3I%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/6abf035439614648a28fd2025eb73772_1585708583~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=1JUD70stGagHJ8FSbxstdVSEfEM%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 4173147,
                    "file_hash": "0508db991fa48ca6737abe3a800affe8",
                    "height": 1246,
                    "uri": "v0200f920000bq1vrt91h1vsj6okis90",
                    "url_key": "v0200f920000bq1vrt91h1vsj6okis90_h264_720p_1887234",
                    "url_list": [
                        "http://v3-web.douyinvod.com/87bae2f10d11ed33f66e4e1c075645e4/646dee35/video/tos/cn/tos-cn-ve-15/ce3e3bcee2c74858a40eab0908e08ca6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1843&bt=1843&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2Q0ZTo0aTw3aTU3OGU8aUBpM3ZuOXY0NHd5dDMzNWkzM0A0LjRjMWFiX2IxYi1jMmFgYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/758f25e1bf952ae05839250f98ffb3d9/646dee35/video/tos/cn/tos-cn-ve-15/ce3e3bcee2c74858a40eab0908e08ca6/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1843&bt=1843&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=O2Q0ZTo0aTw3aTU3OGU8aUBpM3ZuOXY0NHd5dDMzNWkzM0A0LjRjMWFiX2IxYi1jMmFgYSM2Zmxnc2U2by5fLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f920000bq1vrt91h1vsj6okis90&line=0&file_id=cfd95bf504e24fe4b9efd147fb711a78&sign=0508db991fa48ca6737abe3a800affe8&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "ratio": "720p",
                "video_model": "",
                "width": 1080
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAA1Nnat-JpIDvZsTs_USeSSi_X40WnLsen97GfduHlG3ZbBA39qZ4LaXeRzZ2R0wAuAAKwCV6kuxmGSwG9XgA0RNjIZGJpy9MWJY1sNuA2iFW9TGvX4WId8-UPVoOkddkBFC4Hn72myB8l4BSvNtvfSqSEdoSXnGm-z5WC6EXt5lu09GFZPoNi1VdNjdH5urP4-qET80X9Pg-pTgnl-bpbXMW_El3wFv4G-tlWnAkMi6A",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6783660110951582983",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6783660110951582983,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1579443963,
            "desc": "“彭妈妈没来，快过年了都在家里忙着呢。”哈哈，总书记这段“拉家常”太赞了，爱了爱了！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 14258,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6783660110951582983",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6783660110951582983
                ],
                "similar_id_list_a": [
                    6783660110951582983
                ],
                "similar_id_list_b": [
                    6783660110951582983
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"political_review_offline\",\"music_detail_fail_type\":8,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 14,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 14,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"is_subsidy_exp\":false,\"dsp_switch\":0,\"has_edited\":0,\"schedule_search_time\":0,\"cover_colors\":null,\"is_aed_music\":0,\"with_aed_model\":1,\"filter_reason\":\"gov_takedown\",\"douyin_beats_info\":{},\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"is_red\":0,\"music_label_id\":null,\"beats\":{},\"original_song_uri\":\"ies-music/1656163702231048.mp3\",\"aggregate_exempt_conf\":[],\"extract_item_id\":6783660110951582983,\"reviewed\":1,\"review_unshelve_reason\":0,\"hotsoon_review_time\":-1,\"original_song_url\":\"https://sf9-sign.douyinstatic.com/ies-music/1656163702231048.mp3?x-expires=1685008788&x-signature=ZNkOR8imKpYupuviiPpsHML%2B9jU%3D\"}",
                "id": 6783644629047053063,
                "id_str": "6783644629047053063",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_exempt_for_reply": true,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6783644629047053063",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6783644629047053063",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6783644629047053063"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 14,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf26-sign.douyinstatic.com/ies-music/pattern/f03af715f7c57472a1bd05859f1e7c65.json?x-expires=1685008788&x-signature=Z2e0FZ9Hd%2FST6HoSPeLFSoGfUhU%3D",
                    "url_list": [
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/f03af715f7c57472a1bd05859f1e7c65.json?x-expires=1685008788&x-signature=Z2e0FZ9Hd%2FST6HoSPeLFSoGfUhU%3D",
                        "https://sf6-sign.douyinstatic.com/ies-music/pattern/f03af715f7c57472a1bd05859f1e7c65.json?x-expires=1685008788&x-signature=jrhhotcwIqpMBy6udVUL1BsJu%2F0%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 14
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "CN",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "0.71 ztr:/ “彭妈妈没来，快过年了都在家里忙着呢。”哈哈，总书记这段“拉家常”太赞了，爱了爱了！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6783660110951582983/?region=CN&mid=6783644629047053063&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6783660110951582983/?region=CN&mid=6783644629047053063&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6783660110951582983",
                "collect_count": 105540,
                "comment_count": 733521,
                "digg_count": 30498829,
                "play_count": 0,
                "share_count": 933059
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6783660110951582983",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 30,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2007259,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3577439,
                            "file_cs": "c:0-16848-334b",
                            "file_hash": "43d68421755364e4fae68270b54e7d11",
                            "height": 854,
                            "uri": "v0200ff10000boi6ds32ap9f8d5ddrlg",
                            "url_key": "v0200ff10000boi6ds32ap9f8d5ddrlg_h264_540p_2007259",
                            "url_list": [
                                "http://v3-web.douyinvod.com/791b25e4155ecc754ffa04dbd1bd2aaa/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/7df39a067d9b477cba681a0f83e83e50/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1960&bt=1960&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmVmaTU4NjU7OjVpZDRnM0BpanVnZ2lzNXY5cjMzNGkzM0BjNmMtXmMzXzQxMi9gNTRjYSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                                "http://v26-web.douyinvod.com/98e9445132d362134863405e58126a31/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/7df39a067d9b477cba681a0f83e83e50/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1960&bt=1960&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmVmaTU4NjU7OjVpZDRnM0BpanVnZ2lzNXY5cjMzNGkzM0BjNmMtXmMzXzQxMi9gNTRjYSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200ff10000boi6ds32ap9f8d5ddrlg&line=0&file_id=f07d81ca2f524778b263f5a20ffc9bfc&sign=43d68421755364e4fae68270b54e7d11&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/74d12b1eb74e4527b68b29b30537b8e0_1579443966",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/74d12b1eb74e4527b68b29b30537b8e0_1579443966~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=jcvhDGFniOeEih3sP4JuRL3NK9Q%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/74d12b1eb74e4527b68b29b30537b8e0_1579443966?x-expires=2000278800&x-signature=znCBOyaOTn80s8dO8oiD8%2BPBHYw%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/74d12b1eb74e4527b68b29b30537b8e0_1579443966?x-expires=2000278800&x-signature=lxPgUPjC%2FQYMUETjJpV1rYyAvIM%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/74d12b1eb74e4527b68b29b30537b8e0_1579443966?x-expires=2000278800&x-signature=1FHOmfLWBamEy2S%2BE800Ieka%2BgU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 4829153,
                    "height": 720,
                    "uri": "v0200ff10000boi6ds32ap9f8d5ddrlg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/60ca717ae44bcb5515cd88cc13680772/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/e956032fed594d59b27680a3be555488/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2646&bt=2646&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aWRoOGY0PGk7ODg3ZmU3aEBpanVnZ2lzNXY5cjMzNGkzM0AxNjBeNjBfX2ExYGI0LS01YSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                        "http://v26-web.douyinvod.com/46a6d9af460c8cbdce252107f74a8af6/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/e956032fed594d59b27680a3be555488/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2646&bt=2646&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aWRoOGY0PGk7ODg3ZmU3aEBpanVnZ2lzNXY5cjMzNGkzM0AxNjBeNjBfX2ExYGI0LS01YSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200ff10000boi6ds32ap9f8d5ddrlg&line=0&ratio=720p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfESVKvePEcuDMr4gwZy7tS4BlD8FVxc4T4LjT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 14258,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/041c37afc9214322855130f06edadb72_1579443966",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/041c37afc9214322855130f06edadb72_1579443966?x-expires=1686128400&x-signature=fcIT%2Fj710K7oFww2F4vLLrYExKA%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/041c37afc9214322855130f06edadb72_1579443966?x-expires=1686128400&x-signature=T8%2Bl3RUWBGaO6zCJWjOgFiFTX7o%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/041c37afc9214322855130f06edadb72_1579443966?x-expires=1686128400&x-signature=kFP3NOij1BSb1aMxBQHxc61%2Fbxo%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1068,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/dba4ec39662a417b8bc964bd8962f797_1579443966",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/dba4ec39662a417b8bc964bd8962f797_1579443966~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=IvpaPEPl9ZqXNGZnMlkHIen00i0%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/dba4ec39662a417b8bc964bd8962f797_1579443966~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=sWnCo95s1MFKHgdyTz92QXbeLzw%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/dba4ec39662a417b8bc964bd8962f797_1579443966~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=8NqjOeut4Dq0ZvbyviB4jvtLS64%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 3577439,
                    "file_cs": "c:0-16848-334b",
                    "file_hash": "43d68421755364e4fae68270b54e7d11",
                    "height": 854,
                    "uri": "v0200ff10000boi6ds32ap9f8d5ddrlg",
                    "url_key": "v0200ff10000boi6ds32ap9f8d5ddrlg_h264_540p_2007259",
                    "url_list": [
                        "http://v3-web.douyinvod.com/791b25e4155ecc754ffa04dbd1bd2aaa/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/7df39a067d9b477cba681a0f83e83e50/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1960&bt=1960&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmVmaTU4NjU7OjVpZDRnM0BpanVnZ2lzNXY5cjMzNGkzM0BjNmMtXmMzXzQxMi9gNTRjYSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                        "http://v26-web.douyinvod.com/98e9445132d362134863405e58126a31/646dee32/video/tos/hxsy/tos-hxsy-ve-0015/7df39a067d9b477cba681a0f83e83e50/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1960&bt=1960&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZmVmaTU4NjU7OjVpZDRnM0BpanVnZ2lzNXY5cjMzNGkzM0BjNmMtXmMzXzQxMi9gNTRjYSNpYTI1Nl4wYWZfLS1jLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00008000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200ff10000boi6ds32ap9f8d5ddrlg&line=0&file_id=f07d81ca2f524778b263f5a20ffc9bfc&sign=43d68421755364e4fae68270b54e7d11&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 576
                },
                "ratio": "540p",
                "video_model": "",
                "width": 720
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAA27JLMFZSm4QaDgNBPN16AmjnNTit3smtnoJ-67PFsrY5r9npyc1vr0dIDQKL64AZx1iKJuafo3wQ9nm5m28o3-hDZtlDf_y00zzXGFGJq8soxKGNHnRNZyYRx6WgzhjF4ivAHqt32KYC-U5pa42mIQXUHYFveSpknuSw76ZmDasMgoINrXv7lEJCydUNuk_0_agAeq9rwatkwN5qmw5rz5gujS6FrS5ePyZrQEp-15s",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6721119088430632196",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6721119088430632196,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1564908860,
            "desc": "这盛世，如你所愿！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 28050,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6721119088430632196",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6721119088430632196
                ],
                "similar_id_list_a": [
                    6721119088430632196
                ],
                "similar_id_list_b": [
                    6721119088430632196
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 28,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 28,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"reviewed\":1,\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"music_label_id\":null,\"has_edited\":0,\"schedule_search_time\":0,\"beats\":{\"audio_effect_onset\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640944102378509\",\"beats_tracker\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640944123453453\",\"energy_trace\":\"https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640944102365198\",\"merged_beats\":\"https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1640944123473924\"},\"cover_colors\":null,\"is_red\":0,\"is_subsidy_exp\":false,\"aggregate_exempt_conf\":[],\"extract_item_id\":6721119088430632196,\"is_aed_music\":0,\"dsp_switch\":0,\"hotsoon_review_time\":-1,\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"with_aed_model\":1}",
                "id": 6721179554007780109,
                "id_str": "6721179554007780109",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6721179554007780109",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 1,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1640921819449352.mp3",
                    "url_key": "6721179554007780109",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1640921819449352.mp3",
                        "https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/1640921819449352.mp3"
                    ],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 0,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6721179554007780109"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 28,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/b50efa89a422d5464edba7db4570786c.json",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/b50efa89a422d5464edba7db4570786c.json",
                        "https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/pattern/b50efa89a422d5464edba7db4570786c.json"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 28
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "CN",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "7.12 pda:/ 这盛世，如你所愿！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6721119088430632196/?region=CN&mid=6721179554007780109&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6721119088430632196/?region=CN&mid=6721179554007780109&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6721119088430632196",
                "collect_count": 16952,
                "comment_count": 187581,
                "digg_count": 7580883,
                "play_count": 0,
                "share_count": 56883
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6721119088430632196",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 30,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 1056026,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 3702694,
                            "file_hash": "27bee13250286a07fc9fbb9ab4dcc6b1",
                            "height": 998,
                            "uri": "v0200f950000bl39qdulg9jim3l2peh0",
                            "url_key": "v0200f950000bl39qdulg9jim3l2peh0_h264_540p_1056026",
                            "url_list": [
                                "http://v3-web.douyinvod.com/6c4b7b3a522f3855116fe3d0278bc741/646dee40/video/tos/cn/tos-cn-ve-0015c800/2207772a1a039814ec08863c96a80150b6811631374b0000b160f2c7d8c1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1031&bt=1031&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTQ5ZWQ0OmhoaDw4Zjw4ZEBpM2g1Nmw8b2c8bzMzOGkzM0BiMl8zYS0wXl4xMS8yXmIuYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/9e5eca5de477781578a2860b579b7d7c/646dee40/video/tos/cn/tos-cn-ve-0015c800/2207772a1a039814ec08863c96a80150b6811631374b0000b160f2c7d8c1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1031&bt=1031&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTQ5ZWQ0OmhoaDw4Zjw4ZEBpM2g1Nmw8b2c8bzMzOGkzM0BiMl8zYS0wXl4xMS8yXmIuYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f950000bl39qdulg9jim3l2peh0&line=0&file_id=1ae5a95c25494eaeae3701da6bb651ef&sign=27bee13250286a07fc9fbb9ab4dcc6b1&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "2c9a4000297111c7bf809",
                    "url_list": [
                        "https://p9-pc-sign.douyinpic.com/2c9a4000297111c7bf809~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=CdSefv9bhTeFWkdyLWg3PQH7om4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/2c9a4000297111c7bf809?x-expires=2000278800&x-signature=E6hrbUAsmMyGREaAXLMyjyijbuc%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/2c9a4000297111c7bf809?x-expires=2000278800&x-signature=l5hGvmFzSlasgL%2B1IpwRYY1MnIU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/2c9a4000297111c7bf809?x-expires=2000278800&x-signature=hsmBi9xw51Pn%2BYHt8u8oy1ippHo%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 5431905,
                    "height": 720,
                    "uri": "v0200f950000bl39qdulg9jim3l2peh0",
                    "url_list": [
                        "http://v3-web.douyinvod.com/fab210015118bc854fc5dff6ed2f4919/646dee40/video/tos/cn/tos-cn-ve-0015c800/220a56fea27180b4022bb2f77cf72a947931163148b000007d48d077bbea/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1512&bt=1512&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDxoN2Y0N2hoOzk2NGRkNkBpM2g1Nmw8b2c8bzMzOGkzM0AtY2M0YS01NjUxNWA2Yy4tYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/bece4a8a10e3cd7bbb5ae0602a0dc3a6/646dee40/video/tos/cn/tos-cn-ve-0015c800/220a56fea27180b4022bb2f77cf72a947931163148b000007d48d077bbea/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1512&bt=1512&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aDxoN2Y0N2hoOzk2NGRkNkBpM2g1Nmw8b2c8bzMzOGkzM0AtY2M0YS01NjUxNWA2Yy4tYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f950000bl39qdulg9jim3l2peh0&line=0&ratio=720p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfEXpOvePEcuDP9YclcGizTck2AJQCnJgH97yE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 28050,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "2c22c000dd484645ede18",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/2c22c000dd484645ede18?x-expires=1686128400&x-signature=QLGpA95Fhu%2F6gtCg3WwyqsfcvQQ%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/2c22c000dd484645ede18?x-expires=1686128400&x-signature=hWE%2BcColjihiF9C%2BPNeutfkwGLY%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/2c22c000dd484645ede18?x-expires=1686128400&x-signature=PJs8JBwUyXPEbHPQzapRoQCyN4E%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 1248,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "2c591000b14da97ded1bc",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/2c591000b14da97ded1bc~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=YXXFzpb%2Bl9o5067xnrWlrDQ%2BegM%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/2c591000b14da97ded1bc~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=WwVKnFkfG0pEUrwYLxkbglWcoHU%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/2c591000b14da97ded1bc~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=7PxnkGIQFA%2BLhPDG7KrgM6aCcx4%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 3702694,
                    "file_hash": "27bee13250286a07fc9fbb9ab4dcc6b1",
                    "height": 998,
                    "uri": "v0200f950000bl39qdulg9jim3l2peh0",
                    "url_key": "v0200f950000bl39qdulg9jim3l2peh0_h264_540p_1056026",
                    "url_list": [
                        "http://v3-web.douyinvod.com/6c4b7b3a522f3855116fe3d0278bc741/646dee40/video/tos/cn/tos-cn-ve-0015c800/2207772a1a039814ec08863c96a80150b6811631374b0000b160f2c7d8c1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1031&bt=1031&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTQ5ZWQ0OmhoaDw4Zjw4ZEBpM2g1Nmw8b2c8bzMzOGkzM0BiMl8zYS0wXl4xMS8yXmIuYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/9e5eca5de477781578a2860b579b7d7c/646dee40/video/tos/cn/tos-cn-ve-0015c800/2207772a1a039814ec08863c96a80150b6811631374b0000b160f2c7d8c1/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1031&bt=1031&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=aTQ5ZWQ0OmhoaDw4Zjw4ZEBpM2g1Nmw8b2c8bzMzOGkzM0BiMl8zYS0wXl4xMS8yXmIuYSNlbWlqZ2RybjBfLS02LS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f950000bl39qdulg9jim3l2peh0&line=0&file_id=1ae5a95c25494eaeae3701da6bb651ef&sign=27bee13250286a07fc9fbb9ab4dcc6b1&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 576
                },
                "ratio": "540p",
                "video_model": "",
                "width": 720
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAAKrAic8TyOlKlqoJTolovBwISPJHN59196RxwmkC3SCHD0JvYvvO1-Sukg2ncblJF09Rgem1I8jZTMicSJxkVcmicPR9SfoebfugQeLarx4oCuPf9g-nbbFgP0p4XyXUv1ANqP0QxTvjmKb4jgm1mzmvdaAfrAYDV_D4njD0toNzQY-wx5Kd1rcIzs6_b9ZjXAIvEkc4jd2w0qbXV7gHGULM_X7gS9bb5hOBDPb-p1G8",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6732425664521096459",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6732425664521096459,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1567515004,
            "desc": "帅！回顾“九三阅兵”震撼场面，每个动作都像是复制粘贴！一起期待，国庆70年大阅兵！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 15906,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6732425664521096459",
            "horizontal_type": 1,
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6732425664521096459
                ],
                "similar_id_list_a": [
                    6732425664521096459
                ],
                "similar_id_list_b": [
                    6732425664521096459
                ]
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 15,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 15,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"dsp_switch\":0,\"schedule_search_time\":0,\"is_subsidy_exp\":false,\"has_edited\":0,\"music_label_id\":null,\"extract_item_id\":6732425664521096459,\"is_aed_music\":1,\"reviewed\":0,\"review_unshelve_reason\":0,\"douyin_beats_info\":{},\"music_tagging\":{\"Languages\":null,\"Moods\":null,\"Genres\":null,\"Themes\":null,\"AEDs\":null,\"SingingVersions\":null,\"Instruments\":null},\"aggregate_exempt_conf\":[],\"beats\":{\"audio_effect_onset\":\"https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1643707699451908\",\"beats_tracker\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1643707708643357\",\"energy_trace\":\"https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1643707699430429\",\"merged_beats\":\"https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/strong_beat/v3/1643707708666884\"},\"hotsoon_review_time\":-1,\"cover_colors\":null,\"is_red\":0,\"with_aed_model\":1}",
                "id": 6732399362145651468,
                "id_str": "6732399362145651468",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6732399362145651468",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 1,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1643655901190147.mp3",
                    "url_key": "6732399362145651468",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/1643655901190147.mp3",
                        "https://sf86-cdn-tos.douyinstatic.com/obj/ies-music/1643655901190147.mp3"
                    ],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 0,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6732399362145651468"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 15,
                "source_platform": 23,
                "start_time": 0,
                "status": 1,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/1942cd629ad7b28aa27d85b132f930a7.json",
                    "url_list": [
                        "https://sf6-cdn-tos.douyinstatic.com/obj/ies-music/pattern/1942cd629ad7b28aa27d85b132f930a7.json",
                        "https://sf3-cdn-tos.douyinstatic.com/obj/ies-music/pattern/1942cd629ad7b28aa27d85b132f930a7.json"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 15
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "CN",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "6.69 use:/ 帅！回顾“九三阅兵”震撼场面，每个动作都像是复制粘贴！一起期待，国庆70年大阅兵！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6732425664521096459/?region=CN&mid=6732399362145651468&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6732425664521096459/?region=CN&mid=6732399362145651468&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6732425664521096459",
                "collect_count": 8001,
                "comment_count": 55756,
                "digg_count": 1997190,
                "play_count": 0,
                "share_count": 48794
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6732425664521096459",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 30,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 2344045,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 4660549,
                            "file_hash": "a9e9197d7cae730b8143f60c8282e73f",
                            "height": 576,
                            "uri": "v0200f480000bln62ahpskdj6ovrc4hg",
                            "url_key": "v0200f480000bln62ahpskdj6ovrc4hg_h264_540p_2344045",
                            "url_list": [
                                "http://v3-web.douyinvod.com/35e7ce6856f56799fd86db05b7f49c45/646dee33/video/tos/cn/tos-cn-ve-0015c800/2208f5262cd77a145a793d54b6dedc8ea2c1163614d4000050451d1453ec/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2289&bt=2289&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OjNmO2gzOjpnPGVmaWc1ZkBpajd1cm1uc2Q5bzMzO2kzM0AwXl8zMDI2XjAxYDZhLjA1YSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/30c0d150fb5207cb278e9f1ed07ce38d/646dee33/video/tos/cn/tos-cn-ve-0015c800/2208f5262cd77a145a793d54b6dedc8ea2c1163614d4000050451d1453ec/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2289&bt=2289&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OjNmO2gzOjpnPGVmaWc1ZkBpajd1cm1uc2Q5bzMzO2kzM0AwXl8zMDI2XjAxYDZhLjA1YSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0200f480000bln62ahpskdj6ovrc4hg&line=0&file_id=8c321ddf9ccb493da797503e68bca037&sign=a9e9197d7cae730b8143f60c8282e73f&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 1024
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/4731505166a34ffbb0757fafcbefd3cf",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/4731505166a34ffbb0757fafcbefd3cf~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=uvR9y4YUs9EZXDhjWvTEjfjrDDk%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/4731505166a34ffbb0757fafcbefd3cf?x-expires=2000278800&x-signature=zPtKpImsFMMGoTIb3SxXDLTHkuY%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/4731505166a34ffbb0757fafcbefd3cf?x-expires=2000278800&x-signature=ywJAW8fzl7SxMkGfvGFKgJJ4tWI%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/4731505166a34ffbb0757fafcbefd3cf?x-expires=2000278800&x-signature=kaXikyExTKO7D3eyv3x8CYq4H1c%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 5885779,
                    "height": 720,
                    "uri": "v0200f480000bln62ahpskdj6ovrc4hg",
                    "url_list": [
                        "http://v3-web.douyinvod.com/b61d74008916939b6b4ba685f2448c56/646dee33/video/tos/cn/tos-cn-ve-0015c800/220bd75892560864a4da20e2a3be0a35e3b1163557f1000097b8f308eeb4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2890&bt=2890&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZzNkZjczM2dpNTk6Z2gzZEBpajd1cm1uc2Q5bzMzO2kzM0AyYjBgMGFhX18xMV9jYV9eYSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/92b9bf414caa27a0f047a1d13fb2e0c6/646dee33/video/tos/cn/tos-cn-ve-0015c800/220bd75892560864a4da20e2a3be0a35e3b1163557f1000097b8f308eeb4/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2890&bt=2890&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=ZzNkZjczM2dpNTk6Z2gzZEBpajd1cm1uc2Q5bzMzO2kzM0AyYjBgMGFhX18xMV9jYV9eYSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f480000bln62ahpskdj6ovrc4hg&line=0&ratio=720p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3Jx_AfEXdDvePEcuDPqIhmdXWvWZs4A89ehtgUprzT9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&quality_type=11&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 15906,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/cf0479a7b07e492d9a4f568bd7095f48",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/cf0479a7b07e492d9a4f568bd7095f48?x-expires=1686128400&x-signature=rnP0ajC5M2qrBxAtJa6tZ%2F2C8vQ%3D&from=3213915784_large",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/cf0479a7b07e492d9a4f568bd7095f48?x-expires=1686128400&x-signature=ZuIDMrk1%2BcuTg5AzWlyOuoN8QbU%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/cf0479a7b07e492d9a4f568bd7095f48?x-expires=1686128400&x-signature=HhAKmYnSxuwCw7Fu51AYRNANMAk%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 720,
                "horizontal_type": 1,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/addebff09a454ab0aa0d6cb587365ca4",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/addebff09a454ab0aa0d6cb587365ca4~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=R4a39CGYCLZpFZPA8TG4qmMUBFU%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/addebff09a454ab0aa0d6cb587365ca4~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=CGc6OrGlOlASA5G5lJEEYi3ekhY%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/addebff09a454ab0aa0d6cb587365ca4~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=X0wYLnIixXMY1cwzC6raB6A%2BXsA%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 4660549,
                    "file_hash": "a9e9197d7cae730b8143f60c8282e73f",
                    "height": 576,
                    "uri": "v0200f480000bln62ahpskdj6ovrc4hg",
                    "url_key": "v0200f480000bln62ahpskdj6ovrc4hg_h264_540p_2344045",
                    "url_list": [
                        "http://v3-web.douyinvod.com/35e7ce6856f56799fd86db05b7f49c45/646dee33/video/tos/cn/tos-cn-ve-0015c800/2208f5262cd77a145a793d54b6dedc8ea2c1163614d4000050451d1453ec/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2289&bt=2289&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OjNmO2gzOjpnPGVmaWc1ZkBpajd1cm1uc2Q5bzMzO2kzM0AwXl8zMDI2XjAxYDZhLjA1YSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/30c0d150fb5207cb278e9f1ed07ce38d/646dee33/video/tos/cn/tos-cn-ve-0015c800/2208f5262cd77a145a793d54b6dedc8ea2c1163614d4000050451d1453ec/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=2289&bt=2289&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=OjNmO2gzOjpnPGVmaWc1ZkBpajd1cm1uc2Q5bzMzO2kzM0AwXl8zMDI2XjAxYDZhLjA1YSNlYHMzYXBlL2tfLS0xLS9zcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0200f480000bln62ahpskdj6ovrc4hg&line=0&file_id=8c321ddf9ccb493da797503e68bca037&sign=a9e9197d7cae730b8143f60c8282e73f&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 1024
                },
                "ratio": "540p",
                "video_model": "",
                "width": 1280
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        },
        {
            "anchors": null,
            "authentication_token": "MS4wLjAAAAAA8N-_u8NIs9qgti63YrJiPFkr_zI4JL-d9JxXk98hrt0PZR-g1ME-e5VxRCmV6N6buPOVA6vpP8EMy5vc4RWKFT4J9ByEG3OOEGtOI-y5f9ZLjMXT2eRWykDNncG69zQHIi9niFgTX1LogsGUqh9WkBIVR_YEFAY7Y86oEWgkIIr9vPX83YRGjrnm8KPfTjuDF_P5t8sUfTOW7gxt_IaRWoFw8HR-7qs1nw__e3iwV7E",
            "author": {
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "custom_verify": "",
                "enterprise_verify_reason": "央视新闻官方抖音号",
                "follow_status": 0,
                "follower_status": 0,
                "is_ad_fake": false,
                "nickname": "央视新闻",
                "prevent_download": false,
                "risk_notice_text": "",
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "secret": 0,
                "share_info": {
                    "share_desc": "",
                    "share_desc_info": "",
                    "share_qrcode_url": {
                        "height": 720,
                        "uri": "72a4000fe1b5d865c51b",
                        "url_list": [
                            "https://p9-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=NebuTG%2FTS%2FbIM8Jel2o8IwXIN0U%3D&from=116350172",
                            "https://p3-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=%2B%2BrH4rcTZDgZ72kobQ9AiAoD2jw%3D&from=116350172",
                            "https://p6-pc-sign.douyinpic.com/obj/72a4000fe1b5d865c51b?x-expires=1684940400&x-signature=cZyw20pIKkOrJYwkfJCwQfvliLo%3D&from=116350172"
                        ],
                        "width": 720
                    },
                    "share_title": "",
                    "share_title_myself": "",
                    "share_title_other": "",
                    "share_url": "",
                    "share_weibo_desc": ""
                },
                "short_id": "653421556",
                "signature": "我用心，你放心。",
                "uid": "66598046050",
                "unique_id": "cctvnews",
                "verification_type": 0
            },
            "author_mask_tag": 0,
            "author_user_id": 66598046050,
            "aweme_control": {
                "can_comment": true,
                "can_forward": true,
                "can_share": true,
                "can_show_comment": true
            },
            "aweme_id": "6741899236838853901",
            "aweme_type": 0,
            "challenge_position": null,
            "chapter_list": null,
            "collect_stat": 0,
            "comment_gid": 6741899236838853901,
            "comment_list": null,
            "comment_permission_info": {
                "can_comment": true,
                "comment_permission_status": 0,
                "item_detail_entry": false,
                "press_entry": false,
                "toast_guide": false
            },
            "commerce_config_data": null,
            "common_bar_info": "[]",
            "component_info_v2": "{\"desc_lines_limit\":0,\"hide_marquee\":false}",
            "cover_labels": null,
            "create_time": 1569720743,
            "desc": "国士之心，祖国最懂！",
            "digg_lottie": {
                "can_bomb": 0,
                "lottie_id": ""
            },
            "disable_relation_bar": 0,
            "distribute_circle": {
                "campus_block_interaction": false,
                "distribute_type": 0
            },
            "duet_aggregate_in_music_tab": false,
            "duration": 15535,
            "geofencing": [],
            "geofencing_regions": null,
            "group_id": "6741899236838853901",
            "hybrid_label": null,
            "image_album_music_info": {
                "begin_time": -1,
                "end_time": -1,
                "volume": -1
            },
            "image_comment": {},
            "image_infos": null,
            "image_list": null,
            "images": null,
            "impression_data": {
                "group_id_list_a": [],
                "group_id_list_b": [],
                "group_id_list_c": [
                    6741899236838853901
                ],
                "similar_id_list_a": null,
                "similar_id_list_b": null
            },
            "interaction_stickers": null,
            "is_ads": false,
            "is_collects_selected": 0,
            "is_duet_sing": false,
            "is_image_beat": false,
            "is_life_item": false,
            "is_story": 0,
            "is_top": 0,
            "item_warn_notification": {
                "content": "",
                "show": false,
                "type": 0
            },
            "label_top_text": null,
            "libfinsert_task_id": "",
            "long_video": null,
            "main_arch_common": "{\"music_detail_fail_reason\":\"other_offline\",\"music_detail_fail_type\":9,\"music_detail_fail_toast\":\"该声音不可用\"}",
            "music": {
                "album": "",
                "artist_user_infos": null,
                "artists": [],
                "audition_duration": 15,
                "author": "央视新闻",
                "author_deleted": false,
                "author_position": null,
                "author_status": 1,
                "avatar_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "avatar_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "binded_challenge_id": 0,
                "can_background_play": true,
                "collect_stat": 0,
                "cover_hd": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_large": {
                    "height": 720,
                    "uri": "1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/1080x1080/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_medium": {
                    "height": 720,
                    "uri": "720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/720x720/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "cover_thumb": {
                    "height": 720,
                    "uri": "100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03",
                    "url_list": [
                        "https://p3-pc.douyinpic.com/aweme/100x100/aweme-avatar/tos-cn-i-0813c001_c38c2117f66846ed91ea2501733f6e03.jpeg?from=116350172"
                    ],
                    "width": 720
                },
                "dmv_auto_show": false,
                "dsp_status": 10,
                "duration": 15,
                "end_time": 0,
                "external_song_info": [],
                "extra": "{\"original_song_url\":\"https://sf26-sign.douyinstatic.com/ies-music/1645970789345340.mp3?x-expires=1685008788&x-signature=Ke7gfWXYUuDTGSseLnWN1DzHmp0%3D\",\"has_edited\":0,\"douyin_beats_info\":{},\"music_tagging\":{\"Languages\":[\"non_vocal\"],\"Moods\":[\"Excited\"],\"Genres\":[\"Electronic\"],\"Themes\":[\"Danceable\"],\"AEDs\":[\"non_vocal\"],\"SingingVersions\":null,\"Instruments\":null},\"original_song_uri\":\"ies-music/1645970789345340.mp3\",\"music_label_id\":null,\"aggregate_exempt_conf\":[],\"dsp_switch\":0,\"beats\":{\"audio_effect_onset\":\"https://sf3-sign.douyinstatic.com/ies-music/strong_beat/v3/1645977970793479?x-expires=1685008788&x-signature=3Cqz9RDc6s1ZTBIwEQnzaULTR08%3D\",\"beats_tracker\":\"https://sf26-sign.douyinstatic.com/ies-music/strong_beat/v3/1645977980187651?x-expires=1685008788&x-signature=8C1EMoDjP%2BD7P07Sd004uPOybuA%3D\",\"energy_trace\":\"https://sf3-sign.douyinstatic.com/ies-music/strong_beat/v3/1645977970767883?x-expires=1685008788&x-signature=qJS4nIdIrxmp47MVu7UeXT%2FIxi4%3D\",\"merged_beats\":\"https://sf26-sign.douyinstatic.com/ies-music/strong_beat/v3/1645977980213261?x-expires=1685008788&x-signature=Q%2FkDn9pXevenO31TVTPYOL93CNA%3D\"},\"is_red\":0,\"extract_item_id\":6741899236838853901,\"is_aed_music\":1,\"filter_reason\":\"other_takedown\",\"reviewed\":1,\"schedule_search_time\":0,\"cover_colors\":null,\"is_subsidy_exp\":false,\"with_aed_model\":1,\"review_unshelve_reason\":0,\"hotsoon_review_time\":-1}",
                "id": 6741891852313692942,
                "id_str": "6741891852313692942",
                "is_audio_url_with_cookie": false,
                "is_commerce_music": false,
                "is_del_video": false,
                "is_matched_metadata": false,
                "is_original": false,
                "is_original_sound": true,
                "is_pgc": false,
                "is_restricted": false,
                "is_video_self_see": false,
                "lyric_short_position": null,
                "mid": "6741891852313692942",
                "music_chart_ranks": null,
                "music_collect_count": 0,
                "music_cover_atmosphere_color_value": "",
                "music_status": 0,
                "musician_user_infos": null,
                "mute_share": false,
                "offline_desc": "该声音不可用",
                "owner_handle": "cctvnews",
                "owner_id": "66598046050",
                "owner_nickname": "央视新闻",
                "pgc_music_type": 2,
                "play_url": {
                    "height": 720,
                    "uri": "",
                    "url_key": "6741891852313692942",
                    "url_list": [],
                    "width": 720
                },
                "position": null,
                "prevent_download": false,
                "prevent_item_download_status": 0,
                "preview_end_time": 0,
                "preview_start_time": 0,
                "reason_type": 2,
                "redirect": false,
                "schema_url": "",
                "search_impr": {
                    "entity_id": "6741891852313692942"
                },
                "sec_uid": "MS4wLjABAAAAgq8cb7cn9ByhZbmx-XQDdRTvFzmJeBBXOUO4QflP96M",
                "shoot_duration": 15,
                "source_platform": 23,
                "start_time": 0,
                "status": 0,
                "strong_beat_url": {
                    "height": 720,
                    "uri": "https://sf6-sign.douyinstatic.com/ies-music/pattern/fe8520e2ab7354d76b01049afbbd2b68.json?x-expires=1685008788&x-signature=px3Tj9JRfUDKTVrTi%2FNsrcC9D54%3D",
                    "url_list": [
                        "https://sf6-sign.douyinstatic.com/ies-music/pattern/fe8520e2ab7354d76b01049afbbd2b68.json?x-expires=1685008788&x-signature=px3Tj9JRfUDKTVrTi%2FNsrcC9D54%3D",
                        "https://sf26-sign.douyinstatic.com/ies-music/pattern/fe8520e2ab7354d76b01049afbbd2b68.json?x-expires=1685008788&x-signature=%2BgQ450SirhF8OwqkNXgNUeuzhxg%3D"
                    ],
                    "width": 720
                },
                "tag_list": null,
                "title": "@央视新闻创作的原声",
                "unshelve_countries": null,
                "user_count": 0,
                "video_duration": 15
            },
            "nickname_position": null,
            "origin_comment_ids": null,
            "original_images": null,
            "packed_clips": null,
            "photo_search_entrance": {
                "ecom_type": 0
            },
            "position": null,
            "prevent_download": false,
            "promotions": [],
            "region": "CN",
            "series_paid_info": {
                "item_price": 0,
                "series_paid_status": 0
            },
            "share_info": {
                "share_link_desc": "8.92 EhO:/ 国士之心，祖国最懂！  %s 复制此链接，打开Dou音搜索，直接观看视频！",
                "share_url": "https://www.iesdouyin.com/share/video/6741899236838853901/?region=CN&mid=6741891852313692942&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1"
            },
            "share_url": "https://www.iesdouyin.com/share/video/6741899236838853901/?region=CN&mid=6741891852313692942&u_code=e82ji30edg86kc&did=MS4wLjABAAAAa78ZjnYyohUaeLCvsyMhDDaGhpEmJoaWxiHGcycY28sDS4OOY1Ux9R50f5IA6En7&iid=MS4wLjABAAAANwkJuWIRFOzg5uCpDRpMj4OX-QryoDgn-yYlXQnRwQQ&with_sec_did=1&titleType=title&from_ssr=1",
            "show_follow_button": {},
            "social_tag_list": null,
            "statistics": {
                "aweme_id": "6741899236838853901",
                "collect_count": 12657,
                "comment_count": 635349,
                "digg_count": 8481966,
                "play_count": 0,
                "share_count": 99279
            },
            "status": {
                "allow_share": true,
                "aweme_id": "6741899236838853901",
                "in_reviewing": false,
                "is_delete": false,
                "is_prohibited": false,
                "listen_video_status": 0,
                "part_see": 0,
                "private_status": 0,
                "review_result": {
                    "review_status": 0
                }
            },
            "text_extra": [],
            "uniqid_position": null,
            "user_digged": 0,
            "user_recommend_status": 0,
            "video": {
                "big_thumbs": [],
                "bit_rate": [
                    {
                        "FPS": 30,
                        "HDR_bit": "",
                        "HDR_type": "",
                        "bit_rate": 974423,
                        "gear_name": "normal_540_0",
                        "is_bytevc1": 0,
                        "is_h265": 0,
                        "play_addr": {
                            "data_size": 1892208,
                            "file_hash": "c7e779cfb5803ac92cb89d3b7127f641",
                            "height": 748,
                            "uri": "v0300f550000bm80j3lmuq8rag7sm380",
                            "url_key": "v0300f550000bm80j3lmuq8rag7sm380_h264_540p_974423",
                            "url_list": [
                                "http://v3-web.douyinvod.com/0bb360e95e68385cb131cf41f7027ce5/646dee33/video/tos/cn/tos-cn-ve-0015c800/220546bcb29de0646ef84e89b72c8e2a00d116383d8000007c314930e30b/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=951&bt=951&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDo4Z2Y8OjQ2ZTtlNDRmZEBpMzZ2anV0cDYzcDMzOGkzM0A0XjFeYDEzXjYxX2FiXzNiYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "http://v26-web.douyinvod.com/74b5a15dfb71a82074dbf8f252706e66/646dee33/video/tos/cn/tos-cn-ve-0015c800/220546bcb29de0646ef84e89b72c8e2a00d116383d8000007c314930e30b/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=951&bt=951&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDo4Z2Y8OjQ2ZTtlNDRmZEBpMzZ2anV0cDYzcDMzOGkzM0A0XjFeYDEzXjYxX2FiXzNiYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                                "https://www.douyin.com/aweme/v1/play/?video_id=v0300f550000bm80j3lmuq8rag7sm380&line=0&file_id=ea6cb1e1dbb84b93a16749ccad45a779&sign=c7e779cfb5803ac92cb89d3b7127f641&is_play_url=1&source=PackSourceEnum_FAVORITE"
                            ],
                            "width": 576
                        },
                        "quality_type": 20,
                        "video_extra": "{\"PktOffsetMap\":\"\"}"
                    }
                ],
                "bit_rate_audio": null,
                "cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/e06cb6999da2464a909accb887ee7454",
                    "url_list": [
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/e06cb6999da2464a909accb887ee7454~tplv-dy-cropcenter:323:430.jpeg?x-expires=2000278800&x-signature=B9WUIVweLfbvUF7v8NrLbEgBQKU%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=true&sh=323_430&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e06cb6999da2464a909accb887ee7454?x-expires=2000278800&x-signature=N%2BKE9fAIlmBSOajuYCr%2FcCDDy7c%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e06cb6999da2464a909accb887ee7454?x-expires=2000278800&x-signature=P5O48C0YIFwf%2FLcwuFLFcZlnJd4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/e06cb6999da2464a909accb887ee7454?x-expires=2000278800&x-signature=Os4Y1rV9BNEiDyYlhaGV9UG1Bn4%3D&from=3213915784&s=PackSourceEnum_FAVORITE&se=false&sc=cover&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "download_addr": {
                    "data_size": 2628731,
                    "height": 720,
                    "uri": "v0300f550000bm80j3lmuq8rag7sm380",
                    "url_list": [
                        "http://v3-web.douyinvod.com/b94945fd76960e1db8168f8e2f05cad6/646dee33/video/tos/cn/tos-cn-ve-0015c800/22081ffacc9f2204a3686d8524d7f802317116386f9000008f288cff23df/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1321&bt=1321&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDxpZ2c3OGY2OWU4aWY6aUBpMzZ2anV0cDYzcDMzOGkzM0BhX2EvNi0yXjMxYF41LWJeYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/08b7b85e0c4461113d2e757b67eaf82a/646dee33/video/tos/cn/tos-cn-ve-0015c800/22081ffacc9f2204a3686d8524d7f802317116386f9000008f288cff23df/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=1321&bt=1321&cs=0&ds=3&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=NDxpZ2c3OGY2OWU4aWY6aUBpMzZ2anV0cDYzcDMzOGkzM0BhX2EvNi0yXjMxYF41LWJeYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300f550000bm80j3lmuq8rag7sm380&line=0&ratio=540p&watermark=1&media_type=4&vr_type=0&improve_bitrate=0&biz_sign=NRPI1lC4AlkgB1YZ_o3JxvAfEXZOvePEcuDO_o4-J3GyX4FkG5hWx9kaoeyE9VaaOzLa7CA0Ou-V1V2BgFcWdNQR7kfNDGbNHaUZIZuaRMUGyO7s5wbVW7et0I2xsyVeH7OYijs=&logo_name=aweme&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 720
                },
                "duration": 15535,
                "dynamic_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/50390b41fb344605a321a1f970ce1dfd",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/obj/tos-cn-p-0015/50390b41fb344605a321a1f970ce1dfd?x-expires=1686128400&x-signature=F0idD9eegj%2FCOGPH4n9FDKDyAsY%3D&from=3213915784_large",
                        "https://p9-pc-sign.douyinpic.com/obj/tos-cn-p-0015/50390b41fb344605a321a1f970ce1dfd?x-expires=1686128400&x-signature=94h6B7STN5PEePzJXVTQqVnYITM%3D&from=3213915784_large",
                        "https://p3-pc-sign.douyinpic.com/obj/tos-cn-p-0015/50390b41fb344605a321a1f970ce1dfd?x-expires=1686128400&x-signature=CCf%2FlSio3ss%2BkF7QXZuGMlYzpbY%3D&from=3213915784_large"
                    ],
                    "width": 720
                },
                "height": 934,
                "is_h265": 0,
                "is_source_HDR": 1,
                "meta": "{\"qprf\":\"1.000\",\"sr_score\":\"1.000\"}",
                "origin_cover": {
                    "height": 720,
                    "uri": "tos-cn-p-0015/05d82d1b52734cc3be23bffcf08f9901",
                    "url_list": [
                        "https://p6-pc-sign.douyinpic.com/tos-cn-p-0015/05d82d1b52734cc3be23bffcf08f9901~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=otbTR12TDmxm5WTnQLDyxkJAXNM%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p3-pc-sign.douyinpic.com/tos-cn-p-0015/05d82d1b52734cc3be23bffcf08f9901~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=aZoJz2uVTagnHxZgjdIDwhaIA6M%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A",
                        "https://p9-pc-sign.douyinpic.com/tos-cn-p-0015/05d82d1b52734cc3be23bffcf08f9901~tplv-dy-360p.jpeg?x-expires=1686128400&x-signature=uXtAknFwAQrsfEqfFGRAdMW7q%2Bs%3D&from=3213915784&se=false&biz_tag=pcweb_cover&l=2023052417594788E1736391CF0E03184A"
                    ],
                    "width": 720
                },
                "play_addr": {
                    "data_size": 1892208,
                    "file_hash": "c7e779cfb5803ac92cb89d3b7127f641",
                    "height": 748,
                    "uri": "v0300f550000bm80j3lmuq8rag7sm380",
                    "url_key": "v0300f550000bm80j3lmuq8rag7sm380_h264_540p_974423",
                    "url_list": [
                        "http://v3-web.douyinvod.com/0bb360e95e68385cb131cf41f7027ce5/646dee33/video/tos/cn/tos-cn-ve-0015c800/220546bcb29de0646ef84e89b72c8e2a00d116383d8000007c314930e30b/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=951&bt=951&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDo4Z2Y8OjQ2ZTtlNDRmZEBpMzZ2anV0cDYzcDMzOGkzM0A0XjFeYDEzXjYxX2FiXzNiYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "http://v26-web.douyinvod.com/74b5a15dfb71a82074dbf8f252706e66/646dee33/video/tos/cn/tos-cn-ve-0015c800/220546bcb29de0646ef84e89b72c8e2a00d116383d8000007c314930e30b/?a=6383&ch=4&cr=3&dr=0&lr=all&cd=0%7C0%7C0%7C3&cv=1&br=951&bt=951&cs=0&ds=6&ft=ghDK67MgvvBQxgUE8yq8Z.C~xi4JImApI_QqES6BJE&mime_type=video_mp4&qs=0&rc=PDo4Z2Y8OjQ2ZTtlNDRmZEBpMzZ2anV0cDYzcDMzOGkzM0A0XjFeYDEzXjYxX2FiXzNiYSM1ajReNXJpZzVfLS0yLTBzcw%3D%3D&l=2023052417594788E1736391CF0E03184A&btag=e00010000",
                        "https://www.douyin.com/aweme/v1/play/?video_id=v0300f550000bm80j3lmuq8rag7sm380&line=0&file_id=ea6cb1e1dbb84b93a16749ccad45a779&sign=c7e779cfb5803ac92cb89d3b7127f641&is_play_url=1&source=PackSourceEnum_FAVORITE"
                    ],
                    "width": 576
                },
                "ratio": "540p",
                "video_model": "",
                "width": 720
            },
            "video_game_data_channel_config": {},
            "video_labels": null,
            "video_tag": [
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                },
                {
                    "level": 0,
                    "tag_id": 0,
                    "tag_name": ""
                }
            ],
            "video_text": null
        }
    ],
    "has_more": 1,
    "log_pb": {
        "impr_id": "2023052417594788E1736391CF0E03184A"
    },
    "max_cursor": 1596461485000,
    "status_code": 0
}
  </code>
 </pre>
</details>


## 8.抖音主页手机
```
/dy/user/phone
```
### 参数:
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|
|encryStr|string|是|主页信息encrypt_mobile参数|

<details> 
 <summary><font size="4" color="orange">查看返回数据</font></summary> 
 <pre>
  <code class="language-cpp">
    {
      "code": "0",
      "mobile": "12345678910"
    }

  </code>
 </pre>
</details>



## 其他
### 调用次数/剩余次数查询
```
/user/reqCount
```
|参数名|类型|必选|说明|
|--|:--:|:--:|:--|
|token|string|是|访问凭证|


```
有任何问题可交流学习  
请勿使用本服务于商用   
请勿使用本服务大量抓取   
若因使用本服务与平台造成不必要的纠纷，本人盖不负责  
本人纯粹技术爱好，若侵犯贵公司的权益，请告知  
```

<!-- 有需要的[联系QQ45497494](https://qr.api.cli.im/newqr/create?data=https%253A%252F%252Fqm.qq.com%252Fcgi-bin%252Fqm%252Fqr%253Fk%253DgsXU_14bQsI8BdSevrFzHU7vIYnRCnFQ%2526noverify%253D0&level=H&transparent=false&bgcolor=%23FFFFFF&forecolor=%23000000&blockpixel=12&marginblock=1&logourl=&logoshape=no&size=500&kid=cliim&key=211db538a2ba8c28441f5d952fe165db?#pic_center =300x) -->
联系QQ:45497494
<img src="https://qr.api.cli.im/newqr/create?data=https%253A%252F%252Fqm.qq.com%252Fcgi-bin%252Fqm%252Fqr%253Fk%253DgsXU_14bQsI8BdSevrFzHU7vIYnRCnFQ%2526noverify%253D0&level=H&transparent=false&bgcolor=%23FFFFFF&forecolor=%23000000&blockpixel=12&marginblock=1&logourl=&logoshape=no&size=500&kid=cliim&key=211db538a2ba8c28441f5d952fe165db" width="50%">

~~### 另有[小红书](https://github.com/canglingzhiyue/xiaohongshu)数据采集~~
~~### [拼多多](https://github.com/canglingzhiyue/pdd)数据接口~~
