---
title: Application summary
layout: default
---
<style>
    a.dismiss span {
        display: inline-block;
        width: 20px;
        height: 20px;
        vertical-align: middle;
    }

    p:hover a.dismiss span, a.dismiss:focus span {
        background: url(/Content/img/ico-close.png);
        background-size: cover;
    }

    a.dismiss:hover, a.dismiss:focus {
        background-color: transparent;
    }

    .inline p {
        margin: 0;
    }

    .inline {
        display: inline-block;
        margin-right: 20px;
    }	

	tr.extra {
		background-color: #eee;
		display: none;
	}
	
	tr.extra td {
		background-color: transparent;
	}
	.dashboard-container caption .app-status {
		font-size: 80%;
		margin-top: .5em;
		width: 80%;
	}
	.search-date {
		width: 7em !important;
	}
	.search-date + button.ui-datepicker-trigger {
		background: none;
		border: none;
		margin-left: -35px;
		color: #555;
	}
</style>
<main class="wrapper">
	<h1 id="heading" tabindex="-1">Application summary <a class="cd-btn help" href="#help-dashboarddescription"><span>Help - Application summary</span></a></h1>
	<div class="grid-row clearfix">
		<p>Welcome to the application summary! Here you can:</p>
		<ul>
			<li><strong>resume</strong> unfinished applications</li>
			<li><strong>track</strong> the status of applications</li>
			<li><strong>search</strong> for specific applications.</li>
		</ul>
		<p>Need help starting your business? See the business.gov.au <a href="https://www.business.gov.au/Info/Plan-and-Start/Templates-and-tools/Checklists/Starting-your-business-checklist" target="_blank">Starting your business checklist <span class="visuallyhidden">(opens in new window)</span></a>, download a <a href="https://www.business.gov.au/info/plan-and-start/templates-and-tools/business-plan-template-and-guide" target="_blank">business plan template <span class="visuallyhidden">(opens in new window)</span></a> and find the <a href="https://www.business.gov.au/info/plan-and-start/start-your-business/business-and-company-registration/registration-and-licences" target="_blank"> licences and permits <span class="visuallyhidden">(opens in new window)</span></a> you need to run your business. </p>
	</div>
	<div id="dashboard-page">
		<p>You have <strong><span id="application-count">7</span> application(s)</strong>.</p>
		<div class="card clearfix">
			<form action="/registration/dashboard/search" id="search-form" method="post" novalidate="novalidate"><input name="__RequestVerificationToken" type="hidden" value="v0HTD9yGK4oZF86SaC0U1DDBqhAbaJWP-VzqDS3U4AAWGBssoz7lI5ZHjod30AeYr4OZ4rYmS5M5qEzfzMnCivI_DM_4hQJIqgIMfI2Qw5LdNinjOxOKnVen_9cR6VQ_iC7xqeCItQCqvw6A4q8RPw2">            <fieldset id="filterContainer" class="no-margin">
                <div class="filter-container">
					<div class="grid-row">
						<div class="col4">
							<label for="search-term" class="input-right">Search for</label>
						</div>
						<div class="col7">
							<input id="SearchOptions_SearchString" name="SearchOptions.SearchString" placeholder="Australian Business Number (ABN)" style="max-width: 23em" type="text" value="">
							<button id="find-btn" type="submit" class="btn btn-default btn-inline" name="submitAction" value="stringSearch">Find applications</button><br>
							<a href="javascript:void(0)" id="show-adv">Show advanced options</a>
						</div>
						<div class="col1 last"><a class="cd-btn help" href="#help-dashboardsearchhelp"><span>Help - Search help</span></a></div>
					</div>
                    <div id="advanced-search" style="display: none;">
						<div class="grid-row">
							<div class="col4">
								<label for="SearchOptions_DateFrom" class="input-right">Submitted date from<br><span class="field-note">(DD/MM/YYYY)</span></label>
							</div>
							<div class="col8 last">
								<input class="search-date hasDatepicker" data-val="true" data-val-date="The field DateFrom must be a date." id="SearchOptions_DateFrom" name="SearchOptions.DateFrom" type="text" value=""><button type="button" class="ui-datepicker-trigger"><span class="fa fa-calendar"></span></button>
								&nbsp;&nbsp;
								<label for="SearchOptions_DateTo" class="input-right label-inline">Date to <span class="field-note">(DD/MM/YYYY)</span></label>
								<input class="search-date hasDatepicker" data-val="true" data-val-date="The field DateTo must be a date." id="SearchOptions_DateTo" name="SearchOptions.DateTo" type="text" value=""><button type="button" class="ui-datepicker-trigger"><span class="fa fa-calendar"></span></button>
							</div>
						</div>
						<div class="grid-row">
							<div class="col4">
								<label for="field5" class="input-right">Status of application</label>
							</div>
							<div class="col8 last">
								<select id="SearchOptions_SelectedApplicationStatus" name="SearchOptions.SelectedApplicationStatus"><option value="">Show all</option>
									<option value="1">Not Submitted</option>
									<option value="4">Submitted</option>
									<option value="5">Completed</option>
								</select>
								<br>
							</div>
						</div>
						<div class="grid-row clearfix">
							<div class="col4">
								<p class="label input-right">Registration types</p>
							</div>
							<div class="col8 last">
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_2" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="ABN">
										<label for="RegistrationTypes_2" id="type-abn" style="width: 8em">ABN</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_3" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="GST">
										<label for="RegistrationTypes_3" id="type-gst" style="width: 8em">GST</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_4" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="PAYG">
										<label for="RegistrationTypes_4" id="type-payg" style="width: 8em">PAYG</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_5" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="FBT">
										<label for="RegistrationTypes_5" id="type-fbt" style="width: 8em">FBT</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_6" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="LCT">
										<label for="RegistrationTypes_6" id="type-lct" style="width: 8em">LCT</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_7" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="FTC">
										<label for="RegistrationTypes_7" id="type-ftc" style="width: 8em">FTC</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_8" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="WET">
										<label for="RegistrationTypes_8" id="type-wet" style="width: 8em">WET</label>
									</p>
								</div>
								<div class="custom-controls inline">
									<p class="no-margin">

										<input id="RegistrationTypes_9" name="SearchOptions.SelectedRegistrationTypes" type="checkbox" value="AKEY">
										<label for="RegistrationTypes_9" id="type-akey" style="width: 8em">AUSKey</label>
									</p>
								</div>
							</div>
						</div>
                        <div>
                            <p class="margin4">
                                <button type="submit" class="btn btn-default btn-inline" id="btnSearch" name="submitAction" value="advancedSearch">Find applications</button>
                            </p>
                        </div>
                    </div>
                </div><!-- filterContainer -->
            </fieldset>
		</form>
	</div>
	<div id="resubmit" style="display: none;">
		<div class="dashboard-container">
			<table>
				<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
					
					<div class="app-status">
						<p class="clickable" onclick="$(this).next().toggle()">
							<a href="javascript:void(0)" class="more">Unsuccessful</a>&nbsp;<span class="fa fa-plus-square"></span>
						</p>
						<div class="extra-content" style="display: none;">
							<p>You have submitted the application and at least one of your registrations has been unsuccessful. You can use the <strong>Resume</strong> button to go back and edit the unsuccessful registration(s) and resubmit them.</p>
						</div>
					</div>
					<span class="controls">
						<a href="resubmit-auskeys2" class="edit">Resume</a>
						&nbsp;
						<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
						&nbsp;
						<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
					</span>
				</caption>
				<thead>
					<tr>
						<th class="status-item">Registration item</th>
						<th class="status-detail">Detail</th>
						<th class="status-information" colspan="2">Status</th>
					</tr>
				</thead>
				<tbody>
					<tr class="rego" onclick="$(this).next().toggle('fast')">
						<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
						<td class="status-waiting">Fred Albert Nerk</td>
						<td class="">
							<span>
								<a class="more" href="javascript:void(0)">Submitted</a>
							</span>
						</td>
						<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
					</tr>
					<tr style="display: table-row;" class="extra" style="display: none">
						<td>&nbsp;</td>
						<td colspan="3">
							<p>Your registration has been successful. Your activation code is blah blah  blah. Content.</p>
						</td>
					</tr>
					<tr class="rego" onclick="$(this).next().toggle('fast')">
						<td class="declined"><span class="visuallyhidden">Unsuccessful-</span>AUSkey</td>
						<td class="status-waiting">Simon Arthur Bourke</td>
						<td class="">
							<span><a class="more" href="javascript:void(0)">Unsuccessful</a></span>
						</td>
						<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
					</tr>
					<tr style="display: table-row;" class="extra" style="display: none">
						<td>&nbsp;</td>
						<td colspan="3">
							<p>Unfortunately your application was unable to be submitted due to the following errors:</p>
							<ul>
								<li>Invalid Tax File Number.</li>
							</ul>
							<p>You can re-submit your application by selecting the "Resume" button above and correcting the errors.</p>
						</td>
					</tr>
					<tr class="rego" onclick="$(this).next().toggle('fast')">
						<td class="declined"><span class="visuallyhidden">Unsuccessful-</span>AUSkey</td>
						<td class="status-waiting">Graham Alexander Carson</td>
						<td class="">
							<span><a class="more" href="javascript:void(0)">Unsuccessful</a></span>
						</td>
						<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
					</tr>
					<tr style="display: table-row;" class="extra" style="display: none">
						<td>&nbsp;</td>
						<td colspan="3">
							<p>Unfortunately your application was unable to be submitted due to the following errors:</p>
							<ul>
								<li>Invalid Tax File Number.</li>
							</ul>
							<p>You can re-submit your application by selecting the "Resume" button above and correcting the errors.</p>
						</td>
					</tr>
					<tr class="rego" onclick="$(this).next().toggle('fast')">
						<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
						<td class="status-waiting">Bryan Jeremy Cartright</td>
						<td class="">
							<span>
								<a class="more" href="javascript:void(0)">Submitted</a>
							</span>
						</td>
						<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
					</tr>
					<tr style="display: table-row;" class="extra" style="display: none">
						<td>&nbsp;</td>
						<td colspan="3">
							<p>Your registration has been successful. Your activation code is blah blah  blah. Content.</p>
						</td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>
