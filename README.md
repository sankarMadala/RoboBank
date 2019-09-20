# Robobank

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.7.

# Purpose of the project
 Rabobank receives monthly deliveries of customer statement records. This information is delivered in two formats, CSV and XML. These records need to be validated.
 <table class="tableblock frame-all grid-all spread">
<caption class="title">Table 1. Record description</caption>
<colgroup>
<col style="width: 50%;">
<col style="width: 50%;">
</colgroup>
<thead>
<tr>
<th class="tableblock halign-left valign-top">Field</th>
<th class="tableblock halign-left valign-top">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Transaction reference</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">A numeric value</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Account number</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">An IBAN</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Start Balance</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">The starting balance in Euros</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Mutation</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Either and addition (+) or a deducation (-)</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">Description</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">Free text</p></td>
</tr>
<tr>
<td class="tableblock halign-left valign-top"><p class="tableblock">End Balance</p></td>
<td class="tableblock halign-left valign-top"><p class="tableblock">The end balance in Euros</p></td>
</tr>
</tbody>
</table>
<div class="sect1">
<h2 id="_output">Input</h2>
<div class="sectionbody">

<div class="ulist">
<ul>
<li>
<p>Import the statement processor file in CSV or XML format ,the data table will be displayed.click on generate report button to view the failed transactions</p>
</li>
<li>
<p>the end balance needs to be validated</p>
</li>
</ul>
</div>

</div>
</div>
<div class="sect1">
<h2 id="_output">Output</h2>
<div class="sectionbody">
<div class="paragraph">
<p>There are two validations:</p>
</div>
<div class="ulist">
<ul>
<li>
<p>all transaction references should be unique</p>
</li>
<li>
<p>the end balance will be validated with the mutation and starting balance</p>
</li>
</ul>
</div>
<div class="paragraph">
<p>At the end of the processing, a report will be created which will display both the transaction reference and description of each of the failed records.</p>
</div>
</div>
</div>

## Live demo
https://robobank-processor.herokuapp.com

## Development server

Run `node server.js` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
