能够用到的 Anim 的枚举常量有两类
## ANIM_TWEEN

ANIM_TWEEN.LINEAR

ANIM_TWEEN.SINE

ANIM_TWEEN.QUAD

ANIM_TWEEN.CUBIC

ANIM_TWEEN.QUART

ANIM_TWEEN.QUINT

ANIM_TWEEN.EXPO

ANIM_TWEEN.CIRC

ANIM_TWEEN.BACK

ANIM_TWEEN.ELASTIC

ANIM_TWEEN.BOUNCE

## ANIM_EASE

ANIM_EASE.IN

ANIM_EASE.OUT

ANIM_EASE.IN_OUT

## 用法

详情可以参考网站：[缓动参考](https://easings.net/zh-cn)

当然，你也可以直接查看以下的页面：

<iframe src="https://easings.net/zh-cn" width="100%" height="500" frameborder="0">
</iframe>

如果我们需要使用 `easeInQuad` 效果，那么我们在运行 `Anim_Create` 的时候只需要调用 `ANIM_TWEEN.QUAD` 和 `ANIM_EASE.IN`。

请注意：效果名和实际代码编写是反过来的，若效果名里先是 `In`，后是 `Quad`。那么在编写代码时就需要先写 `ANIM_TWEEN.QUAD`，后写 `ANIM_EASE.IN`。