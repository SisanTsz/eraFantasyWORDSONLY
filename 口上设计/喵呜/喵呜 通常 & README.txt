;玛雯口上试作
;README部分

;人物性格
;猫娘，实际上是从学院里跑出来的融合试验品，
;初始白色短袖短裤，橙色头发黑色挑染，猫耳猫尾，裸足裸手，中期会逐渐喜欢打扮，身着变成浅蓝水手服裙。
;好感度逐渐提升后，渐渐开始学会一些单词，最终学会和你交流
;口上里所有“陷落”指恋慕or爱慕or拜倒or献身or奉献or浸淫or情欲or情迷or淫欲or隶属or服从or仰慕or狂乱之一
;其中基础陷落素质为恋慕/拜倒/奉献/情欲，二级陷落素质为爱慕/献身/浸淫/情迷，进阶陷落素质为淫欲/隶属/服从/仰慕，最终获得狂乱
;个人喜好问题，不写粪相关以及血腥内容，可自行加笔
;
;更新日志:
;20240604 - 开写
;
;
;
;
;
;
;
;
；
；
;To Do List：
;总之慢慢填吧……



;互动 
	;对话（任意,满足要求的都可以选择其一显示）
		IF 狂乱
		PRINTFORMW 【作为猫来看……人类的社会真是复杂喵……规矩好多，还是当一只家猫最好了】
		or
		PRINTFORMW 【在主人的身边确实感觉轻松很多喵……无论是气味，还是暖暖的怀抱……都喜欢喵】
		or
		PRINTFORMW 【太阳充足的时候，正是暖暖和和，适合睡觉的时间喵。雨天？出门毛都要沾湿了，也是在家睡觉的好时间喵。】
		OR
		PRINTFORMW 【主人的事，如果我能多分担一些就好了喵……要学习的喵？那还是算了喵。】
		ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
		PRINTFORMW 【能再讲一次那个故事吗？就是把我捡到那天的故事喵！】  
		or
		PRINTFORMW 【还是不喜欢衣服……磨着身体，有点难受喵……】
		or
		PRINTFORMW 【呜哇！别用黄瓜吓我啊喵。】
		ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
		PRINTFORMW 【喜欢吃肉喵！多要多要！】
		or 
		PRINTFORMW 【主人喝的那个冒气的东西我也能尝一下嘛？谢谢主人！嘶……呜哇好烫！好苦喵！我不要喝啦喵！】
		or 
		PRINTFORMW 【来和喵呜聊天吧，只要喵呜知道，什么都会教给主人哦！无论是是抓鸟，还是抓蝴蝶，还是……什么论宇宙……飞行器……不懂啦喵！不要刁难我啦喵！】
		ELSEIF 恋慕 or 拜倒 or 奉献 or 情欲
		PRINTFORMW 【抱抱~喵~】
		or
		PRINTFORMW 【嗅嗅~呼噜~】
		or
		PRINTFORMW 【哈欠……好困……】
		ELSE 无陷落
		PRINTFORMW 【喵？】
		or
		PRINTFORMW 【咕呜~prpr~】
		or
		PRINTFORMW 【呼噜呼噜~】	
		;约会聊天（以下只有约会时候显示）
		IF 狂乱
		PRINTFORMW 【虽然不喜欢人多的地方，但是和主人牵着手走路，就感觉充满了勇气喵。】
		or
		PRINTFORMW 【那个摊子……好像很香喵！不去看吗？不去看看喵？】
		or
		PRINTFORMW 【那里有蝴蝶，看我扑住它……看我扑到啦，可以带我去吃那个喵？】
		ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
		PRINTFORMW 【看，主人，那里有鸽子喵！看我抓一只过来……不行吗喵？】 
		or
		PRINTFORMW 【腋窝，还有大腿，还有屁股上都痒痒的喵，想要舔舔喵……不能吗喵？】
		or
		PRINTFORMW 【那个飞起来的，是叫气球喵，怎么飞起来的喵？知道啦，不会用爪子的喵！】
		ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
		PRINTFORMW 【牵手……嘻嘻……】 
		or
		PRINTFORMW 【那个，想要……喜欢吃柔……rou……肉！喵！】
		or
		PRINTFORMW 【出来玩！很开心喵！】
		ELSEIF 恋慕 or 拜倒 or 奉献 or 情欲 or 无陷落
		PRINTFORMW 【喵？】
		or
		PRINTFORMW 【咕呜~prpr~】
		or
		PRINTFORMW 【呼噜呼噜~】	
	;抱抱
		;恋爱线
		IF 恋慕
		PRINTFORMW 【主人……身边……卵卵和和的……】
		PRINTFORMW 不容你分说，喵呜直接钻进了你的怀抱里，喉咙里发出了开心的呼噜声
		ELSEIF 爱慕
		PRINTFORMW 【主人……在一起……喜欢……】
		PRINTFORMW 不容你分说，喵呜直接钻进了你的怀抱里，粗糙的舌头刮着你的皮肤，仿佛在为你梳毛一般
		ELSEIF 拜倒 or 仰慕
		PRINTFORMW 【主人，喵呜喜欢抱抱~要抱抱~】
			IF MASTER是女性 or 扶她
			PRINTFORMW 不容你分说，喵呜撒娇着，直接钻进了你的怀抱里，像是刚出生的小猫一样，不自觉揉按起了你胸前的柔软。
			ELSE
			PRINTFORMW 不容你分说，喵呜撒娇着，直接钻进了你的怀抱里，像是刚出生的小猫一样，不自觉揉按起了你柔软的腹部。
		;淫乱线
		ELSEIF 情欲
		PRINTFORMW 【主人……痒……蹭蹭……】
		PRINTFORMW 不容你分说，喵呜直接钻进了你的怀抱里，双腿无意识的夹住你的大腿，不断磨蹭。		
		ELSEIF 情迷
		PRINTFORMW 【主人……味道……喵呜喜欢……】
		PRINTFORMW 不容你分说，喵呜直接钻进了你的怀抱里，嘴巴含住着你的手指啧啧吮吸起来
		ELSEIF 淫欲 or 浸淫
		PRINTFORMW 【喵呜，下面好痒喵……闻到主人的气味就……】
		PRINTFORMW 喵呜趴在你的怀里，直接把你的手夹进她的双腿之间，不断蹭弄起来
		ELSEIF 狂乱
		PRINTFORMW 【嘿嘿，我来啦喵~咕噜咕噜~】
		PRINTFORMW 终于学会人类的语言和习俗的喵呜直接冲进了你的怀里，肉肉的脸颊在你胸口磨蹭，两个尖尖的猫耳朵不停戳着你的下巴。
		ELSEIF 隶属 or 服从 or 献身 or 奉献
		PRINTFORMW 你抱起呜喵，手放在了尖尖的猫耳朵之间，揉搓起来。 
		PRINTFORMW 喵呜虽然没有反抗，但是也不像是很喜欢你的抱抱，只是静静接受了你的抚摸。
		ELSE 无陷落
		PRINTFORMW 你抱起呜喵，慢慢地给她梳起了头发。 
		PRINTFORMW 喵呜虽然没有直接反抗，但是也不像是很喜欢你的抱抱，在你的怀里不停的乱动。





	;拉去隐秘的地方
	;送礼
		IF 狂乱
		PRINTFORMW 【这朵些是给我的吗？嘶哈……好香啊！谢谢主人，我会好好养的！】 
		PRINTFORMW 喵呜很开心的抱着你给她的东西————一捧鲜花。圆圆的脸蛋埋在花丛中，嘴角勾起甜美的笑容
		PRINTFORMW 喵呜已经和一个普通人别无二致，无论是行为还是思维————当然前提是要忽略头顶上因为喜悦而抖动的猫耳朵。
		ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
		PRINTFORMW 【这个给我嘛？谢谢喵！】 
		PRINTFORMW 喵呜很开心的抱着你给她的东西————一个橡皮老鼠，却没有像以前那样直接玩起来，而是抱在胸口。
		PRINTFORMW 喵呜的进步很快，似乎很快就能融入人类了。		
		ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
		PRINTFORMW 【给我？能……吃？不能喵？】 
		PRINTFORMW 喵呜很开心的抱着你给她的东西————一个铃铛，然后出乎你意料的咬了一口，发现咬不动后大大的眼睛里反射出了大大的疑惑。
		PRINTFORMW 喵呜已经逐渐理解了人类的行为，虽然还不太准确。
		ELSEIF 恋慕 or 拜倒 or 奉献 or 情欲
		PRINTFORMW 【喵？】
		PRINTFORMW 喵呜看着你的礼物————一个玻璃球，扒拉了一下，似乎觉得很好玩，又开始追逐起来。
		PRINTFORMW 看来还需要教她很多人类的行为呢。
		ELSE 无陷落
		PRINTFORMW 【……？】
		PRINTFORMW 喵呜扒拉着你给她的礼物————一双拖鞋。但她似乎对礼物没兴趣，而是对装拖鞋的纸袋更感兴趣，直接把脑袋钻了进去。
		PRINTFORMW 猫的习性还很严重，需要进一步的观察吧。

	;摸头
	;膝枕