<div id="add-auskeys" style="display: none">
	<div class="dashboard-container" id="299">
		<table id="auskey-pending">
			<caption>Application reference: <strong>#1702-AA-0299-L</strong><br>
				<div class="app-status"><p>Submitted on 09 May 2017 14:32</p></div>
				<span class="controls">
					<a href="javascript:void(0);" class="edit" style="display: none;">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="waiting"><span class="visuallyhidden">Pending-</span>AUSkey</td>
					<td class="status-waiting">Fred Albert Nerk</td>
					<td class=""><a href="javascript:void(0)">Pending</a></td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Use the refresh button above to check on the status of your application.</p>
					</td>
				</tr>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="waiting"><span class="visuallyhidden">Pending-</span>AUSkey</td>
					<td class="status-waiting">Simon Arthur Bourke</td>
					<td class=""><a href="javascript:void(0)">Pending</a></td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Use the refresh button above to check on the status of your application.</p>
					</td>
				</tr>
			</tbody>
		</table>
		<table id="new-auskeys" style="display: none;">
			<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
				
				<div class="app-status"><p>Not submitted</p></div>
				<span class="controls">
					<a href="register-existing5" class="edit">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				
				<tr class="rego">
					<td class="editing"><span class="visuallyhidden">Not submitted-</span>AUSkey</td>
					<td class="status-waiting">Fred Albert Nerk</td>
					<td class="">
						<span>Not submitted</span>
					</td>
					<td class="">&nbsp;</td>
				</tr>
				<tr class="rego">
					<td class="editing"><span class="visuallyhidden">Not submitted-</span>AUSkey</td>
					<td class="status-waiting">Simon Arthur Bourke</td>
					<td class="">
						<span>Not submitted</span>
					</td>
					<td class="">&nbsp;</td>
				</tr>
			</tbody>
		</table>
	</div>
		<div class="dashboard-container" id="9619">
		<table>
			<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
				
				<div class="app-status"><p>Completed on 09 Apr 2017 16:18</p></div>
				<span class="controls" style="display: none;">
					<a href="javascript:void(0);" class="edit" style="display: none;">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
					<td class="status-waiting">John Cecil Smith</td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Submitted</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
					</td>
				</tr>
			</tbody>
		</table>
		<div class="referrer"></div>
	</div>
