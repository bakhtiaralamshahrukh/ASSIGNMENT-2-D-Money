# ASSIGNMENT D-Money:
### d-money is a demo financial related project where fake money can be transferred. In this project I have automate the d-money api using postman and newman. Here I have covered folowing tasks as create new user, login, deposit money, withdraw money, send money, make payment, and checking Statement of user.

## About this project:
- Postman
- Newman
- Visual Studio

## Prerequisites
- nodejs
- newman-reporter-htmlextra

## How to run this project:
- clone this project
- Give following command
- npm i
- npm test

## D-Money API Documentation
https://documenter.getpostman.com/view/22180294/2s9Y5ZvhTh

## Test Report
![image](https://github.com/bakhtiaralamshahrukh/ASSIGNMENT-2-D-Money/assets/69646920/3dcda8b2-3d25-4c68-9237-2666845c7b62)

[Upl<!DOCTYPE html>
<html lang="en" style="overflow-y: scroll;">
<head>
  <meta charset="UTF-8">
  <title>Newman Summary Report</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.13.0/css/all.min.css">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.2/styles/default.min.css">
  <link rel="stylesheet" href="https://cdn.datatables.net/v/bs4/dt-1.10.18/datatables.min.css"/>

<style>
code.renderMarkdown table, code.renderMarkdown th, code.renderMarkdown td {
    border: 1px solid black;
    width: max-content;
    padding: .75rem;
}

.theme-dark {
    --background-color: #222;
    --bg-card-deck: #444444;
    --text-color: #ccd2d8;
    --tab-border: solid 1px #444;
    --success: #3c9372;
    --failure: #c24a3f;
    --warning: #d28c23;
    --info: #4083b6;
    --badge-outline: #3c9372;
    --badge-bg: #cdd3db;
    --badge-text: #ccd2d9;
    --failure-row: #c24a3f;
    --warning-row: #d28c23;
    --card-bg: #444;
    --card-footer: #4f5758;
    --form-input: #ececb5;
    --hov-text: #d2dae5;
    --h4-text: #ccd1d9;
}

.theme-light {
    --tab-border: solid 1px #fff;
    --text-color: #000000;
    --success: #42a745;
    --failure: #dc3544;
    --warning: #f4c10b;
    --info: #49a1b8;
    --badge-outline: #040411;
    --badge-bg: #f8f9fa;
    --badge-text: #fff;
    --failure-row: #f5c6cb;
    --warning-row: #ffeeba;
    --card-bg: #f7f7f7;
    --hov-text: #fff;
    --h4-text: #ffffff;
}

body {
  padding-top:30px;
  background-color: var(--background-color)!important;
  color: var(--text-color);
}

#execution-data {
  padding: 10px;
  border: var(--tab-border);
  border-top: none;
}

.nav-tabs {
  padding-top: 10px;
  height: 105px;
  overflow-y: auto;
}

body.theme-dark .card-header {
    background-color: #444;
}

body.theme-light .card-header {
    background-color: #f7f7f7;
}

.card-footer {
    padding: .75rem 1.25rem;
    background-color: var(--card-footer);
}

.card-deck {
    background-color: var(--bg-card-deck)!important;
}
.form-control {
    background: var(--form-input);
}

.custom-tab {
  padding: 10px 15px;
  margin-right: 0px;
  height: 47px;
  width: 69px;
  text-align: center;
  border: var(--tab-border);
  border-bottom: none;
  cursor:pointer;
}

body.theme-dark .text-white {
    color: #ccd2d9!important;
}
h4 {
    color: var(--h4-text);
}

body.theme-dark h1 {
    color: #ccd2da;
}

body.theme-dark .bg-light>td {
    background: #4f5858!important;
}

body.theme-dark .hljs {
    background: #0a0a0ab0!important;
    color: #8d8787!important;
}

.bg-info {
    background-color: var(--info)!important;
}
.bg-success {
    background-color: var(--success)!important;
}

.alert-success {
    background-color: var(--success)!important;
}

.alert-warning {
    background-color: var(--warning)!important;
}

.alert-info {
    background-color: var(--info)!important;
}

.bg-warning {
    background-color: var(--warning)!important;
}

.badge-warning {
    color: var(--badge-text)!important;
    background-color: var(--warning)!important;
}

.table-warning>td {
    background-color: var(--warning-row);
}

.alert-danger {
    background-color: var(--failure)!important;
}

body.theme-dark .alert-dark {
    background-color: #636467!important;
}

body.theme-dark .text-dark {
    color: #d1dae4!important;
}

body.theme-dark .badge-light {
    color: #212529;
    background-color: #cdd3db;
}

body.theme-light .badge-light {
    color: #212529;
    background-color: #f8f9fa;
}
body.theme-light .bg-danger {
    background-color: var(--failure)!important;
}

body.theme-dark .bg-danger {
    background-color: var(--failure)!important;
}

.table-danger>td {
    background-color: var(--failure-row);
}

body.theme-dark .table .thead-light th {
    background-color: #4f5858!important;
    border-color: #dee2e6!important;
    color: #ccd2d8!important;
}

.itPassed {
  background: var(--success);
  color: white;
}
.itFailed {
  background: var(--failure);
  color: white;
}

.resultsInfoPass {
  color: var(--success);
  padding-top: 4px;
}

.resultsInfoFail {
  color: var(--failure);
  padding-top: 4px;
}

.badge-outline-success {
  color: var(--success);
  border: 1px solid var(--success);
  background-color: transparent;
}

.badge-outline {
  color: var(--badge-outline);
  border: 1px solid var(--badge-outline);
  background-color: transparent;
}

.btn-outline-success {
    color: var(--success)!important;
    border-color: var(--success)!important;
}

.backToTop:hover {
  background-color: var(--success);
  border-color: var(--success);
  color: var(--hov-text)!important;
}

.btn-outline-success:hover {
  background-color: var(--success);
  border-color: var(--success);
  color: var(--hov-text)!important;
}

.btn-outline-secondary {
  background-color: var(--success)!important;
  color: var(--hov-text)!important;
}

body.theme-dark .env-heading {
    color: #ccd2d9!important;
}

body, html {
  height:100%;
}

.card {
  overflow:hidden;
}

body.theme-dark .card-body {
    background-color: #444;
}

body.theme-light .card-body {
    background-color: #f7f7f7;
}

body.theme-dark .card-body .bg-danger {
    background-color: var(--failure)!important;
}

body.theme-light .card-body .bg-danger {
    background-color: var(--failure)!important;
}

.card-body .rotate {
  z-index: 8;
  float: right;
  height: 100%;
}

.card-body .rotate i {
  color: #14141426;
  position: absolute;
  left: 0;
  left: auto;
  right: -10px;
  bottom: 0;
  display: block;
  -webkit-transform: rotate(-44deg);
  -moz-transform: rotate(-44deg);
  -o-transform: rotate(-44deg);
  -ms-transform: rotate(-44deg);
  transform: rotate(-44deg);
}

.dyn-height {
  max-height:350px;
  overflow-y:auto;
}

.nav-pills .nav-link.active {
  background-color: transparent!important;
}

.backToTop {
  display: none;
  position: fixed;
  bottom: 10px;
  right: 20px;
  z-index: 99;
  font-size: 15px;
  outline: none;
  cursor: pointer;
  padding: 15px;
  border-radius: 4px;
}

.card-header .fa {
  transition: .3s transform ease-in-out;
}
.card-header .collapsed .fa {
  transform: rotate(90deg);
}

.single-line-tabs {
  padding-top: 10px;
  height: 60px;
}

::-webkit-scrollbar {
  width: 5px;
}

::-webkit-scrollbar-track {
  background: #f1f1f1;
}

::-webkit-scrollbar-thumb {
  background: #888;
}

::-webkit-scrollbar-thumb:hover {
  background: #555;
}

/* The switch - the box around the slider */
.switch {
  position: relative;
  display: inline-block;
  width: 44px;
  height: 20px;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 20px;
  width: 20px;
  left: 0px;
  bottom: 4px;
  top: 0;
  bottom: 0;
  margin: auto 0;
  -webkit-transition: 0.4s;
  transition: 0.4s;
  box-shadow: 0 0px 15px #2020203d;
  background: white;
  background-repeat: no-repeat;
  background-position: center;
}

input:checked + .slider {
  background-color: #4083b6;
}

input:focus + .slider {
  box-shadow: 0 0 1px #4083b6;
}

input:checked + .slider:before {
  -webkit-transform: translateX(24px);
  -ms-transform: translateX(24px);
  transform: translateX(24px);
  background: white;
  background-repeat: no-repeat;
  background-position: center;
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

table.dataTable td, table.dataTable tr {
    vertical-align: middle;
}

body.theme-dark code {
    color: #ccd2d8!important;
}

body.theme-light code {
    color: #000000!important;
}

.text-wrap {
    word-wrap: break-word; 
    min-width: 600px; 
    max-width: 600px; 
    white-space: normal;
}

</style>
</head>
<body class="theme-dark">
<script>
    function setTheme(themeName) {
        localStorage.setItem('theme', themeName);
        document.body.className = themeName;
    }

    function toggleTheme() {
        if (localStorage.getItem('theme') === 'theme-light') {
            setTheme('theme-dark');
        } else {
            setTheme('theme-light');
        }
    }
</script>
  <div class="container">
        <div class="container">
            <label>Light</label>
            <label id="switch" class="switch">
                <input type="checkbox" onchange="toggleTheme()" id="slider">
                <span class="slider round"></span>
            </label>
            <label>Dark</label>
        </div>
        <div class="card">
        <div class="card-header">
            <ul class="nav nav-pills mb-3 nav-justified" id="pills-tab" role="tablist">
            <li class="nav-item bg-info active" data-toggle="tooltip" title="Click to view the Summary">
                <a class="nav-link text-white" id="pills-summary-tab" data-toggle="pill" href="#pills-summary" role="tab" aria-controls="pills-summary" aria-selected="true">Summary</a>
            </li>
            <li class="nav-item bg-success" data-toggle="tooltip" title="Click to view the Requests">
                <a class="nav-link text-white" id="pills-requests-tab" data-toggle="pill" href="#pills-requests" role="tab" aria-controls="pills-requests" aria-selected="false">Total Requests <span class="badge badge-light">21</span></a>
            </li>
            <li class="nav-item bg-danger" data-toggle="tooltip" title="Click to view the Failed Tests">
                <a class="nav-link text-white" id="pills-failed-tab" data-toggle="pill" href="#pills-failed" role="tab" aria-controls="pills-failed" aria-selected="false">Failed Tests <span class="badge badge-light">1</span></a>
            </li>
            <li class="nav-item bg-warning" data-toggle="tooltip" title="Click to view the Skipped Tests">
                <a class="nav-link text-white" id="pills-skipped-tab" data-toggle="pill" href="#pills-skipped" role="tab" aria-controls="pills-skipped" aria-selected="false">Skipped Tests <span class="badge badge-light">0</span></a>
            </li>
            </ul>
        <div class="tab-content" id="pills-tabContent">
            <div class="tab-pane fade show active" id="pills-summary" role="tabcard" aria-labelledby="pills-summary-tab">
<div class="row">
  <div class="col-md-9 col-lg-12 main">
   <h1 class="display-2 text-center">Newman Run Dashboard</h1>
   <h5 class="text-center">Tuesday, 29 August 2023 17:25:38</h5>
   <div class="row">
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-success">
      <div class="card-body bg-danger">
       <div class="rotate">
        <i class="fa fa-retweet fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Iterations</h6>
       <h1 class="display-1">1</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-danger">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-list fa-4x"></i>
       </div>
       <h6 class="text-uppercase">Total Assertions</h6>
       <h1 class="display-1">29</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-info">
      <div class="card-body bg-danger">
       <div class="rotate">
        <i class="fa fa-plus-circle fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Failed Tests</h6>
       <h1 class="display-1">1</h1>
      </div>
     </div>
    </div>
    <div class="col-lg-3 col-md-6">
     <div class="card text-white card-warning">
      <div class="card-body bg-success">
       <div class="rotate">
        <i class="fa fa-share fa-5x"></i>
       </div>
       <h6 class="text-uppercase">Total Skipped Tests</h6>
       <h1 class="display-1">0</h1>
      </div>
     </div>
    </div>
   </div>
   <hr>
    <div class="row">
    <div class="col">
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="card border-info">
                <div class="card-body">
                <h5 class="card-title text-uppercase text-white text-center bg-info">File Information</h5>
                <span><i class="fas fa-file-code"></i></span><strong> Collection:</strong> 2. postman collection D-money<br>
                
                
                </div>
            </div>
        </div>
        </div>
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="card border-info">
                <div class="card-body">
                <h5 class="card-title text-uppercase text-white text-center bg-info">Timings and Data</h5>
                <span><i class="fas fa-stopwatch"></i></span><strong> Total run duration:</strong> 2.5s<br>
                <span><i class="fas fa-database"></i></span><strong> Total data received:</strong> 2.19KB<br>
                <span><i class="fas fa-stopwatch"></i></span><strong> Average response time:</strong> 35ms<br>
                </div>
            </div>
        </div>
        </div>
        <div class="row">
        <div class="col-sm-12 mb-3">
            <div class="table-responsive">
            <table class="table table-striped table-bordered">
                <thead class="thead-inverse">
                    <tr class="text-center">
                        <th class="text-uppercase">Summary Item</th>
                        <th class="text-uppercase">Total</th>
                        <th class="text-uppercase">Failed</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Requests</td>
                        <td class="text-center">21</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr>
                        <td>Prerequest Scripts</td>
                        <td class="text-center">27</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr>
                        <td>Test Scripts</td>
                        <td class="text-center">42</td>
                        <td class="text-center">0</td>
                    </tr>
                    <tr class="table-danger">
                        <td>Assertions</td>
                        <td class="text-center">29</td>
                        <td class="text-center">1</td>
                    </tr>
                    <tr class="">
                        <td>Skipped Tests</td>
                        <td class="text-center">0</td>
                        <td class="text-center">-</td>
                    </tr>
                </tbody>
            </table>
            </div>
        </div>
        </div>
    <hr>
   </div>
   </div>
  </div>
 </div>
        </div>
            <div class="tab-pane fade" id="pills-failed" role="tabcard" aria-labelledby="pills-failed-tab">
                <button id="topOfFailuresScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()">Go To Top</button>

                    <div class="btn-group float-right" role="group" aria-label="Button Group">
                        <button id="openAllFailed" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width: 185px;">Expand All Failed Tests</button>
                    </div>
                    <br>
                    <br>

                    <div class="alert alert-danger text-uppercase text-center">
                        <h4>Showing 1 Failure</h4>
                    </div>
                    <div class="col-sm-12 mb-3">
                    <div class="card-deck">
                        <div class="card border-danger">
                            <div class="card-header bg-danger">
                                <a data-toggle="collapse" href="#" data-target="#fails-collapse-75beb489-1ae7-4c12-aca3-68b6dc31bc44" aria-expanded="false" aria-controls="collapse" id="fails-75beb489-1ae7-4c12-aca3-68b6dc31bc44" class="collapsed text-white z-block">
                                    Iteration 1 - AssertionError - 2. postman collection D-money - Admin can Create Customer 1 invalid role <i class="float-lg-right fa fa-chevron-down" style="padding-top:5px;"></i>
                                </a>
                            </div>
                            <div id="fails-collapse-75beb489-1ae7-4c12-aca3-68b6dc31bc44" class="collapse" aria-labelledby="fails-75beb489-1ae7-4c12-aca3-68b6dc31bc44">
                            <div class="card-body">
                                <h5 ><strong>Failed Test:</strong> Status code is 203</h5>
                            <hr>
                            <h5 class="card-title text-uppercase text-white text-center bg-danger">Assertion Error Message</h5>
                            <div>
                                <pre><code >expected response to have status code 203 but got 201</code></pre>
                            </div>
                            </div>
                            </div>
                        </div>
                    </div>
                    </div>
            </div>

            <div class="tab-pane fade" id="pills-skipped" role="tabcard" aria-labelledby="pills-skipped-tab">
                <button id="topOfSkippedScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()">Go To Top</button>

                <div class="alert alert-success text-uppercase text-center">
                    <br><br><h1 class="text-center">There are no skipped tests <span><i class="far fa-thumbs-up"></i></span></h1><br><br>
                </div>
            </div>
            <div class="tab-pane fade" id="pills-requests" role="tabcard" aria-labelledby="pills-requests-tab">

            <button id="topOfRequestsScreen" class="btn btn-outline-success btn-sm backToTop" onclick="topFunction()">Go To Top</button>

            <div class="btn-group float-right" role="group" aria-label="Button Group">
                <button id="showOnlyFailures" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width:160px;">Show Failed Iterations</button>
                <button id="openAll" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width: 140px;">Expand Folders</button>
                <button id="openAllRequests" class="btn btn-outline-success btn-sm float-right" style="text-align: center; width: 140px;">Expand Requests</button>
            </div>

    <div class="text-uppercase" id="execution-menu">
        <h5>1 Iteration available to view</h5>
        
        <nav class="table-responsive">
        <ul class="nav single-line-tabs" id="iterationList">
        </ul>
        </nav>
    </div>
    <h6 class="text-uppercase text-muted" id="iterationSelected" style="padding-top: 10px;"></h6>
	<div class="tab-content" id="execution-data">
            <div id="folder-fcece535-4118-4b27-891b-a8c911607358" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-fcece535-4118-4b27-891b-a8c911607358" aria-expanded="false" aria-controls="collapse" id="requests-fcece535-4118-4b27-891b-a8c911607358" class="collapsed text-white z-block">
                    Iteration: 1 - Admin can do login successfully <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-fcece535-4118-4b27-891b-a8c911607358" class="collapse" aria-labelledby="requests-fcece535-4118-4b27-891b-a8c911607358">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/user/login" target="_blank">http://dmoney.roadtocareer.net/user/login</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 51ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 254B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">e191b9d5-210b-4d5b-b8e3-643534bfff69</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">66</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-0" class="prettyPrint">{
            &quot;email&quot;:&quot;admin@roadtocareer.net&quot;,
            &quot;password&quot;:&quot;1234&quot;
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:35 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;fe-XCCay0eK7+uwxAVlbMIUi3KLDYk&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">254</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">200 OK</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;100</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-6bf54cea-5dee-459f-8fe8-228eb4b7e6b1" class="prettyPrint">{&quot;message&quot;:&quot;Login successfully&quot;,&quot;token&quot;:&quot;eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c&quot;,&quot;role&quot;:&quot;Admin&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-6bf54cea-5dee-459f-8fe8-228eb4b7e6b1">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User can login successfully</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 200</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-365fcc48-f716-480a-b216-d5488b1677d9" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-365fcc48-f716-480a-b216-d5488b1677d9" aria-expanded="false" aria-controls="collapse" id="requests-365fcc48-f716-480a-b216-d5488b1677d9" class="collapsed text-white z-block">
                    Iteration: 1 - Admin can Create Customer 1 <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-365fcc48-f716-480a-b216-d5488b1677d9" class="collapse" aria-labelledby="requests-365fcc48-f716-480a-b216-d5488b1677d9">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/user/create" target="_blank">http://dmoney.roadtocareer.net/user/create</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 28ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 261B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">2654106f-8cbb-436a-a30f-19b9efebefbd</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">176</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-1" class="prettyPrint">{
            &quot;name&quot;:&quot;Test Customer 1&quot;,
            &quot;email&quot;:&quot;user78517@test.com&quot;,
            &quot;password&quot;:&quot;1234&quot;,
            &quot;phone_number&quot;:&quot;01502640607&quot;,
            &quot;nid&quot;:&quot;123456789&quot;,
            &quot;role&quot;:&quot;Customer&quot;
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-1">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:35 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;105-rNErokLvlVmytkS4vtQMy7Z+VK0&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">261</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;99</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-b7d9bede-abdf-44e4-8395-00971ac936c0" class="prettyPrint">{&quot;message&quot;:&quot;User created&quot;,&quot;user&quot;:{&quot;id&quot;:25462,&quot;name&quot;:&quot;Test Customer 1&quot;,&quot;email&quot;:&quot;user78517@test.com&quot;,&quot;password&quot;:&quot;1234&quot;,&quot;phone_number&quot;:&quot;01502640607&quot;,&quot;nid&quot;:&quot;123456789&quot;,&quot;role&quot;:&quot;Customer&quot;,&quot;updatedAt&quot;:&quot;2023-08-29T11:25:35.808Z&quot;,&quot;createdAt&quot;:&quot;2023-08-29T11:25:35.808Z&quot;}}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-b7d9bede-abdf-44e4-8395-00971ac936c0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User created successfully</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-8e43d38b-c2e2-488f-a3a8-6598af9398ea" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-danger iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea" aria-expanded="false" aria-controls="collapse" id="requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea" class="collapsed text-white z-block">
                    Iteration: 1 - Admin can Create Customer 1 invalid role <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea" class="collapse" aria-labelledby="requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/user/create" target="_blank">http://dmoney.roadtocareer.net/user/create</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 25ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 262B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-danger" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>50 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">e4f18cdd-3eb2-4889-b996-61d561be1385</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">177</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-2" class="prettyPrint">{
            &quot;name&quot;:&quot;Test Customer 1&quot;,
            &quot;email&quot;:&quot;user68173@test.com&quot;,
            &quot;password&quot;:&quot;1234&quot;,
            &quot;phone_number&quot;:&quot;01502184884&quot;,
            &quot;nid&quot;:&quot;123456789&quot;,
            &quot;role&quot;:&quot;Custome2r&quot;
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-2">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:35 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;106-5fLUgRd9Hf/+1K6wSwK6d13yorI&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">262</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;98</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-f643d1ff-369c-4541-bad1-49ed8210c7fc" class="prettyPrint">{&quot;message&quot;:&quot;User created&quot;,&quot;user&quot;:{&quot;id&quot;:25463,&quot;name&quot;:&quot;Test Customer 1&quot;,&quot;email&quot;:&quot;user68173@test.com&quot;,&quot;password&quot;:&quot;1234&quot;,&quot;phone_number&quot;:&quot;01502184884&quot;,&quot;nid&quot;:&quot;123456789&quot;,&quot;role&quot;:&quot;Custome2r&quot;,&quot;updatedAt&quot;:&quot;2023-08-29T11:25:35.914Z&quot;,&quot;createdAt&quot;:&quot;2023-08-29T11:25:35.914Z&quot;}}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-f643d1ff-369c-4541-bad1-49ed8210c7fc">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User created successfully</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 203</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center bg-danger">1</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row ">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                            <tr>
                                                                <td class="w-45 text-nowrap ">Status code is 203</td>
                                                                <td class="w-55"><pre><code >expected response to have status code 203 but got 201</code></pre></td>
                                                            </tr>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77" aria-expanded="false" aria-controls="collapse" id="requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77" class="collapsed text-white z-block">
                    Iteration: 1 - Admin can Create Customer 2 <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77" class="collapse" aria-labelledby="requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/user/create" target="_blank">http://dmoney.roadtocareer.net/user/create</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 26ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 261B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">4c305304-05e5-4047-81ef-bc6f0ce0b95e</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">176</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-3" class="prettyPrint">{
            &quot;name&quot;:&quot;Test Customer 2&quot;,
            &quot;email&quot;:&quot;user20248@test.com&quot;,
            &quot;password&quot;:&quot;1234&quot;,
            &quot;phone_number&quot;:&quot;01503689922&quot;,
            &quot;nid&quot;:&quot;123456789&quot;,
            &quot;role&quot;:&quot;Customer&quot;
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-3">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;105-kmlWFZ9AKpEMyAE5j17JcvU7JXY&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">261</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;97</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-5d99c233-46e5-4a4e-b804-42bbf9b6ff33" class="prettyPrint">{&quot;message&quot;:&quot;User created&quot;,&quot;user&quot;:{&quot;id&quot;:25464,&quot;name&quot;:&quot;Test Customer 2&quot;,&quot;email&quot;:&quot;user20248@test.com&quot;,&quot;password&quot;:&quot;1234&quot;,&quot;phone_number&quot;:&quot;01503689922&quot;,&quot;nid&quot;:&quot;123456789&quot;,&quot;role&quot;:&quot;Customer&quot;,&quot;updatedAt&quot;:&quot;2023-08-29T11:25:36.039Z&quot;,&quot;createdAt&quot;:&quot;2023-08-29T11:25:36.039Z&quot;}}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-5d99c233-46e5-4a4e-b804-42bbf9b6ff33">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User created successfully</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-b3bbb584-3b43-4158-86e7-86c9c288145d" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-b3bbb584-3b43-4158-86e7-86c9c288145d" aria-expanded="false" aria-controls="collapse" id="requests-b3bbb584-3b43-4158-86e7-86c9c288145d" class="collapsed text-white z-block">
                    Iteration: 1 - Admin can Create agent <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-b3bbb584-3b43-4158-86e7-86c9c288145d" class="collapse" aria-labelledby="requests-b3bbb584-3b43-4158-86e7-86c9c288145d">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/user/create" target="_blank">http://dmoney.roadtocareer.net/user/create</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 25ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 258B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">3ac65887-ce65-4c84-b2b3-8722396d7bde</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">173</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-4" class="prettyPrint">{
            &quot;name&quot;:&quot;Test Agent 1&quot;,
            &quot;email&quot;:&quot;user71747@test.com&quot;,
            &quot;password&quot;:&quot;1234&quot;,
            &quot;phone_number&quot;:&quot;01505407246&quot;,
            &quot;nid&quot;:&quot;123456789&quot;,
            &quot;role&quot;:&quot;Customer&quot;
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-4">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;102-lH0AKZT6wRTp5zdAJQPO6YZnTog&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">258</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;96</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-42e35cf9-62ed-4945-8387-c9e5f3739636" class="prettyPrint">{&quot;message&quot;:&quot;User created&quot;,&quot;user&quot;:{&quot;id&quot;:25465,&quot;name&quot;:&quot;Test Agent 1&quot;,&quot;email&quot;:&quot;user71747@test.com&quot;,&quot;password&quot;:&quot;1234&quot;,&quot;phone_number&quot;:&quot;01505407246&quot;,&quot;nid&quot;:&quot;123456789&quot;,&quot;role&quot;:&quot;Customer&quot;,&quot;updatedAt&quot;:&quot;2023-08-29T11:25:36.153Z&quot;,&quot;createdAt&quot;:&quot;2023-08-29T11:25:36.153Z&quot;}}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-42e35cf9-62ed-4945-8387-c9e5f3739636">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User created successfully</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-bac5453f-810a-4e4b-b3c4-54d33ecd596c" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c" aria-expanded="false" aria-controls="collapse" id="requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c" class="collapsed text-white z-block">
                    Iteration: 1 - System Deposit to Agent <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c" class="collapse" aria-labelledby="requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/deposit" target="_blank">http://dmoney.roadtocareer.net/transaction/deposit</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 90ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 99B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">67790223-5389-4ae6-b06f-7ff9b457e06d</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">91</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-5" class="prettyPrint">{
            &quot;from_account&quot;:&quot;SYSTEM&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:500
        }
        
        
        </code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-5">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;63-lcGlpUnUwTtpkq4CXbvvTJgxJCE&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">99</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;95</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-0d3d9abf-dae1-4fce-af52-a13bac4cc9c8" class="prettyPrint">{&quot;message&quot;:&quot;Deposit successful&quot;,&quot;trnxId&quot;:&quot;TXN427178&quot;,&quot;commission&quot;:12.5,&quot;currentBalance&quot;:3940842.37}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-0d3d9abf-dae1-4fce-af52-a13bac4cc9c8">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Deposit successful</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 201</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-274e566a-ec91-4926-834f-99df62950d47" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-274e566a-ec91-4926-834f-99df62950d47" aria-expanded="false" aria-controls="collapse" id="requests-274e566a-ec91-4926-834f-99df62950d47" class="collapsed text-white z-block">
                    Iteration: 1 - System Deposit to Agent wrong account <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-274e566a-ec91-4926-834f-99df62950d47" class="collapse" aria-labelledby="requests-274e566a-ec91-4926-834f-99df62950d47">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/deposit" target="_blank">http://dmoney.roadtocareer.net/transaction/deposit</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 404 - Not Found</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 19ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 36B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">f2c300f2-5c43-41fb-8773-ebd5b74601d0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">90</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-6" class="prettyPrint">{
            &quot;from_account&quot;:&quot;AGENT&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:500
        }
        
        
        </code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-6">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;24-dQ7qDQebbvfP5t+vS4R/Nenb2N4&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">36</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">404 Not Found</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;94</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-37ec3ec0-f6dd-4686-aa14-8b9881295a15" class="prettyPrint">{&quot;message&quot;:&quot;Account does not exist&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-37ec3ec0-f6dd-4686-aa14-8b9881295a15">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Account does not exist</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-9821549c-0cd5-4af3-9a72-f09a48b9b909" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909" aria-expanded="false" aria-controls="collapse" id="requests-9821549c-0cd5-4af3-9a72-f09a48b9b909" class="collapsed text-white z-block">
                    Iteration: 1 - System Deposit to Agent (10-10000) <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909" class="collapse" aria-labelledby="requests-9821549c-0cd5-4af3-9a72-f09a48b9b909">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/deposit" target="_blank">http://dmoney.roadtocareer.net/transaction/deposit</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 208 - Already Reported</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 49ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 78B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">a85be14a-13df-4b2d-9fe9-2dd0d3fb4697</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-7" class="prettyPrint">{
            &quot;from_account&quot;:&quot;SYSTEM&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:7
        }
        
        
        </code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-7">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;4e-etUN+0yOCvPMw0BBolT64hpUR3U&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">78</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">208 Already Reported</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;93</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-7f019a99-50de-4806-8a23-1a23a30413c0" class="prettyPrint">{&quot;message&quot;:&quot;Minimum deposit amount 10 tk and maximum deposit amount 10000 tk&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-7f019a99-50de-4806-8a23-1a23a30413c0">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Minimum deposit amount 10 tk and maximum deposit amount 10000 tk</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 208</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-a88996bc-acbd-45bf-ad63-2862da5ba58a" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a" aria-expanded="false" aria-controls="collapse" id="requests-a88996bc-acbd-45bf-ad63-2862da5ba58a" class="collapsed text-white z-block">
                    Iteration: 1 - agent Deposit to Customer <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a" class="collapse" aria-labelledby="requests-a88996bc-acbd-45bf-ad63-2862da5ba58a">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/deposit" target="_blank">http://dmoney.roadtocareer.net/transaction/deposit</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 113ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 91B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">c7d978be-42b5-47ec-b1d5-83ad5bb6c778</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">90</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-8" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01708938089&quot;,
            &quot;to_account&quot;:&quot;01505407246&quot;,
            &quot;amount&quot;:400
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-8">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;5b-7xeUx/pfi3fTVmOR8L+g137xRu0&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">91</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;92</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-2bdba909-da1a-47cf-bbb8-6f8a7c3a85ef" class="prettyPrint">{&quot;message&quot;:&quot;Deposit successful&quot;,&quot;trnxId&quot;:&quot;TXN363292&quot;,&quot;commission&quot;:10,&quot;currentBalance&quot;:2139}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-2bdba909-da1a-47cf-bbb8-6f8a7c3a85ef">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Customer deposit is successful</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-d0cadf5b-0cda-4d24-923c-b0dc09ee777e" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e" aria-expanded="false" aria-controls="collapse" id="requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e" class="collapsed text-white z-block">
                    Iteration: 1 - agent Deposit to Customer invalid agent no. <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e" class="collapse" aria-labelledby="requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/deposit" target="_blank">http://dmoney.roadtocareer.net/transaction/deposit</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 404 - Not Found</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 18ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 36B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">56acaa35-0823-4d06-ba4a-b61103b7cc69</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">102</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-9" class="prettyPrint">{
            &quot;from_account&quot;:&quot;{{agent_phone_number2}}&quot;,
            &quot;to_account&quot;:&quot;01505407246&quot;,
            &quot;amount&quot;:400
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-9">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;24-dQ7qDQebbvfP5t+vS4R/Nenb2N4&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">36</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">404 Not Found</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;91</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-471fc7dc-4405-4cde-a0f8-372a7b611f2b" class="prettyPrint">{&quot;message&quot;:&quot;Account does not exist&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-471fc7dc-4405-4cde-a0f8-372a7b611f2b">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Status code is 404</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-c809d899-c8e4-4294-9e25-27b6ccb7487d" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d" aria-expanded="false" aria-controls="collapse" id="requests-c809d899-c8e4-4294-9e25-27b6ccb7487d" class="collapsed text-white z-block">
                    Iteration: 1 - Check agent balance <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d" class="collapse" aria-labelledby="requests-c809d899-c8e4-4294-9e25-27b6ccb7487d">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/balance/01708938089" target="_blank">http://dmoney.roadtocareer.net/transaction/balance/01708938089</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 15ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 41B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">eddd893a-0405-40b2-a7a6-12615e4d6f82</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:36 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;29-KBYls1jjxIA6dMajjQARXKrZBF4&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">41</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">200 OK</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;90</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-078e2fe2-568f-4935-be0d-d39cbc6e5865" class="prettyPrint">{&quot;message&quot;:&quot;User balance&quot;,&quot;balance&quot;:2139}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-078e2fe2-568f-4935-be0d-d39cbc6e5865">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User balance</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 200</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-6c9848c7-f920-439e-ac54-2ee7fa72f16c" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c" aria-expanded="false" aria-controls="collapse" id="requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c" class="collapsed text-white z-block">
                    Iteration: 1 - Money withdraw by customer <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c" class="collapse" aria-labelledby="requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/withdraw" target="_blank">http://dmoney.roadtocareer.net/transaction/withdraw</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 49ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 83B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">12507c2d-27ab-4277-a088-f26a2cba6480</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-11" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01505407246&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:20
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-11">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;53-QP/e/FtGmhI0OIYkJzvK51TdYl0&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">83</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;89</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-2465bf79-954b-4109-9325-7634f8df9711" class="prettyPrint">{&quot;message&quot;:&quot;Withdraw successful&quot;,&quot;trnxId&quot;:&quot;TXN957969&quot;,&quot;fee&quot;:5,&quot;currentBalance&quot;:375}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-2465bf79-954b-4109-9325-7634f8df9711">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Customer deposit is successful</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27" aria-expanded="false" aria-controls="collapse" id="requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27" class="collapsed text-white z-block">
                    Iteration: 1 - Money withdraw by customer invalid customer no. <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27" class="collapse" aria-labelledby="requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/withdraw" target="_blank">http://dmoney.roadtocareer.net/transaction/withdraw</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 404 - Not Found</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 27ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 36B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">c54f2c97-1e39-4395-b49d-1f4814fd7d20</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">104</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-12" class="prettyPrint">{
            &quot;from_account&quot;:&quot;{{customer_phone_number4}}&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:20
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-12">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;24-dQ7qDQebbvfP5t+vS4R/Nenb2N4&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">36</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">404 Not Found</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;88</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-0285316d-2cb1-4557-8207-898310ac2b3a" class="prettyPrint">{&quot;message&quot;:&quot;Account does not exist&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-0285316d-2cb1-4557-8207-898310ac2b3a">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Status code is 404</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-8a43df4a-b198-48c8-a801-4fb030eb77d8" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8" aria-expanded="false" aria-controls="collapse" id="requests-8a43df4a-b198-48c8-a801-4fb030eb77d8" class="collapsed text-white z-block">
                    Iteration: 1 - Money withdraw by customer (10-10000) <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8" class="collapse" aria-labelledby="requests-8a43df4a-b198-48c8-a801-4fb030eb77d8">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/withdraw" target="_blank">http://dmoney.roadtocareer.net/transaction/withdraw</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 208 - Already Reported</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 21ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 43B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">216ee0ff-d16b-4994-bb03-06aaf2358df9</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">88</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-13" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01505407246&quot;,
            &quot;to_account&quot;:&quot;01708938089&quot;,
            &quot;amount&quot;:1
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-13">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;2b-3OON25YR5UIK4rYrXbJcrsd4FWo&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">43</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">208 Already Reported</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;87</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-c5511aac-07d6-49a7-9d29-190f93a339a5" class="prettyPrint">{&quot;message&quot;:&quot;Minimum withdraw amount 10 tk&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-c5511aac-07d6-49a7-9d29-190f93a339a5">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Minimum withdraw amount 10 tk</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-666dc391-1c2f-40b2-b810-3346141740c3" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-666dc391-1c2f-40b2-b810-3346141740c3" aria-expanded="false" aria-controls="collapse" id="requests-666dc391-1c2f-40b2-b810-3346141740c3" class="collapsed text-white z-block">
                    Iteration: 1 - Check customer1 balance <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-666dc391-1c2f-40b2-b810-3346141740c3" class="collapse" aria-labelledby="requests-666dc391-1c2f-40b2-b810-3346141740c3">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/balance/01505407246" target="_blank">http://dmoney.roadtocareer.net/transaction/balance/01505407246</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 15ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 40B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">31a1513d-0fce-405e-a607-3734a67275f9</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;28-Mvgh+F44zf/DaO1gsgSEKT0utEU&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">40</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">200 OK</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;86</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-cfbdba8e-1944-4485-9d96-b1c7e5a6a7f1" class="prettyPrint">{&quot;message&quot;:&quot;User balance&quot;,&quot;balance&quot;:375}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-cfbdba8e-1944-4485-9d96-b1c7e5a6a7f1">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User balance</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 200</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-8f63cbb3-27ff-42a3-8076-4b557848c563" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-8f63cbb3-27ff-42a3-8076-4b557848c563" aria-expanded="false" aria-controls="collapse" id="requests-8f63cbb3-27ff-42a3-8076-4b557848c563" class="collapsed text-white z-block">
                    Iteration: 1 - Send money to other created customer <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-8f63cbb3-27ff-42a3-8076-4b557848c563" class="collapse" aria-labelledby="requests-8f63cbb3-27ff-42a3-8076-4b557848c563">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/sendmoney" target="_blank">http://dmoney.roadtocareer.net/transaction/sendmoney</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 42ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 83B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">3913ac88-2b6a-4186-9a06-9eba8e36da86</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-15" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01505407246&quot;,
            &quot;to_account&quot;:&quot;01503689922&quot;,
            &quot;amount&quot;:40
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-15">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;53-XTgKc1Z2BRa/9vkZ7STyv9aMy+U&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">83</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;85</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-113e93af-10f0-43b1-acdf-968525b5db1f" class="prettyPrint">{&quot;message&quot;:&quot;Send money successful&quot;,&quot;trnxId&quot;:&quot;TXN8112&quot;,&quot;fee&quot;:5,&quot;currentBalance&quot;:330}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-113e93af-10f0-43b1-acdf-968525b5db1f">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Send Money is successful</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-d5a93981-540d-4b73-9f35-bb16545b181a" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-d5a93981-540d-4b73-9f35-bb16545b181a" aria-expanded="false" aria-controls="collapse" id="requests-d5a93981-540d-4b73-9f35-bb16545b181a" class="collapsed text-white z-block">
                    Iteration: 1 - Send money to other created customer  invalid account <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-d5a93981-540d-4b73-9f35-bb16545b181a" class="collapse" aria-labelledby="requests-d5a93981-540d-4b73-9f35-bb16545b181a">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/sendmoney" target="_blank">http://dmoney.roadtocareer.net/transaction/sendmoney</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 208 - Already Reported</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 18ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 56B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">ed5aec6f-9991-4c6c-9c9e-8666018a0d21</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-16" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01503689922&quot;,
            &quot;to_account&quot;:&quot;01503689922&quot;,
            &quot;amount&quot;:10
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-16">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;38-gVq4Byg+fonYJkqP5GaPVc+OjRM&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">56</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">208 Already Reported</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;84</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-08666353-a2bd-4f64-b92a-6826e02ffa2d" class="prettyPrint">{&quot;message&quot;:&quot;From account and to account cannot be same&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-08666353-a2bd-4f64-b92a-6826e02ffa2d">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >From account and to account cannot be same</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-32abf62a-d634-4e00-9eba-a685f8142fca" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-32abf62a-d634-4e00-9eba-a685f8142fca" aria-expanded="false" aria-controls="collapse" id="requests-32abf62a-d634-4e00-9eba-a685f8142fca" class="collapsed text-white z-block">
                    Iteration: 1 - Payment by customer2 <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-32abf62a-d634-4e00-9eba-a685f8142fca" class="collapse" aria-labelledby="requests-32abf62a-d634-4e00-9eba-a685f8142fca">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/payment" target="_blank">http://dmoney.roadtocareer.net/transaction/payment</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 201 - Created</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 49ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 81B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">58252904-efe4-49ee-a47e-e198251d9817</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-17" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01503689922&quot;,
            &quot;to_account&quot;:&quot;01686606905&quot;,
            &quot;amount&quot;:10
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-17">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;51-y4uwp/1qvrtg50eiMGzk0fBwslQ&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">81</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">201 Created</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;83</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-2b68a8d1-0c80-407a-a8b3-cff3c680f7af" class="prettyPrint">{&quot;message&quot;:&quot;Payment successful&quot;,&quot;trnxId&quot;:&quot;TXN437483&quot;,&quot;fee&quot;:5,&quot;currentBalance&quot;:25}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-2b68a8d1-0c80-407a-a8b3-cff3c680f7af">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >Payment successful</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-95420692-cbb9-4a2b-b66b-6631fc77a101" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-95420692-cbb9-4a2b-b66b-6631fc77a101" aria-expanded="false" aria-controls="collapse" id="requests-95420692-cbb9-4a2b-b66b-6631fc77a101" class="collapsed text-white z-block">
                    Iteration: 1 - Payment by customer2 invalid account <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-95420692-cbb9-4a2b-b66b-6631fc77a101" class="collapse" aria-labelledby="requests-95420692-cbb9-4a2b-b66b-6631fc77a101">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> POST</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/payment" target="_blank">http://dmoney.roadtocareer.net/transaction/payment</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 208 - Already Reported</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 18ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 56B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Type</td>
                                                        <td class="text-wrap">application/json</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">385e5aed-cfbc-4fa5-91df-4b65529ef349</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Content-Length</td>
                                                        <td class="text-wrap">89</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Body</h5>
                                        <div class="dyn-height">
                                            <pre><code id="copyReqText-18" class="prettyPrint">{
            &quot;from_account&quot;:&quot;01686606905&quot;,
            &quot;to_account&quot;:&quot;01686606905&quot;,
            &quot;amount&quot;:10
        }</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyReqText-18">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;38-gVq4Byg+fonYJkqP5GaPVc+OjRM&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">56</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">208 Already Reported</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;82</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-b0c4eca2-1bd1-47ca-a8b3-7b4d6777fb14" class="prettyPrint">{&quot;message&quot;:&quot;From account and to account cannot be same&quot;}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-b0c4eca2-1bd1-47ca-a8b3-7b4d6777fb14">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >From account and to account cannot be same</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">1</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-1400d117-6cbe-44ed-a9ba-eacd1dc41099" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099" aria-expanded="false" aria-controls="collapse" id="requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099" class="collapsed text-white z-block">
                    Iteration: 1 - Check customer2 balance <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099" class="collapse" aria-labelledby="requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/balance/01503689922" target="_blank">http://dmoney.roadtocareer.net/transaction/balance/01503689922</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 16ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 39B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">3a09fd88-0ce3-440e-a9d1-3ebe9a12bb32</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:37 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;27-ceo7UvXhlPR9DtEslMm/QxRbvpY&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">39</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">200 OK</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;81</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-f99c727e-68ef-490f-837c-ad3d4418d992" class="prettyPrint">{&quot;message&quot;:&quot;User balance&quot;,&quot;balance&quot;:25}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-f99c727e-68ef-490f-837c-ad3d4418d992">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User balance</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 200</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
            <div id="folder-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91" class="card-deck iteration-0">
            <div class="row iteration-0">
                <div class="col-sm-12 mb-3 iteration-0">
                <div class="card iteration-0">
                    <div class="card-header  bg-success iteration-0">
                        <a data-toggle="collapse" href="#" data-target="#collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91" aria-expanded="false" aria-controls="collapse" id="requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91" class="collapsed text-white z-block">
                    Iteration: 1 - Check merchant balance <i class="float-lg-right fa fa-chevron-down" style="padding-top: 5px;"></i>
                </a>
                    </div>
                    <div id="collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91" class="collapse" aria-labelledby="requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Request Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request Method:</strong> <span class="badge-outline-success badge badge-success"> GET</span><br>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Request URL:</strong> <a href="http://dmoney.roadtocareer.net/transaction/balance/01686606905" target="_blank">http://dmoney.roadtocareer.net/transaction/balance/01686606905</a><br>
                                    </div>
                                </div>
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Information</h5>
                                    <span><i class="fas fa-info-circle"></i></span><strong> Response Code:</strong> <span class="float-right badge-outline badge badge-success"> 200 - OK</span><br>
                                    <span><i class="fas fa-stopwatch"></i></span><strong> Mean time per request:</strong> <span class="float-right badge-outline badge badge-success"> 28ms</span><br>
                                    <span><i class="fas fa-database"></i></span><strong> Mean size per request:</strong> <span class="float-right badge-outline badge badge-success"> 46B</span><br>
                                    <hr>
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Test Pass Percentage</h5>
                                    <div>
                                        <div class="progress" style="height: 40px;">
                                            <div class="progress-bar  bg-success" style="width: 100%" role="progressbar">
                                            <h5 style="padding-top:5px;"><strong>100 %</strong></h5>
                                            </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-sm-12 mb-3">
                                <div class="card-deck">
                                <div class="card border-info" style="width: 50rem;">
                                    <div class="card-body">
                                        <h5 class="card-title text-uppercase text-white text-center bg-info">Request Headers</h5>
                                        <div class="table-responsive">
                                            <table class="table table-bordered">
                                            <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                                <tbody>
                                                    <tr>
                                                        <td class="text-nowrap">Authorization</td>
                                                        <td class="text-wrap">eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImFkbWluQHJvYWR0b2NhcmVlci5uZXQiLCJwYXNzd29yZCI6IjEyMzQiLCJpYXQiOjE2OTMzMDgzMzUsImV4cCI6MTY5MzMxMDEzNX0.I0GMKUocV6aKbdgdFtazOpVxalDP4u931pr4cU8wR9c</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">X-AUTH-SECRET-KEY</td>
                                                        <td class="text-wrap">ROADTOSDET</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">User-Agent</td>
                                                        <td class="text-wrap">PostmanRuntime/7.29.0</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept</td>
                                                        <td class="text-wrap">*/*</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Cache-Control</td>
                                                        <td class="text-wrap">no-cache</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Postman-Token</td>
                                                        <td class="text-wrap">bf5a572f-2fc6-4be4-8589-7ad72f5b7a45</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Host</td>
                                                        <td class="text-wrap">dmoney.roadtocareer.net</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Accept-Encoding</td>
                                                        <td class="text-wrap">gzip, deflate, br</td>
                                                    </tr>
                                                    <tr>
                                                        <td class="text-nowrap">Connection</td>
                                                        <td class="text-wrap">keep-alive</td>
                                                    </tr>
                                                </tbody>
                                            </table>
                                        </div>
                                    </div>
                                </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Headers</h5>
                                    <div class="table-responsive">
                                        <table class="table table-bordered">
                                        <thead class="thead-light text-center"><tr><th>Header Name</th><th>Header Value</th></tr></thead>
                                            <tbody>
                                                <tr>
                                                    <td class="text-nowrap">Date</td>
                                                    <td class="text-wrap">Tue, 29 Aug 2023 11:25:38 GMT</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Server</td>
                                                    <td class="text-wrap">Apache</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">X-Powered-By</td>
                                                    <td class="text-wrap">Express, Phusion Passenger(R) 6.0.18</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Access-Control-Allow-Origin</td>
                                                    <td class="text-wrap">*</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">ETag</td>
                                                    <td class="text-wrap">W/&quot;2e-f2P7D915Io3JcnsCjSMZGpdJ6jE&quot;</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Length</td>
                                                    <td class="text-wrap">46</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Status</td>
                                                    <td class="text-wrap">200 OK</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Keep-Alive</td>
                                                    <td class="text-wrap">timeout&#x3D;5, max&#x3D;80</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Connection</td>
                                                    <td class="text-wrap">Keep-Alive</td>
                                                </tr>
                                                <tr>
                                                    <td class="text-nowrap">Content-Type</td>
                                                    <td class="text-wrap">application/json; charset&#x3D;utf-8</td>
                                                </tr>
                                            </tbody>
                                        </table>
                                    </div>
                                </div>
                            </div>
                            </div>
                        </div>
                        </div>
                        <div class="row">
                        <div class="col-sm-12 mb-3">
                            <div class="card-deck">
                            <div class="card border-info" style="width: 50rem;">
                                <div class="card-body">
                                    <h5 class="card-title text-uppercase text-white text-center bg-info">Response Body</h5>
                                        <div class="dyn-height">
                                                <pre><code id="copyText-e7c668fc-0778-4cf0-a401-9ce6b00318ae" class="prettyPrint">{&quot;message&quot;:&quot;User balance&quot;,&quot;balance&quot;:353262.88}</code></pre>
                                        </div>
                                        <div class="card-footer">
                                            <button class="btn btn-outline-secondary btn-sm copyButton" type="button" data-clipboard-action="copy" data-clipboard-target="#copyText-e7c668fc-0778-4cf0-a401-9ce6b00318ae">Copy to Clipboard</button>
                                        </div>
                                </div>
                            </div>
                            </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="card border-info">
                                <div class="card-body">
                                <h5 class="card-title text-uppercase text-white text-center bg-info">Test Information</h5>
                                    <div class="table-responsive text-nowrap">
                                        <table class="datatable table table-hover">
                                        <thead><tr class="text-center"><th>Name</th><th>Passed</th><th>Failed</th><th>Skipped</th></tr></thead>
                                            <tbody>
                                                <tr >
                                                    <td >User balance</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                                <tr >
                                                    <td >Status code is 200</td>
                                                    <td class="text-center bg-success">1</td>
                                                    <td class="text-center ">0</td>
                                                    <td class="text-center ">0</td>
                                                </tr>
                                            </tbody>
                                            <tfoot>
                                                <tr class="bg-light">
                                                    <td><strong>Total</strong></td>
                                                    <td class="text-center">2</td>
                                                    <td class="text-center">0</td>
                                                    <td class="text-center">0</td>
                                                </tr>
                                            </tfoot>
                                        </table>
                                    </div>
                                    <div class="row d-none">
                                    <div class="col-sm-12 mb-3">
                                        <div class="card-deck">
                                        <div class="card border-danger" style="width: 50rem;">
                                            <div class="card-body">
                                                <h5 class="card-title text-uppercase text-white text-center bg-danger">Test Failure</h5>
                                                <div class="table-responsive">
                                                    <table class="table table-hover">
                                                    <thead><tr class="text-nowrap"><th>Test Name</th><th>Assertion Error</th></tr></thead>
                                                        <tbody>
                                                        </tbody>
                                                    </table>
                                                </div>
                                            </div>
                                        </div>
                                        </div>
                                    </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
    </div>
    </div>
    </div>
    </div>
    </div>


<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.2.1/js/bootstrap.bundle.min.js"></script>
<script src="https://cdn.datatables.net/v/bs4/dt-1.10.18/datatables.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.0/clipboard.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/remarkable/1.7.1/remarkable.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.2/highlight.min.js"></script>
<script>hljs.initHighlightingOnLoad();</script>

<!-- Set slider initial position depending on the localstorage state -->

<script>
(function () {
  var sliderChecked = true;
  if (localStorage.getItem('theme') === 'theme-light') {
    setTheme('theme-light');
    sliderChecked = false;
  } else {
    setTheme('theme-dark');
    sliderChecked = true;
  }
  $(document).ready( function () {
    document.getElementById('slider').checked = sliderChecked;
  });
})();
</script>

<!-- Data Table Configuration -->

<script>
$(document).ready( function () {
    $('.datatable').DataTable({
        "retrieve": true,
        "paging": false,
        "info": false,
        "fixedColumns":   {
            "heightMatch": 'none'
        }
    });
});
</script>

<!-- Tooltip Configuration -->

<script>
$(document).ready(function() {
    $('[data-toggle="tooltip"]').tooltip({
        trigger : 'hover'
    })
})
</script>

<!-- Show/Hide The Folders -->

<script>
$('#openAll').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#folder-7790913c-3864-4c2e-b394-7b664064a051-iteration-0').removeClass('collapsed')
            $('#folder-collapse-7790913c-3864-4c2e-b394-7b664064a051-iteration-0').addClass('show')
        $('#openAll').html("Collapse Folders");
        break;
    case 2:
            $('#folder-7790913c-3864-4c2e-b394-7b664064a051-iteration-0').addClass('collapsed')
            $('#folder-collapse-7790913c-3864-4c2e-b394-7b664064a051-iteration-0').removeClass('show')
        $('#openAll').html("Expand Folders");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Requests -->

<script>
$('#openAllRequests').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#requests-fcece535-4118-4b27-891b-a8c911607358').removeClass('collapsed')
            $('#collapse-fcece535-4118-4b27-891b-a8c911607358').removeClass('collapsed')
            $('#requests-fcece535-4118-4b27-891b-a8c911607358').addClass('show')
            $('#collapse-fcece535-4118-4b27-891b-a8c911607358').addClass('show')
            $('#requests-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('collapsed')
            $('#collapse-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('collapsed')
            $('#requests-365fcc48-f716-480a-b216-d5488b1677d9').addClass('show')
            $('#collapse-365fcc48-f716-480a-b216-d5488b1677d9').addClass('show')
            $('#requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('collapsed')
            $('#collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('collapsed')
            $('#requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('show')
            $('#collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('show')
            $('#requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('collapsed')
            $('#collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('collapsed')
            $('#requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('show')
            $('#collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('show')
            $('#requests-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('collapsed')
            $('#collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('collapsed')
            $('#requests-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('show')
            $('#collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('show')
            $('#requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('collapsed')
            $('#collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('collapsed')
            $('#requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('show')
            $('#collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('show')
            $('#requests-274e566a-ec91-4926-834f-99df62950d47').removeClass('collapsed')
            $('#collapse-274e566a-ec91-4926-834f-99df62950d47').removeClass('collapsed')
            $('#requests-274e566a-ec91-4926-834f-99df62950d47').addClass('show')
            $('#collapse-274e566a-ec91-4926-834f-99df62950d47').addClass('show')
            $('#requests-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('collapsed')
            $('#collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('collapsed')
            $('#requests-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('show')
            $('#collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('show')
            $('#requests-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('collapsed')
            $('#collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('collapsed')
            $('#requests-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('show')
            $('#collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('show')
            $('#requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('collapsed')
            $('#collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('collapsed')
            $('#requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('show')
            $('#collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('show')
            $('#requests-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('collapsed')
            $('#collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('collapsed')
            $('#requests-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('show')
            $('#collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('show')
            $('#requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('collapsed')
            $('#collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('collapsed')
            $('#requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('show')
            $('#collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('show')
            $('#requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('collapsed')
            $('#collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('collapsed')
            $('#requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('show')
            $('#collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('show')
            $('#requests-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('collapsed')
            $('#collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('collapsed')
            $('#requests-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('show')
            $('#collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('show')
            $('#requests-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('collapsed')
            $('#collapse-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('collapsed')
            $('#requests-666dc391-1c2f-40b2-b810-3346141740c3').addClass('show')
            $('#collapse-666dc391-1c2f-40b2-b810-3346141740c3').addClass('show')
            $('#requests-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('collapsed')
            $('#collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('collapsed')
            $('#requests-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('show')
            $('#collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('show')
            $('#requests-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('collapsed')
            $('#collapse-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('collapsed')
            $('#requests-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('show')
            $('#collapse-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('show')
            $('#requests-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('collapsed')
            $('#collapse-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('collapsed')
            $('#requests-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('show')
            $('#collapse-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('show')
            $('#requests-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('collapsed')
            $('#collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('collapsed')
            $('#requests-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('show')
            $('#collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('show')
            $('#requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('collapsed')
            $('#collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('collapsed')
            $('#requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('show')
            $('#collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('show')
            $('#requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('collapsed')
            $('#collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('collapsed')
            $('#requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('show')
            $('#collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('show')
        $('#openAllRequests').html("Collapse Requests");
        break;
    case 2:
            $('#requests-fcece535-4118-4b27-891b-a8c911607358').addClass('collapsed')
            $('#collapse-fcece535-4118-4b27-891b-a8c911607358').addClass('collapsed')
            $('#requests-fcece535-4118-4b27-891b-a8c911607358').removeClass('show')
            $('#collapse-fcece535-4118-4b27-891b-a8c911607358').removeClass('show')
            $('#requests-365fcc48-f716-480a-b216-d5488b1677d9').addClass('collapsed')
            $('#collapse-365fcc48-f716-480a-b216-d5488b1677d9').addClass('collapsed')
            $('#requests-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('show')
            $('#collapse-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('show')
            $('#requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('collapsed')
            $('#collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('collapsed')
            $('#requests-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('show')
            $('#collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('show')
            $('#requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('collapsed')
            $('#collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('collapsed')
            $('#requests-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('show')
            $('#collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('show')
            $('#requests-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('collapsed')
            $('#collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('collapsed')
            $('#requests-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('show')
            $('#collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('show')
            $('#requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('collapsed')
            $('#collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('collapsed')
            $('#requests-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('show')
            $('#collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('show')
            $('#requests-274e566a-ec91-4926-834f-99df62950d47').addClass('collapsed')
            $('#collapse-274e566a-ec91-4926-834f-99df62950d47').addClass('collapsed')
            $('#requests-274e566a-ec91-4926-834f-99df62950d47').removeClass('show')
            $('#collapse-274e566a-ec91-4926-834f-99df62950d47').removeClass('show')
            $('#requests-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('collapsed')
            $('#collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('collapsed')
            $('#requests-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('show')
            $('#collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('show')
            $('#requests-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('collapsed')
            $('#collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('collapsed')
            $('#requests-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('show')
            $('#collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('show')
            $('#requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('collapsed')
            $('#collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('collapsed')
            $('#requests-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('show')
            $('#collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('show')
            $('#requests-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('collapsed')
            $('#collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('collapsed')
            $('#requests-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('show')
            $('#collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('show')
            $('#requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('collapsed')
            $('#collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('collapsed')
            $('#requests-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('show')
            $('#collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('show')
            $('#requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('collapsed')
            $('#collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('collapsed')
            $('#requests-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('show')
            $('#collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('show')
            $('#requests-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('collapsed')
            $('#collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('collapsed')
            $('#requests-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('show')
            $('#collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('show')
            $('#requests-666dc391-1c2f-40b2-b810-3346141740c3').addClass('collapsed')
            $('#collapse-666dc391-1c2f-40b2-b810-3346141740c3').addClass('collapsed')
            $('#requests-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('show')
            $('#collapse-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('show')
            $('#requests-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('collapsed')
            $('#collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('collapsed')
            $('#requests-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('show')
            $('#collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('show')
            $('#requests-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('collapsed')
            $('#collapse-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('collapsed')
            $('#requests-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('show')
            $('#collapse-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('show')
            $('#requests-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('collapsed')
            $('#collapse-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('collapsed')
            $('#requests-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('show')
            $('#collapse-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('show')
            $('#requests-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('collapsed')
            $('#collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('collapsed')
            $('#requests-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('show')
            $('#collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('show')
            $('#requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('collapsed')
            $('#collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('collapsed')
            $('#requests-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('show')
            $('#collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('show')
            $('#requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('collapsed')
            $('#collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('collapsed')
            $('#requests-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('show')
            $('#collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('show')
        $('#openAllRequests').html("Expand Requests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Skipped Tests -->

<script>
$('#openAllSkipped').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
switch (clickCount){
    case 1:
            $('#skipped-fcece535-4118-4b27-891b-a8c911607358').removeClass('collapsed')
            $('#skipped-collapse-fcece535-4118-4b27-891b-a8c911607358').removeClass('collapsed')
            $('#skipped-fcece535-4118-4b27-891b-a8c911607358').addClass('show')
            $('#skipped-collapse-fcece535-4118-4b27-891b-a8c911607358').addClass('show')
            $('#skipped-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('collapsed')
            $('#skipped-collapse-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('collapsed')
            $('#skipped-365fcc48-f716-480a-b216-d5488b1677d9').addClass('show')
            $('#skipped-collapse-365fcc48-f716-480a-b216-d5488b1677d9').addClass('show')
            $('#skipped-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('collapsed')
            $('#skipped-collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('collapsed')
            $('#skipped-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('show')
            $('#skipped-collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('show')
            $('#skipped-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('collapsed')
            $('#skipped-collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('collapsed')
            $('#skipped-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('show')
            $('#skipped-collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('show')
            $('#skipped-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('collapsed')
            $('#skipped-collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('collapsed')
            $('#skipped-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('show')
            $('#skipped-collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('show')
            $('#skipped-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('collapsed')
            $('#skipped-collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('collapsed')
            $('#skipped-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('show')
            $('#skipped-collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('show')
            $('#skipped-274e566a-ec91-4926-834f-99df62950d47').removeClass('collapsed')
            $('#skipped-collapse-274e566a-ec91-4926-834f-99df62950d47').removeClass('collapsed')
            $('#skipped-274e566a-ec91-4926-834f-99df62950d47').addClass('show')
            $('#skipped-collapse-274e566a-ec91-4926-834f-99df62950d47').addClass('show')
            $('#skipped-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('collapsed')
            $('#skipped-collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('collapsed')
            $('#skipped-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('show')
            $('#skipped-collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('show')
            $('#skipped-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('collapsed')
            $('#skipped-collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('collapsed')
            $('#skipped-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('show')
            $('#skipped-collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('show')
            $('#skipped-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('collapsed')
            $('#skipped-collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('collapsed')
            $('#skipped-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('show')
            $('#skipped-collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('show')
            $('#skipped-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('collapsed')
            $('#skipped-collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('collapsed')
            $('#skipped-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('show')
            $('#skipped-collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('show')
            $('#skipped-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('collapsed')
            $('#skipped-collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('collapsed')
            $('#skipped-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('show')
            $('#skipped-collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('show')
            $('#skipped-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('collapsed')
            $('#skipped-collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('collapsed')
            $('#skipped-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('show')
            $('#skipped-collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('show')
            $('#skipped-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('collapsed')
            $('#skipped-collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('collapsed')
            $('#skipped-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('show')
            $('#skipped-collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('show')
            $('#skipped-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('collapsed')
            $('#skipped-collapse-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('collapsed')
            $('#skipped-666dc391-1c2f-40b2-b810-3346141740c3').addClass('show')
            $('#skipped-collapse-666dc391-1c2f-40b2-b810-3346141740c3').addClass('show')
            $('#skipped-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('collapsed')
            $('#skipped-collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('collapsed')
            $('#skipped-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('show')
            $('#skipped-collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('show')
            $('#skipped-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('collapsed')
            $('#skipped-collapse-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('collapsed')
            $('#skipped-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('show')
            $('#skipped-collapse-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('show')
            $('#skipped-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('collapsed')
            $('#skipped-collapse-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('collapsed')
            $('#skipped-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('show')
            $('#skipped-collapse-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('show')
            $('#skipped-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('collapsed')
            $('#skipped-collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('collapsed')
            $('#skipped-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('show')
            $('#skipped-collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('show')
            $('#skipped-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('collapsed')
            $('#skipped-collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('collapsed')
            $('#skipped-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('show')
            $('#skipped-collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('show')
            $('#skipped-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('collapsed')
            $('#skipped-collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('collapsed')
            $('#skipped-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('show')
            $('#skipped-collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('show')
        $('#openAllSkipped').html("Collapse All Skipped Tests");
        break;
    case 2:
            $('#skipped-fcece535-4118-4b27-891b-a8c911607358').addClass('collapsed')
            $('#skipped-collapse-fcece535-4118-4b27-891b-a8c911607358').addClass('collapsed')
            $('#skipped-fcece535-4118-4b27-891b-a8c911607358').removeClass('show')
            $('#skipped-collapse-fcece535-4118-4b27-891b-a8c911607358').removeClass('show')
            $('#skipped-365fcc48-f716-480a-b216-d5488b1677d9').addClass('collapsed')
            $('#skipped-collapse-365fcc48-f716-480a-b216-d5488b1677d9').addClass('collapsed')
            $('#skipped-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('show')
            $('#skipped-collapse-365fcc48-f716-480a-b216-d5488b1677d9').removeClass('show')
            $('#skipped-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('collapsed')
            $('#skipped-collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').addClass('collapsed')
            $('#skipped-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('show')
            $('#skipped-collapse-8e43d38b-c2e2-488f-a3a8-6598af9398ea').removeClass('show')
            $('#skipped-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('collapsed')
            $('#skipped-collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').addClass('collapsed')
            $('#skipped-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('show')
            $('#skipped-collapse-ce041859-fd77-4e0b-b4ce-f4bbd80ffa77').removeClass('show')
            $('#skipped-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('collapsed')
            $('#skipped-collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').addClass('collapsed')
            $('#skipped-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('show')
            $('#skipped-collapse-b3bbb584-3b43-4158-86e7-86c9c288145d').removeClass('show')
            $('#skipped-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('collapsed')
            $('#skipped-collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').addClass('collapsed')
            $('#skipped-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('show')
            $('#skipped-collapse-bac5453f-810a-4e4b-b3c4-54d33ecd596c').removeClass('show')
            $('#skipped-274e566a-ec91-4926-834f-99df62950d47').addClass('collapsed')
            $('#skipped-collapse-274e566a-ec91-4926-834f-99df62950d47').addClass('collapsed')
            $('#skipped-274e566a-ec91-4926-834f-99df62950d47').removeClass('show')
            $('#skipped-collapse-274e566a-ec91-4926-834f-99df62950d47').removeClass('show')
            $('#skipped-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('collapsed')
            $('#skipped-collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').addClass('collapsed')
            $('#skipped-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('show')
            $('#skipped-collapse-9821549c-0cd5-4af3-9a72-f09a48b9b909').removeClass('show')
            $('#skipped-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('collapsed')
            $('#skipped-collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').addClass('collapsed')
            $('#skipped-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('show')
            $('#skipped-collapse-a88996bc-acbd-45bf-ad63-2862da5ba58a').removeClass('show')
            $('#skipped-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('collapsed')
            $('#skipped-collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').addClass('collapsed')
            $('#skipped-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('show')
            $('#skipped-collapse-d0cadf5b-0cda-4d24-923c-b0dc09ee777e').removeClass('show')
            $('#skipped-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('collapsed')
            $('#skipped-collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').addClass('collapsed')
            $('#skipped-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('show')
            $('#skipped-collapse-c809d899-c8e4-4294-9e25-27b6ccb7487d').removeClass('show')
            $('#skipped-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('collapsed')
            $('#skipped-collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').addClass('collapsed')
            $('#skipped-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('show')
            $('#skipped-collapse-6c9848c7-f920-439e-ac54-2ee7fa72f16c').removeClass('show')
            $('#skipped-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('collapsed')
            $('#skipped-collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').addClass('collapsed')
            $('#skipped-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('show')
            $('#skipped-collapse-a74f7b27-eeb7-4417-b8d4-eaced8ff7c27').removeClass('show')
            $('#skipped-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('collapsed')
            $('#skipped-collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').addClass('collapsed')
            $('#skipped-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('show')
            $('#skipped-collapse-8a43df4a-b198-48c8-a801-4fb030eb77d8').removeClass('show')
            $('#skipped-666dc391-1c2f-40b2-b810-3346141740c3').addClass('collapsed')
            $('#skipped-collapse-666dc391-1c2f-40b2-b810-3346141740c3').addClass('collapsed')
            $('#skipped-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('show')
            $('#skipped-collapse-666dc391-1c2f-40b2-b810-3346141740c3').removeClass('show')
            $('#skipped-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('collapsed')
            $('#skipped-collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').addClass('collapsed')
            $('#skipped-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('show')
            $('#skipped-collapse-8f63cbb3-27ff-42a3-8076-4b557848c563').removeClass('show')
            $('#skipped-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('collapsed')
            $('#skipped-collapse-d5a93981-540d-4b73-9f35-bb16545b181a').addClass('collapsed')
            $('#skipped-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('show')
            $('#skipped-collapse-d5a93981-540d-4b73-9f35-bb16545b181a').removeClass('show')
            $('#skipped-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('collapsed')
            $('#skipped-collapse-32abf62a-d634-4e00-9eba-a685f8142fca').addClass('collapsed')
            $('#skipped-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('show')
            $('#skipped-collapse-32abf62a-d634-4e00-9eba-a685f8142fca').removeClass('show')
            $('#skipped-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('collapsed')
            $('#skipped-collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').addClass('collapsed')
            $('#skipped-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('show')
            $('#skipped-collapse-95420692-cbb9-4a2b-b66b-6631fc77a101').removeClass('show')
            $('#skipped-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('collapsed')
            $('#skipped-collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').addClass('collapsed')
            $('#skipped-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('show')
            $('#skipped-collapse-1400d117-6cbe-44ed-a9ba-eacd1dc41099').removeClass('show')
            $('#skipped-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('collapsed')
            $('#skipped-collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').addClass('collapsed')
            $('#skipped-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('show')
            $('#skipped-collapse-53fdf6f6-5e2d-4232-9a8c-1afa88d43b91').removeClass('show')
        $('#openAllSkipped').html("Expand All Skipped Tests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Show/Hide The Failures -->

<script>
$('#openAllFailed').on('click', function(e) {
let clickCount = $(this).data("clickCount") || 1
let failedItemContent
let failedItemHeading
switch (clickCount){
    case 1:
            failedItemHeading = $('#fails-75beb489-1ae7-4c12-aca3-68b6dc31bc44');
            failedItemContent = $("#fails-collapse-75beb489-1ae7-4c12-aca3-68b6dc31bc44");
            failedItemHeading.removeClass('collapsed')
            failedItemContent.removeClass('collapsed')
            failedItemHeading.addClass('show')
            failedItemContent.addClass('show')
        $('#openAllFailed').html("Collapse All Failed Tests");
        break;
    case 2:
            failedItemHeading = $('#fails-75beb489-1ae7-4c12-aca3-68b6dc31bc44');
            failedItemContent = $("#fails-collapse-75beb489-1ae7-4c12-aca3-68b6dc31bc44");
            failedItemHeading.removeClass('show')
            failedItemContent.removeClass('show')
            failedItemHeading.addClass('collapsed')
            failedItemContent.addClass('collapsed')
        $('#openAllFailed').html("Expand All Failed Tests");
        break;
}
clickCount = clickCount > 1 ? 1 : ++clickCount;
$(this).data("clickCount", clickCount)
})
</script>

<!-- Pretty Print the Response Body-->

<script>
function isJSON(data)
{
    var ret = true;
    try {
            JSON.parse(data);
    }catch(e) {
            ret = false;
    }
    return ret;
}

function isXML(data)
{
    return (data.length > 0 && data[0] === '<');
}

// see https://gist.github.com/sente/1083506/d2834134cd070dbcc08bf42ee27dabb746a1c54d#gistcomment-2254622
function formatXML(data) {
    const PADDING = ' '.repeat(2); // set desired indent size here
    const reg = /(>)(<)(\/*)/g;
    let pad = 0;
    xml = data.replace(reg, '$1\r\n$2$3');

    return xml.split('\r\n').map((node, index) => {
        let indent = 0;
        if (node.match(/.+<\/\w[^>]*>$/)) {
            indent = 0;
        } else if (node.match(/^<\/\w/) && pad > 0) {
            pad -= 1;
        } else if (node.match(/^<\w[^>]*[^\/]>.*$/)) {
            indent = 1;
        } else {
            indent = 0;
        }

        pad += indent;
        return PADDING.repeat(pad - indent) + node;
    }).join('\r\n');
}

$(".prettyPrint").each(function () {
        var data = $(this).text();
        // Verify whether data is JSON
        if(isJSON(data))
        {
                obj = JSON.parse(data);
                data = JSON.stringify(obj, null, 2);
        }
        else if(isXML(data)) {
            data = formatXML(data);
        }
        $(this).text(data);
});
</script>


<!-- Copy Response Body To Clipboard -->

<script>
    var clipboard = new ClipboardJS('.copyButton');

    clipboard.on('success', function(e) {
        e.clearSelection();
        $(".copyButton").addClass("bg-success text-white")
        e.trigger.textContent = '✔ Copied!';
        window.setTimeout(function() {
            $(".copyButton").removeClass("bg-success text-white")
            e.trigger.textContent = 'Copy to Clipboard';
        }, 2000);
    });
    clipboard.on('error', function(e) {
        e.clearSelection();
        $(".copyButton").addClass("bg-danger text-white")
        e.trigger.textContent = '✗ Not Copied';
        window.setTimeout(function() {
            $(".copyButton").removeClass("bg-danger text-white")
            e.trigger.textContent = 'Copy to Clipboard';
        }, 2000);
    });

</script>

<!-- Render the Description Markdown and link in the test failures -->

<script>
    const remarkable = new Remarkable();

    const descriptions = document.querySelectorAll(".renderMarkdown");
    descriptions.forEach(description => {
        description.innerHTML = renderHtmlFromMarkdown(description.textContent);
    });
    function renderHtmlFromMarkdown(markdown) {
        return remarkable.render(trim(markdown));
    }
    function trim(string) {
        return string ? string.replace(/^ +| +$/gm, "") : string;
    }
</script>

<!-- Show/Hide The Toggles When Scrolling The Page -->

<script>
window.onscroll = function() {scrollFunction()};

function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    document.getElementById("topOfRequestsScreen").style.display = "block";
    document.getElementById("topOfFailuresScreen").style.display = "block";
    document.getElementById("topOfSkippedScreen").style.display = "block";
    document.getElementById("openAll").style.display = "none";
    document.getElementById("openAllRequests").style.display = "none";


    document.getElementById("showOnlyFailures").style.display = "none";
    document.getElementById("openAllFailed").style.display = "none";
  } else {
    document.getElementById("topOfRequestsScreen").style.display = "none";
    document.getElementById("topOfFailuresScreen").style.display = "none";
    document.getElementById("topOfSkippedScreen").style.display = "none";
    document.getElementById("openAll").style.display = "block";
    document.getElementById("openAllRequests").style.display = "block";

    document.getElementById("showOnlyFailures").style.display = "block";
    document.getElementById("openAllFailed").style.display = "block";
  }
}

function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
</script>

<!-- Creates The Iteration Tabs -->

<script type="text/javascript">
    "use strict";

window.onload = function () {

  // set display for all blocks of response
  var allItems = document.querySelectorAll('[class*=iteration-]');
  allItems.forEach(function(elem){
    elem.style.display = 'block';
  });

   
  let totalIterations = 1;
   

  let menu = document.querySelector('#execution-menu .nav');

  for(var i = 0; i < totalIterations; i++)
  {
    let li = document.createElement('li');
    li.appendChild(document.createTextNode((i + 1)));
    li.setAttribute('id', 'iteration-' + i);
    li.classList.add("custom-tab");
    li.classList.add("itPassed");

    li.addEventListener('click', function() {
      //set display to none for all except row
      let allItems = document.querySelectorAll('[class*=iteration-]:not(.row)');
      allItems.forEach(function(elem) {
        elem.style.display = 'none';
      })

      let allMenus = document.querySelectorAll('[id*=iteration-]');
      allMenus.forEach(function(elem){
        elem.style.borderBottom = 'none';
      })

      this.style.borderBottom = 'solid 3px #032a33';

      let items = document.querySelectorAll("." + this.id + ':not(.row)');
      items.forEach(function(elem) {
        elem.style.display = elem.style.display == 'block' ? 'none' : 'block';
      })
    });
    menu.appendChild(li);
  }

  //shows first tab data
  document.getElementById('iteration-0').click();
  document.getElementById('iterationSelected').innerHTML = `Iteration ${document.getElementById('iteration-0').innerHTML} selected`

    $("#iteration-0").removeClass('itPassed').addClass('itFailed')
}
</script>

<!-- Create the Selected Iteration Label -->

<script>
$(document).ready(function(){
    $(function() {
        $("#iterationList li").click(function() {
            document.getElementById('iterationSelected').innerHTML = "Iteration " + this.innerHTML + " selected"
        });
    });
});
</script>

<!-- Filter Action for the Iterations -->

<script>
$("#filterInput").on("input paste", function() {
    var value = $(this).val();
    $("#iterationList li").filter(function() {
	    $("#showOnlyFailures").data("clickCount") ? $("#showOnlyFailures").click():null;
        $(this).toggle($(this).text().indexOf(value) > -1)
    });
});
</script>

<!-- Showing the Failed Interations -->

<script>
$('#showOnlyFailures').on('click', function(e) {
    let clickCount = $(this).data("clickCount") || 1
	$("#filterInput").val()!="" && clickCount==1 ? $("#filterInput").val('').trigger('input'): null;
    let selectedIteration = $('#iterationList li').filter(function () {
        return $(this).css('border-bottom').indexOf("solid") > -1 && $(this).hasClass('itFailed');
    });
    selectedIteration.length || clickCount > 1 ? null : $("#iterationList li.itFailed")[0].click()
    $("#iterationList li.itPassed").toggle()
    $("div.bg-success [id*=requests]").parents('[class^="row iteration-"]').toggle();
    clickCount = clickCount > 1 ? 1 : ++clickCount;
    clickCount > 1 ? $("#showOnlyFailures").html("Show All Iterations") : $("#showOnlyFailures").html("Show Failed Iterations");
    $(this).data("clickCount", clickCount)
})
</script>
</body>
</html>
oading report.html…]()

