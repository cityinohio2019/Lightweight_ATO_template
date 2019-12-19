id: pia_notice
format: html
title: PIA Notice
...

<style>
  .dos-pta-form {
    font-family: TimesNewRoman, Times, serif;
    width: 650px;
    margin: auto;
  }

  .dos-pta-form h2 {
    font-size: 12pt;
    font-family: TimesNewRoman, Times, serif;
    background-color: rgb(89, 129, 187);
    padding: 4px 30px 4px 30px;
    color: white;
    font-weight: bold;
    margin: 0px 0px 0px 0px;
    margin-top: 2em;
  }

  .dos-pta-form .cell-full {
    border-left: 1px solid rgb(89, 129, 187);
    border-right: 1px solid rgb(89, 129, 187);
    border-bottom: 1px solid rgb(89, 129, 187);padding: 4px 30px 4px 30px;
    font-family: TimesNewRoman, Times, serif;
  }

  .dos-pta-form .cell-left {
    border-left: 1px solid rgb(89, 129, 187);
    border-bottom: 1px solid rgb(89, 129, 187);
    padding: 4px 30px 4px 30px;
    width: 49.5%;
    display: table-cell;
    height: 100%;
  }

  .dos-pta-form .cell-right {
    border-left: 1px solid rgb(89, 129, 187);
    border-right: 1px solid rgb(89, 129, 187);
    border-bottom: 1px solid rgb(89, 129, 187);
    padding: 4px 30px 4px 30px;
    width: 49.5%;
    display: table-cell;
    height: 100%;
    vertical-align: top;
  }

</style>

<div class="dos-pta-form">

  <h2>Information Usage, Reasoning and Methods</h2>
  <div class="cell-full">
    <p>{{project.pia_info_usage.q1}}</p>
  </div>

  <h2>Usage of Predictive and Querying Technology</h2>
  <div class="cell-full">
    <p>{{project.pia_info_usage.q2}}</p>
  </div>

  <h2>Assigned Roles and Responsibilitiesy</h2>
  <div class="cell-full">
    <p>{{project.pia_info_usage.q3}}</p>
  </div>

  <h2>PIA, Related to the Uses of Information</h2>
  <div class="cell-full">
    <p>{{project.pia_info_usage.q4}}</p>
  </div>

 
</div>