</div>
<div id="submit">
	<div class="dashboard-container" id="9513">
		<table>
			<caption>
				Australian Business Number (ABN): <strong>44 987 654 321</strong><br>
				
				<div class="app-status"><p>Completed on 12 Apr 2017 09:16</p></div>
				<span class="controls">
					<a href="register-existing5" class="edit">Reapply</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
			<tr>
				<th class="status-item">Registration item</th>
				<th class="status-detail">Detail</th>
				<th class="status-information" colspan="2">Status</th>
			</tr>
			</thead>
			<tbody>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="declined"><span class="visuallyhidden">Unsuccessful-</span>GST</td>
					<td class="status-waiting"></td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Unsuccessful</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your Goods and Services Tax (GST) registration has been unsuccessful:</p>
						<ul>
							 <li>Error with application for some reason.</li>
						</ul>
						<p>You can correct the errors and resubmit the application by using the <strong>Reapply</strong> button above.</p>
					</td>
				</tr>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="declined"><span class="visuallyhidden">Unsuccessful-</span>WET</td>
					<td class="status-waiting"></td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Unsuccessful</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your Wine Equalisation Tax (WET) registration has been unsuccessful:</p>
						<ul>
							 <li>Error with application for some reason.</li>
						</ul>
						<p>You can correct the errors and resubmit the application by using the <strong>Reapply</strong> button above.</p>
					</td>
				</tr>
				</tbody>
		</table>
		<div class="referrer"></div>
	</div>
	<div class="dashboard-container">
		<table>
			<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
				
				<div class="app-status"><p>Not submitted</p></div>
				<span class="controls">
					<a href="javascript:void(0);" class="edit">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				
				<tr>
					<td>&nbsp;</td>
					<td colspan="3">No registrations added.</td>
				</tr>
			</tbody>
		</table>
		<div class="referrer"></div>
	</div>
