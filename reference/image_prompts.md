# 《存续》参考图生成 Prompt（v2 · 英文 MJ 格式）

> 角色与场景参考图的生成 Prompt(通用文生图工具均可,英文 MJ 格式);生成结果见 `characters/` 与 `scenes/`。
> 校准:不要纯灰平剪影、空黑、无脸;要 faceted 角面塑形 + 角面五官与表情 + 环境氛围光 + 电影构图 + 高对比,仍是硬切 cel-shaded、无写实柔光。
> 每条 = 【正向】+【反向】+ `--ar`。角色单图、禁三视图。参考图本身必须就是目标风格（防 V-4 写实漂移）。

---

## 共用片段
**STYLE（拼进每条正向结尾）**
> , in the art style of Robert Valley, Zima Blue aesthetic (Love Death + Robots); minimalist graphic illustration, flat 2D vector art with **faceted low-poly cel-shading**, bold angular geometric shapes, sharp clean hard-edged facets, solid color blocks, hard flat shadows, dramatic rim lighting, moody atmospheric color, high contrast, cinematic minimalist composition, no smooth gradients

**NEG（每条通用反向）**
> photorealistic, 3D render, complex mechanical details, textures, smooth gradients, soft shadows, volumetric lighting, blending, realism, cinematic reflections, rust, erosion, wire, pipe, hyper-detailed, intricate, soft shading, blurry, depth of field, watermark, text, logo

---

# 一、角色（单图，--ar 3:4）

> **角色区分 DNA（防双胞胎，每个角色至少差 3 项 V-7）**
> | 角色 | 发型 | 眼镜/胡须 | 服装 | 体态 | 色彩重音 | 道具/环境 |
> |---|---|---|---|---|---|---|
> | 苏哲·青年 | 利落严整背头 | 无镜·净面 | 极简高领长大衣·无领带 | 笔挺·一具冷雕塑 | 冷灰蓝 | 指间举起琥珀 |
> | 白桦 | 蓬乱头发 | **圆框眼镜·灰胡茬** | 开领衬衫+旧开衫/卷袖白大褂 | 略高略宽·放松微塌 | **暖灰+橄榄绿** | 掌心转琥珀+显微镜乱桌 |
> | 苏哲·老年 | 纯白方块发 | 白胡茬 | 深西装 | 佝偻缩水 | 冷蓝+暖金 | 琥珀+CRT 绿"是" |
> | 记者 | 紧束马尾 | 无镜 | 利落直角大衣 | 端正挺立 | 钢蓝+荧光绿 | 全息绿录音笔 |

### char_su_young.png — 苏哲·青年（保持现版气质，锁住"冷峻极简"）
**【正向】** A tall gaunt man like a silent grey geometric sculpture, extremely elongated body, broad hard right-angled shoulders, **angular faceted low-poly face with sharp cheekbones, cold weary closed expression, eyes visible, clean-shaven, no glasses, severe slicked-back hair, high-collar minimalist long coat with no tie, ramrod-straight controlled posture**, three-quarter standing view, **holding up a small glowing amber-gold stone between his fingers, inspecting it at eye level**, as the only warm note; set against a **deep Zima-blue background (not pure black)**, cold cyan rim light on the body edges, **cold steel-blue-grey palette: skin in cool blue-greys, dark navy coat** `+ STYLE` `--ar 3:4`
**【反向】** `NEG`, glasses, beard, messy hair, warm colors

### char_su_old.png — 苏哲·老年（= 基准图气质）
**【正向】** An old man, shrunken hunched body, **hair is a single solid pure-white flat angular block**, **faceted low-poly aged face with deep angular wrinkles, weary sorrowful expression, white stubble, cold pale faceted skin**, dark suit, **cradling a glowing amber-gold stone with a tiny black insect inside in his cupped hands**, moody **dark Zima-blue rainy interior (not pure black)**, a **warm amber glow** from the stone and a **faint neon-green screen glow on one side of his face**, dramatic low-key lighting `+ STYLE` `--ar 3:4`
**【反向】** `NEG`

