# Revisiting Textual Feature of Bug-Triage Approach
***
### Project summary
***
With the increase in software size, developers depend on issue tracking systems and researchers attempt to design automatic bug triage approaches. To simulate the process of manual triage where managers make triage after reading descriptions of bug reports, prior approaches typically use natural language processing (NLP) for text understanding. Although the technical choice is straightforward, this technical choice is not built on solid empirical evidences. In this paper, we explore the impact of textual features in bug triage. By enabling and disabling the textual features of a state-of-the-art approach, we analyze their impacts on assigning thousands bug reports of six widely used open source projects. Our result shows that instead of improving it, textual features in fact reduce the effectiveness. In particular, after we turn off its textual features, the f-scores of the baseline approach are improved by 8%. After manual inspection, we find two reasons to explain our result: (1) classic NLP techniques are insufficient to analyze bug reports, because they are not pure natural language texts and contain other elements (e.g., code samples); and (2) some bug reports are poorly written. Our findings reveal a strong need and sufficient opportunities to explore more advanced techniques to handle these complicated elements in bug reports.

### Dataset
***
[ALL](./dataset)
[SHIRO](./dataset/SHIRO) [PDFBOX](./dataset/PDFBOX) [LUCENE](./dataset/LUCENE) [HBASE](./dataset/HBASE) [CASSANDRA](./dataset/CASSANDRA)

List of related papers:
-[bug triage](./researchPapers/KeyWord=bugTriage.txt)
-[bug assignment](./researchPapers/KeyWord=bugAssignment.txt)
-[change request triage](./researchPapers/KeyWord=changeRequestTriage.txt)
-[change request assign](./researchPapers/KeyWord=changeRequestAssign.txt)

### Tools
***
[WEKA, a mature machine learning environment](https://www.cs.waikato.ac.nz/ml/weka/)

As Jonsson[<sup>1</sup>](#refer-anchor-1) used WEKA in his research work, we also leverage this tool for reproduction by following the preprocessing steps in his work.

### References
<div id="refer-anchor-1"></div>

-[1]  Jonsson, Leif, et al. "[Automated bug assignment: Ensemble-based machine learning in large scale industrial contexts.](https://link.springer.com/article/10.1007/s10664-015-9401-9)" Empirical Software Engineering 21.4 (2016): 1533-1578]