</div>
<div id="not-submitted">
	<div class="dashboard-container">
		<table>
			<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
				
				<div class="app-status"><p>Not submitted</p></div>
				<span class="controls">
					<a href="register-existing5" class="edit">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				
				<tr class="rego">
					<td class="editing"><span class="visuallyhidden">Not submitted-</span>GST</td>
					<td class="status-waiting"></td>
					<td class="">
						<span>Not submitted</span>
					</td>
					<td class="">&nbsp;</td>
				</tr>
				<tr class="rego">
					<td class="editing"><span class="visuallyhidden">Not submitted-</span>PAYG</td>
					<td class="status-waiting"></td>
					<td class="">
						<span>Not submitted</span>
					</td>
					<td class="">&nbsp;</td>
				</tr>
			</tbody>
		</table>
		<div class="referrer"></div>
	</div>
	<div class="dashboard-container" id="9619">
		<table>
			<caption>Australian Business Number (ABN): <strong>44 123 456 789</strong><br>
				
				<div class="app-status"><p>Completed on 09 Apr 2017 16:18</p></div>
				<span class="controls" style="display: none;">
					<a href="javascript:void(0);" class="edit" style="display: none;">Resume</a>
					&nbsp;
					<a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
					&nbsp;
					<a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
				</span>
			</caption>
			<thead>
				<tr>
					<th class="status-item">Registration item</th>
					<th class="status-detail">Detail</th>
					<th class="status-information" colspan="2">Status</th>
				</tr>
			</thead>
			<tbody>
				
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
					<td class="status-waiting">Fred Aurthur Nerk</td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Submitted</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
					</td>
				</tr>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
					<td class="status-waiting">John Cecil Smith</td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Submitted</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
					</td>
				</tr>
				<tr class="rego" onclick="$(this).next().toggle('fast')">
					<td class="registered"><span class="visuallyhidden">Submitted-</span>AUSKey</td>
					<td class="status-waiting">Bryan Anthony James</td>
					<td class="">
						<span>
							<a class="more" href="javascript:void(0)">Submitted</a>
						</span>
					</td>
					<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				</tr>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
					</td>
				</tr>
			</tbody>
		</table>
		<div class="referrer"></div>
	</div>
