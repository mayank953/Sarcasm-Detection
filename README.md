<h1><span style="text-decoration: underline;"><strong>SARCASM DETECTION</strong></span></h1>
<p>&nbsp;</p>
<p>The aim of this&nbsp;project is to build a text<span class="fontstyle2"> classification model </span><span class="fontstyle0">to classify statements to sarcastic or non-sarcastic </span>to understand&nbsp;the true context in<span class="fontstyle0"> which it appears.</span></p>
<p>The data is taken from Twitter &amp; contains tweet in different languages.&nbsp;</p>
<h2><span style="text-decoration: underline;"><span class="fontstyle0">PACKAGES USED:</span></span></h2>
<p><span class="fontstyle0"><br /></span><span class="fontstyle0">1. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">data.table</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for faster data manipulations<br />2. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">tm</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> package for text mining<br />3. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">caTools</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for Stratified sampling and Training and Testing splits<br />4. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">caret</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for building confusion matrices<br />5. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">e1071</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for building Na&iuml;ve Bayes classifier<br />6. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">h2o</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for faster implementation of Random forest<br />7. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">wordcloud</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for visualizing word clouds<br />8. <strong>&lsquo;</strong></span><strong><span class="fontstyle2">ggplot2</span></strong><span class="fontstyle0"><strong>&rsquo;</strong> for bar plot visualizations.</span></p>
<p>Project Report.pdf provides a formal report for the project.&nbsp;</p>
<p>&nbsp;</p>
<p><span class="fontstyle0">I have used various models so as to evaluate the performance on "ACCURACY". The table presents details of the same.</span></p>
<p>&nbsp;</p>
<p><span class="fontstyle0"><strong>TABLE PRESENTING AUC FOR VARIOUS MODELS.</strong><br /></span></p>
<table class="NormalTable">
<tbody>
<tr>
<td width="200"><span class="fontstyle2">Random Seed </span></td>
<td width="200"><span class="fontstyle2">NB default </span></td>
<td width="200"><span class="fontstyle2">Numeric RF </span></td>
<td width="200"><span class="fontstyle2">Factor RF </span></td>
<td width="200"><span class="fontstyle2">NB laplace </span></td>
<td width="200"><span class="fontstyle2">GBM </span></td>
<td width="200"><span class="fontstyle2">LR</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">123 </span></td>
<td width="200"><span class="fontstyle2">78.59 </span></td>
<td width="200"><span class="fontstyle2">76.59 </span></td>
<td width="200"><span class="fontstyle2">76.69 </span></td>
<td width="200"><span class="fontstyle2">79.28 </span></td>
<td width="200"><span class="fontstyle2">73.41 </span></td>
<td width="200"><span class="fontstyle3">69.22</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">300 </span></td>
<td width="200"><span class="fontstyle3">76.79 </span></td>
<td width="200"><span class="fontstyle3">72.81 </span></td>
<td width="200"><span class="fontstyle3">76.39 </span></td>
<td width="200"><span class="fontstyle2">79.28 </span></td>
<td width="200"><span class="fontstyle3">72.81 </span></td>
<td width="200"><span class="fontstyle3">70.72</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">111 </span></td>
<td width="200"><span class="fontstyle3">77.89 </span></td>
<td width="200"><span class="fontstyle3">74.7 </span></td>
<td width="200"><span class="fontstyle3">76.2 </span></td>
<td width="200"><span class="fontstyle3">78.09 </span></td>
<td width="200"><span class="fontstyle3">72.91 </span></td>
<td width="200"><span class="fontstyle3">70.12</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">222 </span></td>
<td width="200"><span class="fontstyle3">77.89 </span></td>
<td width="200"><span class="fontstyle3">74.6 </span></td>
<td width="200"><span class="fontstyle3">76.59 </span></td>
<td width="200"><span class="fontstyle3">78.09 </span></td>
<td width="200"><span class="fontstyle3">70.12 </span></td>
<td width="200"><span class="fontstyle3">67.89</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">456 </span></td>
<td width="200"><span class="fontstyle3">76.39 </span></td>
<td width="200"><span class="fontstyle3">74.7 </span></td>
<td width="200"><span class="fontstyle3">76.49 </span></td>
<td width="200"><span class="fontstyle3">77.89 </span></td>
<td width="200"><span class="fontstyle3">73.41 </span></td>
<td width="200"><span class="fontstyle3">69.62</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">10 </span></td>
<td width="200"><span class="fontstyle3">77.69 </span></td>
<td width="200"><span class="fontstyle2">76.59 </span></td>
<td width="200"><span class="fontstyle3">76.1 </span></td>
<td width="200"><span class="fontstyle3">77.89 </span></td>
<td width="200"><span class="fontstyle3">74.4 </span></td>
<td width="200"><span class="fontstyle3">73.8</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">99 </span></td>
<td width="200"><span class="fontstyle3">77.49 </span></td>
<td width="200"><span class="fontstyle3">75.5 </span></td>
<td width="200"><span class="fontstyle3">74.6 </span></td>
<td width="200"><span class="fontstyle3">77.49 </span></td>
<td width="200"><span class="fontstyle3">73.21 </span></td>
<td width="200"><span class="fontstyle2">70.92</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">1215 </span></td>
<td width="200"><span class="fontstyle3">75.3 </span></td>
<td width="200"><span class="fontstyle3">71.31 </span></td>
<td width="200"><span class="fontstyle3">76.1 </span></td>
<td width="200"><span class="fontstyle3">77.09 </span></td>
<td width="200"><span class="fontstyle3">71.71 </span></td>
<td width="200"><span class="fontstyle3">68.33</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">201 </span></td>
<td width="200"><span class="fontstyle3">74.6 </span></td>
<td width="200"><span class="fontstyle3">73.01 </span></td>
<td width="200"><span class="fontstyle3">76.39 </span></td>
<td width="200"><span class="fontstyle3">76.59 </span></td>
<td width="200"><span class="fontstyle3">70.72 </span></td>
<td width="200"><span class="fontstyle3">69.22</span></td>
</tr>
<tr>
<td width="200"><span class="fontstyle3">256 </span></td>
<td width="200"><span class="fontstyle3">76.2 </span></td>
<td width="200"><span class="fontstyle3">73.71 </span></td>
<td width="200"><span class="fontstyle3">75.1 </span></td>
<td width="200"><span class="fontstyle3">76.49 </span></td>
<td width="200"><span class="fontstyle3">70.92 </span></td>
<td width="200"><span class="fontstyle3">67.93</span></td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
