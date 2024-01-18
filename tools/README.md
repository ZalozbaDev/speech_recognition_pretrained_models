# HTML training report

## dlabpro

Based on the evaluation procedure of dlabro for evaluation of a training of an acoustic model

```
Example:

~/dLabPro/bin.release/dlabpro $UASR_HOME/scripts/dlabpro/HMM.xtp evl HSB-01/info/train.cfg -Puasr.am.model="3_8" -v2 | tee eval.txt

```

an HTML report can be generated manually.

    * copy "report.html.template" to the result folder and rename appropriately.
    * copy the result summary from the text report and place it into the HTML file
      exactly where you find the "SUMMARY_RESULTS_HERE!!!!!!!!!!!!!!!!" mark.
    * generate a text file with the label confusion matrix.
        * This table is typically splitted. Use the "rectangular selection" feature 
          to recombine this into one big table (with jEdit copy/mark/paste with CTRL key down)
    * run "generate_html_table.pl" and generate the HTML table.
    * copy the contents of the generated file into the HTML report file
      exactly where you find the "TABLE HERE!!!!!!!!!!!!!!!!" mark.
    * verify proper display of the report in a browser (compare with existing reports).
    
