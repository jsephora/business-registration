---
title: Typography
layout: default
---
<div class="toc">
	<h1><span><a href="../style-guide.html"> &laquo; Style guide</a></span>
	Typography</h1>
</div>
<div class="description">
	<p>Typography describes the fonts, heading size relationships, line and character spacing and styling of specific HTML textual elements.</p>
</div>

<p>Two variations of Open Sans are currently being used:</p>
<ul>
  <li><strong>open_sanslight</strong> for body text</li>
  <li><strong>open_sansregular</strong> for headings</li><!-- Not any more -->
</ul>
<h3>Block Elements</h3>
<p>This is a standard paragraph. Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</p>
<blockquote>
	"<strong>This is a blockquote.</strong> Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Nullam dignissim convallis est. Quisque aliquam. Donec faucibus. Nunc iaculis suscipit dui. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl."
</blockquote>
<p>The <a href="#">a element</a> and <a href="http://example.com" target="_blank">external a element</a> examples</p>
<p>The <abbr>abbr element</abbr> and an <abbr title="Abbreviation">abbr</abbr> element with title examples</p>
<p>The <acronym title="A Cowboy Ran One New York Marathon">ACRONYM</acronym> element example</p>
<p>The <code>code element</code> example</p>
<p>The <data value="3967381398">data element</data> example</p>
<p>The <dfn>dfn element</dfn> and <dfn title="Title text">dfn element with title</dfn> examples</p>
<p>The <em>em element</em> example</p>
<p>The <ins>ins element</ins> example</p>
<p>The <kbd>kbd element</kbd> example</p>
<p>The <mark>mark element</mark> example</p>
<p>The <q>q element</q> example</p>
<p>The <q>q element <q>inside</q> a q element</q> example</p>
<p>The <samp>samp element</samp> example</p>
<p>The <small>small element</small> example</p>
<p>The <span>span element</span> example</p>
<p>The <strong>strong element</strong> example</p>
<p>The <time datetime="2005-05-15 19:00">time element</time> example</p>

#### Ordered List

<ol>
	<li>List Item 1</li>
	<li>List Item 2</li>
	<li>
		List Item 3
		<ol>
			<li>List Item 3.1</li>
			<li>
				List Item 3.2
				<ol>
					<li>List Item 3.2.1</li>
					<li>List Item 3.2.2</li>
				</ol>
			</li>
			<li>List Item 3.3</li>
		</ol>
	</li>
	<li>List Item 4</li>
</ol>

#### Unordered List

<ul>
	<li>List Item 1</li>
	<li>List Item 2</li>
	<li>
		List Item 3
		<ul>
			<li>List Item 3.1</li>
			<li>
				List Item 3.2
				<ul>
					<li>List Item 3.2.1</li>
					<li>List Item 3.2.2</li>
				</ul>
			</li>
			<li>List Item 3.3</li>
		</ul>
	</li>
	<li>List Item 4</li>
</ul>

### Tables

<table cellspacing="0" cellpadding="0">
	<caption>This is a table caption</caption>
	<thead>
	<tr>
		<th>Table Header 1</th>
		<th>Table Header 2</th>
		<th>Table Header 3</th>
	</tr>
	</thead>
	<tbody>
	<tr>
		<td>Division 1</td>
		<td>Division 2</td>
		<td>Division 3</td>
	</tr>
	<tr class="even">
		<td>Division 1</td>
		<td>Division 2</td>
		<td>Division 3</td>
	</tr>
	<tr>
		<td>Division 1</td>
		<td>Division 2</td>
		<td>Division 3</td>
	</tr>
	</tbody>
</table>
<table id="data-table" class="compact">
	<caption>Horizontal compact data table</caption>
	<tbody>
		<tr>
			<th class="field-name right">Table Header 1</th>
			<td class="input-value">Table data 1</td>
		</tr>
		<tr>
			<th class="field-name right">Table Header 2</th>
			<td class="input-value">Table data 2</td>
		</tr>
		<tr>
			<th class="field-name right">Table Header 3</th>
			<td class="input-value">Table data 3</td>
		</tr>
		<tr>
			<th class="field-name right no-border-bottom">Table Header 4</th>
			<td class="input-value no-border-bottom">Table data 4</td>
		</tr>
	</tbody>
</table>
