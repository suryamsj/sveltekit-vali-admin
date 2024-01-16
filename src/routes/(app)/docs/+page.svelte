<script>
	import AppTitle from '$lib/components/AppTitle.svelte';
</script>

<svelte:head>
	<title>Documentation - Vali Admin</title>
</svelte:head>

<AppTitle title="Documentation" desc="Documentation of vali admin" iconTitle="bi bi-code-square" />

<div class="tile">
	<div class="tile-body">
		<div class="docs" style="max-width: 700px;">
			<h2 class="docs-title">Directory Structure</h2>
			<pre class="directory-structure">│
├── docs - <i>compiled files</i>
│   ├── css
│   ├── images
│   └── js
└── src - <i>Layout and style source files</i>
&nbsp;&nbsp;&nbsp;&nbsp;├── pug - <i>Layout source</i>
&nbsp;&nbsp;&nbsp;&nbsp;└── sass - <i>Style source</i>
</pre>
			<h2 class="docs-title" id="Compilation-of-source-files">Compilation of source files</h2>
			<p>
				The theme is built using SASS and PugJs which are in turn compiled into HTML and CSS by
				Grunt. If you are not familiar with Grunt, <a
					href="https://24ways.org/2013/grunt-is-not-weird-and-hard/"
					target="_blank"
					rel="noopener">here</a
				> is an article to get started. If you are familiar with Grunt follow the instruction mentioned
				bellow to edit or customize the source.
			</p>
			<p>
				If you don't want to edit theme you can use the compiled files directly inside <code
					>docs</code
				> folder.
			</p>
			<p>
				Run <code>npm install</code> command in project root directory to install and build dependencies.
			</p>
			<p>
				Use <code>npm run dev</code> task to edit and compile source files on the go or use
				<code>npm run build</code> task to compile all source files at once.
			</p>
			<h2 class="docs-title" id="Layout-Customization">Layout Customization</h2>
			<p>
				The layout is built using PugJs. All the layout source files are located in <code
					>src/pug</code
				> directory. There are two sub directories inside this directory:
			</p>
			<ol>
				<li>
					<code>layout</code> - Includes common HTML skeleton layout which is extended by all the pages
				</li>
				<li><code>includes</code> - Includes layout partials like sidebar and navbar and footer</li>
			</ol>
			<h2 class="docs-title" id="Style-Customization">Style Customization</h2>
			<p>
				The styles are written in SASS. All the style files are located in <code>src/sass</code>
				directory. There is a file in this directory <code>main.sass</code> which imports all the files
				and exported as main.css There are four sub directories inside this directory:
			</p>
			<ol>
				<li>
					<code>1-tools</code> - It includes styles of all the external libraries and a file
					<code>_var.scss</code> which contains the variables required for the application
				</li>
				<li>
					<code>2-basics</code> - It contains the basic style like overall structure css and theming
					options
				</li>
				<li>
					<code>3-component</code> - It contains the styles for the components like card, widgets, sidebar,
					navbar etc
				</li>
				<li>
					<code>4-pages</code> - It contains the styles for the specific pages like login page, lock-screen
					page
				</li>
			</ol>
			<p>
				To customize the primary color of the theme and sidebar you need to change the variables in
				the <code>1-tools/_var.scss</code>. The detailed documentation about changing the colors is
				mentioned in this file itself.
			</p>
			<p>
				If you don't want to use particular component or plug-in just comment the import statement
				for that particular component in <code>src/sass/main.scss</code> and compile the SASS by
				running <code>npm run build</code> command.
			</p>
			<h2 class="docs-title" id="Compatibility-with-other-frameworks">
				Compatibility with other frameworks
			</h2>
			<p>
				This theme is not built for a specific framework or technology like Angular or React etc.
				But due to it's modular nature it's very easy to incorporate it into any front-end or
				back-end framework like Angular, React or VueJs or Node JS. The CSS is modular enough to be
				incorporated in any framework. While the Javascript used to make the components interactive
				can be used from any of the following framework.
			</p>
			<p>
				If you are using Angular you can use <a
					href="https://angular-ui.github.io/bootstrap/"
					rel="noopener">ui-bootstrap</a
				>, for React use
				<a href="https://react-bootstrap.github.io/" rel="noopener">React-Bootstrap</a>
				and for VueJs you can use
				<a href="https://yuche.github.io/vue-strap/" rel="noopener">VueStrap</a>.
			</p>
			<p>
				If you are using Node JS as your web server you can use pug as your layout engine to render
				html templates as is without compiling them to HTML. More details are available <a
					href="https://pugjs.org/api/express.html"
					target="_balnk">here</a
				>.
			</p>
			<h2 class="docs-title" id="RTL-Support">RTL Support</h2>
			<p>To enable RTL support</p>
			<ul>
				<li>
					Uncomment this line <code>@import '3-component/rtl';</code> in
					<code>src/sass/main.scss</code>.
				</li>
				<li>
					Add <code>dir="rtl"</code> attribute to <code>&lt;html&gt;</code> tag in
					<code>src/pug/layouts/_layout.pug</code>.
				</li>
				<li>Build the source files using <code>npm run build</code> command.</li>
			</ul>
			<h2 class="docs-title" id="Contribution-and-Issues">Contribution & Issues</h2>
			<p>
				If you liked the theme do star and fork it on <a
					href="https://github.com/pratikborsadiya/vali-admin"
					target="_blank"
					rel="noopener">GitHub</a
				>. If you find anything missing or want to contribute to this documentation, the source is
				available
				<a
					href="https://github.com/pratikborsadiya/vali-admin/blob/master/src/pug/charts.pug"
					target="_blank"
					rel="noopener">here</a
				>. If you have an issue or feature request regarding theme please report it
				<a
					href="https://github.com/pratikborsadiya/vali-admin/issues/new"
					target="_blank"
					rel="noopener">here</a
				>.
			</p>
		</div>
	</div>
</div>
