# 说明

内部原生 js 实现，可支持跨框架引用，包括倒计时动效。可自定义红包图片倒计时时长等;

# 使用方式

引入：
`import RedEnvelopeRainAnimation from 'red-envelope-rain-animation';`

需要调用的地方 定义关于红包雨的参数，实例化红包雨类，传入红包雨完毕后的回调处理函数
`	let params = {配置参数};
	let rwr = new RedEnvelopeRainAnimation(params);
	rwr.start((redPacketsCount) => {
		// console.log('回调红包个数', redPacketsCount);
	});
`

# 可传入参数说明

    #space = 300; // 生成红包间隔  最小300
    #speed_max = 5; // 红包下落速度随机值__最大值
    #speed_min = 1; // 红包下落速度随机值__最小值
    #red_img_src = ''; //红包图片
    #red_img_ratio = 1; // 红包宽高比例
    #duration = 5; // 红包雨下落时长
    #activityTheme = '红包'; // 活动主题