;性骚扰
	;摸屁
	;摸腿
	;摸脚
	;掀裙子
	;接吻
		
	;摸胸
	;手指插入
	;摸菊
	;


;约会
	;约会选择地点后显示
	IF 有陷落
		在银行
		PRINTFORMW 【	】
		书店
			IF 狂乱
			PRINTFORMW 【上次买的书？还没看完喵，好难懂喵……】
			ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
			PRINTFORMW 【书，不喜欢喵……书上面有好多字……】
			ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
			PRINTFORMW 【书，看不懂喵……这里不要吗喵……】
			ELSE 恋慕 or 拜倒 or 奉献 or 情欲 or 无陷落
			PRINTFORMW 【喵呜……（沮丧）】

		神殿
			IF 狂热
			PRINTFORMW 【很安静的地方喵。】
			ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
			PRINTFORMW 【】
			ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
			PRINTFORMW
			ELSEIF 恋慕 or 拜倒 or 奉献 or 情欲
			PRINTFORMW
			ELSE 无陷落
			PRINTFORMW
		道具店
			IF 狂热
			PRINTFORMW 【需要买东西嘛喵？喵呜帮主人一起提！】
			ELSEIF 淫欲 or 隶属 or 服从 or 仰慕
			PRINTFORMW 【】
			ELSEIF 爱慕 or 献身 or 浸淫 or 情迷
			PRINTFORMW
			ELSEIF 恋慕 or 拜倒 or 奉献 or 情欲
			PRINTFORMW
			ELSE 无陷落
			PRINTFORMW

		饭店
			IF 未陷落 OR 献身 OR 隶属 OR 奉献 OR 服从 or 恋慕 or 情欲
			PRINTFORMW 【一直以来我要求的，就只有能够填饱肚子这一条，所以一直以来都吃的方便口粮，热量又大，饱腹感又高，不过细想来美味度肯定是不如新鲜现做的啦。所以看你吃什么，我和你吃一样的就行，要是还有肉吃就最好啦。】
			ELSE 爱慕 OR 情迷 OR 拜倒 OR 浸淫 OR 淫欲 OR 仰慕 OR 狂热
			PRINTFORMW 【这道菜味道可真好！再多吃几口的话，怕是以后那些方便口粮就再也入不了口了啊。】
		公园
		PRINTFORMW 【】
		服饰店
		PRINTFORMW
		社会事务管理中心
		PRINTFORMW
		PRINTFORMW
		星际开拓事业管理中心
		PRINTFORMW
		PRINTFORMW
		魔导科学院
		PRINTFORMW
			
	ELSE 无陷落
	PRINTFORMW 【喵？】
	;牵手
		IF 恋慕 or 情欲
		PRINTFORMW 【不要一下子就摸过来啊！给……给你牵就是了……】
		ELSEIF 爱慕 OR 情迷 OR 拜倒 OR 浸淫 OR 淫欲 OR 仰慕
		PRINTFORMW 【之前都没意识到，原来Boss的手是这么大的吗……很温暖……】
		ELSEIF 狂热
		PRINTFORMW 【再多握一会嘛。手心好温暖，好怀念……】
		ELSEIF 初次 && 未陷落
		PRINTFORMW 【多大人了，还要拉手啊？害不害羞啊。】
		ELSEIF 未陷落 OR 献身 OR 隶属 OR 奉献 OR 服从
			IF男性
			PRINTFORMW 【……行吧，也习惯了。】
			ELSE 女性 or 扶她
			PRINTFORMW 【之前不知道，你这手保养得还可以嘛……】
	
	;休息
