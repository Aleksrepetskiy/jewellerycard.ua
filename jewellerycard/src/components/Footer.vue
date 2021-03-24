<template>
	<footer class="footer">
		<div class="wrapper">
			<div class="footer__box footer__contacts">
				<div class="relations">
					<div class="relations__item">
						<a href="tel:+380442353916" class="relations__link"><span class="icon icon-phone"></span>+380442353916</a>
					</div>
					<div class="relations__item">
						<a href="mailto:inquiries@jewellerycard.ua" class="relations__link"><span class="icon icon-mail"></span>inquiries@jewellerycard.ua</a>
					</div>
				</div>
			</div>
			<div class="footer__box footer__logo">
				<img src="/img/svg/logo-footer.svg?v=1" alt="logo-footer">
			</div>
			<div class="footer__box footer__copyrating">
				© 1999 Jewellery Card
			</div>
			<div class="to-top" style="display: block;">
				<div class="to-top__img">
					<img src="/img/totopNormal.png" alt="">
				</div>
			</div>
		</div>
	</footer>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    msg: String
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>