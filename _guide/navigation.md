---
title: Navigation
layout: default
---
<div class="toc">
	<h1><span><a href="../style-guide.html"> &laquo; Style guide</a></span>
	Navigation</h1>
</div>
<div class="description">
	<p>Navigation describes the process for moving through an application and ensuring a person understands where they are during the process.</p>
</div>
<p>Due to the complexity of the application process (particularly company registration), the user interface has been designed to cater for <em>sections within pages</em>. Rather than bombarding the user with a long list of form controls some pages are divided into logical sections. Only one section is presented at one time. Each section must contain valid data before the next section will open. Once all sections have valid data the applicant can move onto the next step in the application process.</p>
<h2>Example - step meter:</h2>
<div class="progress-container">
	<div class="progress-bar">
		<span id="progress-percent" style="width: 58%"></span>
	</div><!-- meter -->
	<ul class="section-nav">
		<li class="done"><a href="#"><span>1</span><br>Step<br> name</a></li>
		<li class="done"><a href="#"><span>2</span><br>Step<br> name</a></li>
		<li class="done"><a href="#"><span>3</span><br>Step<br> name</a></li>
		<li class="active"><span>4</span><br>Example<br> page</li>
		<li><span>5</span><br>Step<br> name</li>
		<li><span>6</span><br>Step<br> name</li>
	</ul>
</div><!-- progress-container -->
<h2 id="percentage">Example - percentage meter:</h2>
<p>In situations where there are no distinct steps or the steps are determined along the way (like the help me decide tool) just the percentage meter may be more appropriate.</p>
<p class="meter-description"><strong>Step <span id="stepNo">3</span>:</strong> <span id="percentCompleted">40</span>% complete</p>
<div class="meter">
	<span id="percentMeter" style="width: 40%;"></span>
</div>

<h1 id="heading" tabindex="-1">4. Example page heading <span>(Step 3 of 6)</span></h1>
<p>This example demonstrates how a page can be divided into multiple sections. Choices made in sections can also influence the questions that are asked in sections not yet opened. <a href="style-guide.html">Back to style guide.</a></p>
<p>Click the next button in each section to navigate through.</p>

<div id="section1-container" class="sub-section-container sub-section-open">
	<h2>Section one heading</h2>
	<div id="section1-content" class="sub-section-content">
		<fieldset>
			<legend class="margin4 larger">Section 1 details</legend>
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel1" class="input-right">Field label 1</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel1" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel2" class="input-right">Field label 2</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel2" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="question1" class="input-right">Question</label>
				</div><!-- col -->
				<div class="col8 last">
					<div class="radio-toggle">
						<label class="on label-left" for="on"><input id="on" type="radio" name="question1"><span>Yes</span></label>
						<label class="off label-right" for="off"><input id="off" type="radio" name="question1"><span>No</span></label>
					</div>
				</div><!-- col -->
			</div><!-- grid-row -->
		</fieldset>
		<div id="section1-controls" class="controls-container">
			<div class="controls-content">
				<button type="button" class="btn">Previous</button><button type="button" id="next1" class="btn btn-default next">Next</button>
				<button type="button" class="btn btn-float">Options</button><button type="button" class="btn btn-float btn-save">Save</button>
			</div><!-- controls-content -->
		</div><!-- controls-container -->
	</div><!-- sub-section-content -->
</div><!-- sub-section-container -->

<div id="section2" class="sub-section-container">
	<h2>Section two heading</h2>
	<div class="sub-section-content">
		<fieldset>
			<legend class="margin4 larger">Section 2 details</legend>
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel3" class="input-right">Field label 3</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel3" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel4" class="input-right">Field label 4</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel4" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="question2" class="input-right">Question</label>
				</div><!-- col -->
				<div class="col8 last">
					<div class="radio-toggle">
						<label class="on label-left" for="on"><input id="on" type="radio" name="question2"><span>Yes</span></label>
						<label class="off label-right" for="off"><input id="off" type="radio" name="question2"><span>No</span></label>
					</div>
				</div><!-- col -->
			</div><!-- grid-row -->
		</fieldset>
		<div class="controls-container">
			<div class="controls-content">
				<button type="button" class="btn previous">Previous</button><button type="button" class="btn btn-default next">Next</button>
				<button type="button" class="btn btn-float">Options</button><button type="button" class="btn btn-float btn-save">Save</button>
			</div><!-- controls-content -->
		</div>
	</div><!-- sub-section-content -->

</div><!-- sub-section-container -->

<div id="section3" class="sub-section-container">
	<h2>Section three heading</h2>
	<div class="sub-section-content">
		<fieldset>
			<legend class="margin4 larger">Section 3 details</legend>
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel5" class="input-right">Field label 5</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel5" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="fieldLabel6" class="input-right">Field label 6</label>
				</div><!-- col -->
				<div class="col8 last">
					<input type="text" id="fieldLabel6" />
				</div><!-- col -->
			</div><!-- grid-row -->
			<div class="grid-row">
				<div class="col4">
					<label for="question3" class="input-right">Question</label>
				</div><!-- col -->
				<div class="col8 last">
					<div class="radio-toggle">
						<label class="on label-left" for="on"><input id="on" type="radio" name="question3"><span>Yes</span></label>
						<label class="off label-right" for="off"><input id="off" type="radio" name="question3"><span>No</span></label>
					</div>
				</div><!-- col -->
			</div><!-- grid-row -->
		</fieldset>
		<div class="controls-container">
			<div class="controls-content">
				<button type="button" class="btn previous">Previous</button><button type="button" class="btn btn-default">Continue to step 5</button> <!-- last next go to next step -->
				<button type="button" class="btn btn-float">Options</button><button type="button" class="btn btn-float btn-save">Save</button>
			</div><!-- controls-content -->
		</div>
	</div><!-- sub-section-content -->

</div><!-- sub-section-container -->
