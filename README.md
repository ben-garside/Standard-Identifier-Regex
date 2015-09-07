# Standard-Identifier-Regex
Standard Identifier Regex

The following examples are based on the parsing of this identifier: ``NA + A1:2014 to BS EN / ISO 1997-1.5x:2004+A1:2013``
<table>
	<tbody><tr class="row0">
		<th class="col0">#</th><th class="col1" colspan="3">Named group</th><th class="col4">Definition</th><th class="col5">Example</th>
	</tr>
	<tr class="row1">
		<td class="col0"> – </td><td class="col1" colspan="3"> – </td><td class="col4">Match must be a the beginning of a word</td><td class="col5"></td>
	</tr>
	<tr class="row2">
		<td class="col0">1</td><td class="col1" rowspan="6">NA</td><td class="col2" colspan="2"> – </td><td class="col4">National Annex information</td><td class="col5"><code>NA + A1:2014 to </code></td>
	</tr>
	<tr class="row3">
		<td class="col0">2</td><td class="col1" colspan="2"> NA_PREFIX</td><td class="col3">The prefix of the NA</td><td class="col4"><code>NA</code></td>
	</tr>
	<tr class="row4">
		<td class="col0">3</td><td class="col1" rowspan="3"> NA_AMD</td><td class="col2"> – </td><td class="col3">The amendment of the National Annex</td><td class="col4"><code>+ A1:2014</code></td>
	</tr>
	<tr class="row5">
		<td class="col0">4</td><td class="col1">NA_AMD_NO</td><td class="col2">The amendment number of the National Annex</td><td class="col3"><code>+ A1</code></td>
	</tr>
	<tr class="row6">
		<td class="col0">5</td><td class="col1">NA_AMD_YEAR</td><td class="col2">The amendment year of the National Annex</td><td class="col3"><code>:2014</code></td>
	</tr>
	<tr class="row7">
		<td class="col0">6</td><td class="col1" colspan="2">NA_SUFFIX</td><td class="col3">The suffix of the NA</td><td class="col4"><code> to </code></td>
	</tr>
	<tr class="row8">
		<td class="col0">7</td><td class="col1" rowspan="9">STD</td><td class="col2" colspan="2"> – </td><td class="col4">The root standard identifier</td><td class="col5"><code>BS EN 1997-1:2004</code></td>
	</tr>
	<tr class="row9">
		<td class="col0">8</td><td class="col1" rowspan="3">STD_PREFIX</td><td class="col2"> – </td><td class="col3">The prefix of the root standard</td><td class="col4"><code>BS EN </code></td>
	</tr>
	<tr class="row10">
		<td class="col0">9</td><td class="col1">STD_PREFIX_TEXT</td><td class="col2">The text from the prefix of the root standard</td><td class="col3"><code>BS</code> &amp; <code>EN</code> &amp; <code>ISO</code></td>
	</tr>
	<tr class="row11">
		<td class="col0">10</td><td class="col1">STD_PREFIX_DELIMITER</td><td class="col2">The delimiters from the prefix of the root standard</td><td class="col3"><code>_</code> &amp; <code>/</code> &amp; <code>_</code> (<code>_</code> ⇒ white space)</td>
	</tr>
	<tr class="row12">
		<td class="col0">11</td><td class="col1" colspan="2">STD_NO</td><td class="col3">The numeric part of the root standard</td><td class="col4"><code>1997</code></td>
	</tr>
	<tr class="row13">
		<td class="col0">12</td><td class="col1" colspan="2">STD_PART</td><td class="col3">The part number of the root standard</td><td class="col4"><code>-1</code></td>
	</tr>
	<tr class="row14">
		<td class="col0">13</td><td class="col1" colspan="2">STD_SECTION</td><td class="col3">The section number of the root standard</td><td class="col4"><code>.5</code></td>
	</tr>
	<tr class="row15">
		<td class="col0">14</td><td class="col1" colspan="2">DONT_KNOW</td><td class="col3">No idea, but is catching a viable part of the identifier</td><td class="col4"><code>x</code></td>
	</tr>
	<tr class="row16">
		<td class="col0">15</td><td class="col1" colspan="2">STD_YEAR</td><td class="col3">The year of the root standard</td><td class="col4"><code>:2004</code></td>
	</tr>
	<tr class="row17">
		<td class="col0">16</td><td class="col1" rowspan="3">AMD</td><td class="col2" colspan="2"> – </td><td class="col4">Details of the amendment</td><td class="col5"><code>+A1:2013</code></td>
	</tr>
	<tr class="row18">
		<td class="col0">17</td><td class="col1" colspan="2">AMD_NO</td><td class="col3">The amendment number</td><td class="col4"><code>+A1</code></td>
	</tr>
	<tr class="row19">
		<td class="col0">18</td><td class="col1" colspan="2">AMD_YEAR</td><td class="col3">The year of the amendment</td><td class="col4"><code>:2013</code></td>
	</tr>
</tbody></table>
