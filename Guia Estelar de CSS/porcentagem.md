As porcentagens são valores bem flexíveis
Em muitos casos é tratado da mesma maneira que as distâncias <length>
Sempre será relativo a algum valor
# Exemplo
Relativo ao elemento pai

<ul>
	<li>One</li>
	<li>Two</li>
	<li>Three
		<ul>
			<li>Three A</li>
			<li>Three B</li>
			<ul>
				<li>Three B 2</li>
			</ul>
		</ul>
	</li>
</ul>
li {
    font-size: 80%;
}
