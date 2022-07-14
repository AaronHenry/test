<h1 id="sample-markdown">Sample Markdown</h1>
<p>This is some basic, sample markdown.</p>
<h2 id="second-heading">Second Heading</h2>
<ul>
<li>Unordered lists, and:# test
test</li>
</ul>
<p><a href="https://credprotocol.typeform.com/cred-waitlist?typeform-source=www.credprotocol.com"><img data-opix-event="sign-up" align="center" src="https://img.shields.io/badge/Sign%20up-Cred%20Protocol%20Beta-335EEB?style=for-the-badge&labelColor=414141" /></a>
<a href="https://beta.credprotocol.com/docs/api"><img src="https://img.shields.io/badge/DOCS-Cred%20Protocol%20API-335EEB?style=for-the-badge&amp;labelColor=414141" alt="Cred Protocol API"></a>
<a href="https://www.linkedin.com/company/credprotocol/"><img src="https://img.shields.io/badge/-Cred%20Protocol-335EEB?&amp;logo=linkedin&amp;style=for-the-badge&amp;labelColor=414141" alt="Cred Protocol on LinkedIn"></a>
<a href="https://twitter.com/cred_protocol"><img src="https://img.shields.io/badge/-@Cred__Protocol-335EEB?&amp;logo=twitter&amp;style=for-the-badge&amp;logoColor=white&amp;labelColor=414141" alt="Cred Protocol on Twitter"></a>
<a href="https://github.com/credprotocol"><img src="https://img.shields.io/badge/-credprotocol-335EEB?&amp;logo=github&amp;style=for-the-badge&amp;logoColor=white&amp;labelColor=414141" alt="Cred Protocol on Github"></a></p>
<div align="center">
<h1>Aave V2 Health Factor Dataset</h1>
</div>

<h2 id="-how-can-i-download-this-dataset-">⚡️ How can I download this dataset?</h2>
<h3 id="sample-aave-v2-health-factor-dataset-75-rows-40kb-">Sample Aave V2 health factor dataset (75 rows, 40KB)</h3>
<h3 id="get-your-health-factor-data">Get your health factor data</h3>
<ul>
<li><p>Have borrowing history with Aave V2? Pull your data using this URL
`</p>
</li>
<li><p>AWS CLI </p>
</li>
</ul>
<h3 id="complete-public-aave-v2-health-factor-dataset-1-5m-rows-2-1gb-">Complete public Aave V2 health factor dataset (~1.5M rows, 2.1GB)</h3>
<ul>
<li>AWS CLI</li>
</ul>
<h2 id="-why-this-dataset-">📖 Why this dataset?</h2>
<p>A more granular version of this dataset is the solid foundation upon which our DeFi credit scoring models are built. Reconstructing historical health factors in small intervals is one of the tools we&#39;ve developed the help us judge creditworthiness among DeFi users. Because we&#39;ve grown to appreciate the complexities of Aave health factor data, we want to release a dataset that can help users understand the composition of a health factor.</p>
<h2 id="-how-was-this-data-gathered-">💡 How was this data gathered?</h2>
<p>The following diagram details the main phases of creating this dataset. Generally, they are as follows:</p>
<ul>
<li>Collecting historical off-chain datasets that are used as inputs for the calculations required to compose a health factor</li>
<li>Collecting on-chain data by capturing the emission of every associated event starting at the launch of Aave V2</li>
<li>Combining the off-chain and on-chain data and feeding the resulting values through transformations and ultimately the Aave health factor formula </li>
</ul>
<div>
        <img alt="Aave V2 Health Factor Dataset Data Flow" height="400" src="https://github.com/credprotocol/health-factor-dataset/blob/main/img/Aave%20V2%20Health%20Factor%20Dataset%20Data%20Flow.jpg" width="1200">

</div>

<h2 id="-floppy_disk-what-kinds-of-values-are-in-this-dataset-">:floppy_disk: What kinds of values are in this dataset?</h2>
<p>The Aave V2 Health Factor Dataset contains account-level debt, collateral, and liquidation threshold values for each Aave V2 token along with prices of the associated underlying assets. These columns are accompanied by the aggregate collateral and debt values, computed liquidation thresholds, and the resulting synthetic health factors.  </p>
<h2 id="-what-can-i-do-with-this-dataset-">📖 What can I do with this dataset?</h2>
<p>If you&#39;ve borrowed using Aave V2, the most obvious usecase for this dataset would be reviewing the health factor history of your account. Has your health factor dipped to an uncomfortable level close to liquidation? Have you been successful in staying above your personal health factor benchmarks? How much collateral and debt have you owned at different points in the life of your lending and borrowing account?</p>
<h2 id="-how-accurate-are-the-contents-of-this-dataset-">📖 How accurate are the contents of this dataset?</h2>
<p>In data validation checks performed against available source-of-truth health factors, Our synthetic health factors showed a mean difference of 1.33%. Our calculated aggregated collateral and debt values had mean differences of 0.42% and 1.12%, respectively. These differences can likely be attributed in part to the historical data used in the computation phase. Historical token prices can vary by up to a few percent between sources in times of high volume or volatility. </p>
<h2 id="-contributors">‎‍💻 Contributors</h2>
<ul>
<li>Julian Gay</li>
<li>Xavier Quintuna</li>
<li>Will Wolf</li>
<li>Hamza Al Fadel</li>
<li>Aaron Henry</li>
</ul>
<script>

!function(e,t,n,o,p,i,a){e[o]||((p=e[o]=function(){p.process?p.process.apply(p,arguments):p.queue.push(arguments)}).queue=[],p.t=+new Date,(i=t.createElement(n)).async=1,i.src="/openpixel.js?t="+864e5*Math.ceil(new Date/864e5),(a=t.getElementsByTagName(n)[0]).parentNode.insertBefore(i,a))}(window,document,"script","opix"),opix("init","ID-CREDPROT"),opix("event","pageload");

</script>


<h2 id="-full-schema-and-dataset-properties">⚙️ Full schema and dataset properties</h2>
<p><details></p>
<summary>Reveal full schema and properties</summary>

<h2 id="-dataset-specification-table">⚙️ Dataset specification table</h2>
<table>
<thead>
<tr>
<th style="text-align:left">Specification</th>
<th style="text-align:left">Value</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left">columns</td>
<td style="text-align:left">315</td>
</tr>
<tr>
<td style="text-align:left">observations</td>
<td style="text-align:left">1333683</td>
</tr>
<tr>
<td style="text-align:left">size</td>
<td style="text-align:left">1.91 GB  </td>
</tr>
<tr>
<td style="text-align:left">accounts</td>
<td style="text-align:left">35524</td>
</tr>
</tbody>
</table>