</div>
<div class="dashboard-container" id="9476">
    <table>
        <caption>
            Australian Business Number: <strong>44 555 555 555</strong><br>
            
            <div class="app-status"><p>Completed on 05 Apr 2017 16:06</p></div>
            <span class="controls" style="display: none;">
                <a href="javascript:void(0);" class="edit" style="display: none;">Resume</a>
                &nbsp;
                <a href="javascript:void(0);" class="remove" style="display: none;">Delete</a>
                &nbsp;
                <a href="javascript:void(0);" class="refresh" style="display: none;"><span class="fa fa-refresh"></span>Status update</a>
            </span>
        </caption>
        <thead>
        <tr>
            <th class="status-item">Registration item</th>
            <th class="status-detail">Detail</th>
            <th class="status-information" colspan="2">Status</th>
        </tr>
        </thead>
        <tbody>
			<tr class="rego" onclick="$(this).next().toggle('fast')">
				<td class="registered"><span class="visuallyhidden">Submitted-</span>GST</td>
				<td class="status-waiting"></td>
				<td class="">
					<span>
						<a class="more" href="javascript:void(0)">Submitted</a>
					</span>
				</td>
				<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
			</tr>
			<tr style="display: table-row;" class="extra" style="display: none">
				<td>&nbsp;</td>
				<td colspan="3">
					<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
				</td>
			</tr>
			<tr class="rego" onclick="$(this).next().toggle('fast')">
				<td class="registered"><span class="visuallyhidden">Submitted-</span>LCT</td>
				<td class="status-waiting"></td>
				<td class="">
					<span>
						<a class="more" href="javascript:void(0)">Submitted</a>
					</span>
				</td>
				<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
			</tr>
			<tr style="display: table-row;" class="extra" style="display: none">
				<td>&nbsp;</td>
				<td colspan="3">
					<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
				</td>
			</tr>
			<tr class="rego" onclick="$(this).next().toggle('fast')">
				<td class="registered"><span class="visuallyhidden">Submitted-</span>FTC</td>
				<td class="status-waiting"></td>
				<td class="">
					<span>
						<a class="more" href="javascript:void(0)">Submitted</a>
					</span>
				</td>
				<td class=""><span class="fa fa-plus-square">&nbsp;</span></td>
				<tr style="display: table-row;" class="extra" style="display: none">
					<td>&nbsp;</td>
					<td colspan="3">
						<p>Your registration has been submitted. Check with the ATO to see if it was successful.</p>
					</td>
				</tr>
			</tr>
		</tbody>
    </table>
    <div class="referrer"></div>
</div>
<div id="pager" class="card" style="">
        <div class="grid-row">
            <p>
                You have <span>4</span> more application(s)
                <button id="btnShowMore" type="button" class="btn btn-inline" style="margin-left: 10px">Show more...</button>
            </p>
        </div>
    </div>
</div>

<script type="text/javascript" src="/scripts/clipboard.min.js"></script>

<script type="text/javascript">
	$(document).ready(function() {
	
		var qryStr = getUrlVars();
		if (qryStr.type == "auskey") {
			$("#add-auskeys").show();
			$("#not-submitted").hide();
			$("#submit").hide();
			if (qryStr.action == "save") {
				$("#auskey-pending").hide();
				$("#new-auskeys").show();
			}
		}
		else if (qryStr.action == "submit") {
			$("#submit").show();
			$("#not-submitted").hide();
		} else if (qryStr.action == "resubmit") {
			$("#not-submitted").hide()
			$("#9513").hide()
			$("#resubmit").show()
		} else {
			$("#submit").hide();
			$("#not-submitted").show();
		}
	
		$("#show-adv").click(function () {
			$("#advanced-search").toggle('fast');
			if ($("#advanced-search:visible").length)
				$("#show-adv").html("Hide advanced options");
			else
				$("#show-adv").html("Show advanced options");
			$(this).blur();
		});
	
		
	
	});
		
	/* Drop down settings menu */
	$("nav").accessibleMegaMenu({
		/* prefix for generated unique id attributes, which are required to indicate aria-owns, aria-controls and aria-labelledby */
		uuidPrefix: "accessible-megamenu",
		/* css class used to define the megamenu styling */
		menuClass: "nav-menu",
		/* css class for a top-level navigation item in the megamenu */
		topNavItemClass: "nav-item",
		/* css class for a megamenu panel */
		panelClass: "sub-nav",
		/* css class for a group of items within a megamenu panel */
		panelGroupClass: "sub-nav-group",
		/* css class for the hover state */
		hoverClass: "hover",
		/* css class for the focus state */
		focusClass: "focus",
		/* css class for the open state */
		openClass: "open"
	});
</script>

</main>
