# Bootstrap Calendar #
Event calendars using twitter bootstrap and jQuery. Twitter bootstrap's calendar classes and labels and colors and jQuery's flexibility gives birth to a very robust and functional event calendars.

## Features ##
  * Debug view, visible when opened browser console.
  * Create custom jQuery functions can be customized for every cell.
  * In-cell editing.
  * Responsive girds.
  * Data fed by JSON.

## Advantages ##
  * Leverage the responsiveness of bootstrap to create html calendars.
  * Usage of jQuery to handle events on each action.
  * Can be used as an event calendar when pooled data from a mySQL DB in JSON format.
  * Pagination, Week and Month views
  * Best when used with any server side language that supports JSON encode and decode functions.

## Installation ##
  1. Add the calendarGrid.js file into your bootstrap "assets/js" folder.
  1. Create a html file and call use it as shown below.
```
<!DOCTYPE html>
<html lang="en"><head>
    <meta charset="utf-8">
    <title>jQuery Calendar</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="">
    <meta name="author" content="">
	
	<link href="assets/css/bootstrap.css" rel="stylesheet">
	<link href="assets/css/bootstrap-responsive.css" rel="stylesheet">
	<link href="assets/css/calendar.css" rel="stylesheet">
	
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.6.2/jquery.js"></script>
	<script src="assets/js/calendarGrid.js"></script>
	
	<!-- HTML5 shim, for IE6-8 support of HTML5 elements -->
    <!--[if lt IE 9]><script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->

	<script type="text/javascript">
	$(document).ready(function(){
		$("#attendance_chart").calendarGrid({
			eventFrequency:	"2",
			debugMode:		true,
			startDate:		'25-11-2012',
			endDate:		'05-01-2013',
			weekStart: 		'1',
			hoverActions:	true,
			sAjaxSource: ''
		});
	});
	</script>
</head>
<body>
<div class="container">
	<div class="row">
		<div class="span12">
			<h2>jQuery Calendar</h2>
		</div>
	</div>
	<div class="row">
		<div class="span4 well">
			&nbsp;
		</div>
		<div class="span7">
			<div id="attendance_chart">
				<div class="btn-group" data-toggle="buttons-radio">
				  <button type="button" class="btn active">Month</button>
				  <button type="button" class="btn">Week</button>
				</div>
				<ul class="pager">
				  <li class="previous">
				    <a href="#">&larr; Older</a>
				  </li>
				  <li class="next">
				    <a href="#">Newer &rarr;</a>
				  </li>
				</ul>
				<table class="table table-bordered table-condensed calendar">
					<thead>
						<tr>
							<th>Sunday</th>
							<th>Monday</th>
							<th>Tuesday</th>
							<th>Wednesday</th>
							<th>Thursday</th>
							<th>Friday</th>
							<th>Saturday</th>
						</tr>		
					</thead>
					<tbody></tbody>
				</table>
			</div>
		</div>
	</div>
</div>
<div id="footer">
  <div class="container">
    <p class="muted credit">Courtesy <a href="#">Shankar</a></p>
  </div>
</div>
</body>
</html>
```



---


## Everyone's invited ##
Developers; testers and everyone is invited, please lets contribute and start re-using instead of creating things right from scratch... please mail me or let me know if anyone is interested in contributing to this project.

Best way to contribute to this project is not by donation, but by working on the source files to make it more better.