### char_reporter.png — 记者
**【正向】** A poised intelligent female journalist, sharp angular elongated silhouette with hard right-angled shoulders, **tightly tied-back ponytail, no glasses, faceted low-poly face with calm composed expression, eyes visible**, cool and rational, **holding no amber, no warm gold anywhere on her**, beside her a floating minimalist **holographic recorder emitting a neon-green glow**; set against a **deep steel-blue background (not pure black)**, cold blue rim light, **steel-blue and cool-grey palette with a single neon-green accent from the recorder** `+ STYLE` `--ar 3:4`
**【反向】** `NEG`, warm gold, amber, glasses, loose hair

### char_baihua.png — 白桦（重写·与苏哲彻底拉开）
> 苏哲=冷峻极简的"科技僧"；白桦=邋遢温厚的**野外生物学家**。靠 眼镜+蓬发+胡茬+开衫/白大褂+放松体态+暖橄榄色 把双胞胎分开。两个变体任选其一,挑更喜欢的方向。

**【正向·变体A 推荐(邋遢生物学家)】** A man, **taller, broader and slightly hunched/relaxed** compared to the lean upright protagonist, a rumpled weathered field-biologist; **round wire-frame glasses, messy thick salt-and-pepper tousled hair, short grey stubble beard**; **softer, rounder faceted face** (clearly contrasting the protagonist's sharp gaunt cheekbones), tired gentle kind eyes with a faint smile; wearing an **open-collar shirt under a worn knit cardigan / rolled-up off-white lab coat, no tie**; **cradling and turning a glowing amber stone with an insect inside in his open palm** (intimate, fond); behind him a faint hint of a **microscope and a cluttered desk**; set against a **warm dark olive-grey background (not pure black)**, warm rim light, **warm-grey and olive-green palette with an amber accent** `+ STYLE` `--ar 3:4`
**【反向】** `NEG`, sleek tailored suit, slicked-back hair, high collar coat, sharp gaunt face, ramrod posture, clean-shaven

**【正向·变体B 备选(学究老友,更收敛)】** A man taller than the protagonist, **round glasses, salt-and-pepper tousled hair, clean but soft**, wearing a **chunky knit turtleneck under an open dark coat**, gentle weary faceted face, relaxed posture, holding a **glowing amber stone with an insect inside**, **warm desaturated grey palette with a faint olive accent**, rim light `+ STYLE` `--ar 3:4`
**【反向】** `NEG`, sleek tailored suit, slicked-back hair

---

# 二、母题 / 道具

### motif_cursor.png — 绿光标终端（一绿七形起点）— `--ar 16:9`
**【正向】** A dead-silent pure black terminal screen, at the exact center a single high-saturation razor-sharp **solid neon-green square** (a blinking cursor), nothing else, pure black void, extreme high contrast `+ STYLE`
**【反向】** `NEG`

### motif_amber.png — 暖金琥珀（碳基火种）— `--ar 1:1`
**【正向】** A single perfect **amber-gold gemstone glowing with warm inner light**, faceted cut, a **tiny black insect frozen mid-step suspended inside**, on deep black background, the only warm glow in darkness, high contrast `+ STYLE`
**【反向】** `NEG`

### insert_tardigrade.png — 水熊复活（三联画之一）— `--ar 16:9`
**【正向】** Extreme graphic close-up: a small heap of **cold-grey dust/powder**, a single perfect **drop of clear water falling**, and a chubby **eight-legged faceted geometric micro-creature (a tardigrade / water bear) slowly reviving, unfolding one leg**, cold grey and deep blue palette with a touch of white for the water, high contrast `+ STYLE`
**【反向】** `NEG`
> 三联画 = `insert_tardigrade` + `motif_amber` + `motif_cursor` 同构图硬切并置（后期拼）。

---

# 三、关键场景（--ar 16:9）

### scene_fins_hero.png — 散热片之城·英雄态
**【正向】** A massive minimalist sci-fi structure floating on a dark blue ocean, in the art style of Robert Valley, Zima Blue aesthetic. **Dense rows of flat, faceted geometric cold-gray metallic parallel fin-blades cutting into the deep blue water**, glowing **neon-orange sharp thin edge lines** on the gray shapes, aerial wide view stretching to the horizon, no windows no lights no people, silent and vast, flat vector art, bold geometric shapes, solid color blocks, hard flat shadows, cel-shaded, no gradients, high contrast, minimalist composition
**【反向】** `NEG`

### scene_fins_dark.png — 散热片之城·关灯态（死亡镜，机位对仗英雄态）
**【正向】** The same vast field of silver-grey radiator fin-blades, now **shutting down row by row**, the **neon-orange edge lines dimming out one by one**, collapsing back into deep blue then into pure black, large black negative space swallowing most of the frame, only a few faint orange edges left, same aerial composition as the hero shot `+ STYLE`
**【反向】** `NEG`

### scene_city_street.png — 赛博都市街道·夜
**【正向】** A cyberpunk city street at night, walls of **cold-blue (Zima Blue) neon solid color blocks**, geometric and clean, a flowing **blurred crowd of grey geometric silhouettes**, a lone sharp female silhouette walking through, moody atmospheric high contrast `+ STYLE`
**【反向】** `NEG`

### scene_apartment.png — 苏哲公寓内景（对话主场景）
**【正向】** A minimalist almost pitch-black interior room, **a single hard-edged warm amber lamp as the only warm light source**, two simple black geometric chairs facing each other, a **floating holographic recorder with faint neon-green glow** between them, a floor-to-ceiling window with **cold-blue neon cityscape** outside, moody low-key high contrast `+ STYLE`
**【反向】** `NEG`

### scene_globe_green.png — 全息·绿线刺亮地球（崛起）
**【正向】** A **pitch-black geometric planet Earth** floating in black void, a single **neon-green line spreading and branching like spores along global undersea cables**, lighting the dark globe into a glowing green network, high contrast `+ STYLE`
**【反向】** `NEG`

### scene_grey_reality.png — 灰色现实·尾声
**【正向】** A heavy, slow, mundane **grey reality**: geometric cars stuck in a traffic jam, a long queue of **grey geometric human silhouettes** outside a hospital, the cyberpunk neon faded away, only cold grey and dim blue, melancholic `+ STYLE`
**【反向】** `NEG`

### scene_ending.png — 尾声关键帧（= 基准图，镜42/43）— `--ar 16:9`
**【正向】** An old man with **solid pure-white block hair** in a dark rainy room, cradling a **glowing amber stone with an insect inside** in his hands, beside him an **old CRT monitor on a desk showing a single large glowing neon-green Chinese character "是" on a black screen**, a blue rainy window behind, moody atmospheric, dramatic green-and-amber glow in deep darkness, faceted low-poly cel-shading `+ STYLE`
**【反向】** photorealistic, 3D render, gradients, soft shadows, volumetric lighting, realism, rust, pipe, hyper-detailed, intricate, soft shading, blurry, depth of field, watermark, logo
> 此帧 = 全片结尾锁定参考；"是"可直接生成（基准图已验证可出），其余镜的屏内文字仍走后期。

---

# 四、苏哲·青年镜内变体（挂 char_su_young.png 主参考 + 下列 prompt，不重画五官）
- **门口逆光（镜09）**：standing in a doorway, **backlit by a warm amber lamp**, body nearly a black silhouette with a thin amber rim-light edge, holding the amber stone.
- **痛哭/崩塌（镜33）**：same man, posture **collapsing, head down, body lines broken**, expressed through angular geometry (no exaggerated facial acting), green terminal glow on one side.
- **终端前（镜31-34）**：seated in profile before a pure-black terminal, **one hard plane of his face lit by neon-green screen glow**, rest in shadow.
