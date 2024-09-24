<h2>Automated RPA Challenge Workflow</h2>
<p>
    Developed an RPA workflow to automate the RPA Challenge, focusing on accurately inputting data from an Excel file into dynamic form fields on a website that change positions after each submission. Integrated error handling to ensure accurate data entry across 10 rounds using UiPath.
</p>

<h3>Workflow Overview</h3>
<ul>
    <li>
        <strong>RPA_Challenge_Launch:</strong> Open RPA Challenge Web.<br>
        <em>PreCondition:</em> N/A.<br>
        <em>PostCondition:</em> RPA Challenge Exists.
    </li>
    <li>
        <strong>RPA_Challenge_DownloadFile:</strong> Downloading Excel File.<br>
        <em>PreCondition:</em> RPA Challenge Exists.<br>
        <em>PostCondition:</em> RPA Download Popup Exists.
    </li>
    <li>
        <strong>RPA_Challenge_SaveFile:</strong> Saving Excel File.<br>
        <em>PreCondition:</em> RPA Download Popup Exists.<br>
        <em>PostCondition:</em> File Exists in the Path.
    </li>
    <li>
        <strong>RPA_Challenge_ReadFile:</strong> Read Downloaded Excel File.<br>
        <em>PreCondition:</em> File Exists in the Path.<br>
        <em>PostCondition:</em> Data Read Successfully.
    </li>
    <li>
        <strong>RPA_Challenge_WriteFields:</strong> Write RPA Challenge Fields.<br>
        <em>PreCondition:</em> Data Read Successfully and RPA Challenge Exists.<br>
        <em>PostCondition:</em> Congratulations Exists.
    </li>
    <li>
        <strong>RPA_Challenge_Close_Web:</strong> Close Web.<br>
        <em>PreCondition:</em> Congratulations Exists.<br>
        <em>PostCondition:</em> RPA Challenge is Completed.
    </li>
</ul>
