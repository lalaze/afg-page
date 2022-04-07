<script>

export let tab = 0

function goto(url) {
	window.href = url
}

</script>

<main style={'background-image: url(./bg.jpeg);'}>
	<div class="glass">
		<div class="nav">
			<div>
				<img src="./logo.jpg" class="logo" alt="" />
			</div>
			<div class="{tab === 0 ? 'active' : ''}">首页</div>
			<div class="{tab === 1 ? 'active' : ''}">帮助文档</div>
		</div>
		<div class="back">返回web页</div>
		<div class="title">AFG论坛</div>
		<div class="title2">Android论坛已开放下载</div>
		<div class="content">
			<div class="card" on:click={goto('https://wws.lanzouh.com/i6fnm02qyc2h')}>
				<div class="lanzou"></div>
				<div>蓝奏云下载</div>
				<div class="bottom">密码：afg</div>
			</div>
			<div class="card" on:click={goto('https://pan.baidu.com/share/init?surl=CubKvbBr2hP6zrKNHzDUkQ')}>
				<img src="./baiduyun.png" class="img" alt="" />
				<div>百度云下载</div>
				<div class="bottom">密码：afg1</div>
			</div>
		</div>
	</div>
</main>