IF 恋慕 or 情欲
		PRINTFORMW 【不要一下子就摸过来啊！给……给你牵就是了……】
		ELSEIF 爱慕 OR 情迷 OR 拜倒 OR 浸淫 OR 淫欲 OR 仰慕
		PRINTFORMW 【之前都没意识到，原来Boss的手是这么大的吗……很温暖……】
		ELSEIF 狂热
		PRINTFORMW 【再多握一会嘛。手心好温暖，好怀念……】
		ELSEIF 献身 OR 隶属 OR 奉献 OR 服从
		PRINTFORMW 【……牵吧】
		ELSEIF 初次 && 未陷落
		PRINTFORMW 【多大人了，还要拉手啊？害不害羞啊。】
		ELSEIF 未陷落 
			IF男性
			PRINTFORMW 【……行吧，也习惯了……大男人走路还需要牵别人的手吗？搞不懂。】
			ELSE 女性 or 扶她
			PRINTFORMW 【之前不知道，你这手保养得还可以嘛……】	
	;请吃饭
		;同饭店内容
		IF 未陷落 OR 献身 OR 隶属 OR 奉献 OR 服从 or 恋慕 or 情欲
		PRINTFORMW 【一直以来我要求的，就只有能够填饱肚子这一条，所以一直以来都吃的方便口粮，热量又大，饱腹感又高，不过细想来美味度肯定是不如新鲜现做的啦。所以看你吃什么，我和你吃一样的就行，要是还有肉吃就最好啦。】
		ELSE 爱慕 OR 情迷 OR 拜倒 OR 浸淫 OR 淫欲 OR 仰慕 OR 狂热
		PRINTFORMW 【这道菜味道可真好！再多吃几口的话，怕是以后那些方便口粮就再也入不了口了啊。】		
	;请洗澡
		IF 未陷落 OR 献身 OR 隶属 OR 奉献 OR 服从 or 恋慕 or 情欲
		PRINTFORMW 【一直以来我要求的，就只有能够填饱肚子这一条，所以一直以来都吃的方便口粮，热量又大，饱腹感又高，不过细想来美味度肯定是不如新鲜现做的啦。所以看你吃什么，我和你吃一样的就行，要是还有肉吃就最好啦。】
		ELSE 爱慕 OR 情迷 OR 拜倒 OR 浸淫 OR 淫欲 OR 仰慕 OR 狂热
		PRINTFORMW 【这道菜味道可真好！再多吃几口的话，怕是以后那些方便口粮就再也入不了口了啊。】				
	;去情人旅馆



;陷落特质获得
		恋慕
		PRINTFORMW 【不知不觉，就想一直待在Boss身边呢……】
		爱慕
		PRINTFORMW 【好想和你就这么拥抱着，24小时不分开……】
		拜倒
		PRINTFORMW 【一切都放心交给我吧……无论是商业，还是爱情，还是……】
		献身
		PRINTFORMW 【……是，我可以的。】
		奉献
		PRINTFORMW 【为了BOSS您……我什么都会做的……】
		浸淫
		PRINTFORMW 【那种欲望的处理……我……我也可以……】
		情欲
		PRINTFORMW 【……】（身体不停扭动）
		情迷
		PRINTFORMW 【这样的感觉……或许还不错……】
		淫欲
		PRINTFORMW 【看到BOSS，身体就会不停发热……】
		隶属
		PRINTFORMW 【您有何吩咐？】
		服从
		PRINTFORMW 【我会全力为您服务。】
		仰慕
		PRINTFORMW 【能为您做事，是我的荣幸。】
		狂乱
		PRINTFORMW 【嘿嘿，抓住你啦！这可是如家人般充满爱意的拥抱哦！这样，就不会再消失掉吧……对吗？】

