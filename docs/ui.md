# Portfolio & Dashboards

<br>

## Motivations

The revamped portfolio and dashboard pages were based on UX feedback, regarding certain pain points in the old versions. This included:
<ul>
    <li>Difficulty determining relationships with previous period and/or target values.</li>
    <li>Too text heavy.</li>
    <li>Simultaneous saying too much and not enough</li>
</ul>

<br>

## Implementation Changes

<p>Dashboards are now segmented better. At the top is a key fact bar with the basic details of a fund or asset. We then have a utility section with 1 tile for each utility:
<ul>
    <li>Carbon Emissions</li>
    <li>Energy Intensity</li>
    <li>Electricity</li>
    <li>Gas, Fuels & Thermals</li>
    <li>Water</li>
    <li>Waste recycling</li>
</ul>
</p>
<p>
All these contain a bar showing the current period compared to the same previous the previous year. The charts are seperated into recycling vs non-recycling for the waste recycling, and otherwise are actual vs gapfill data. Below these we have larger tiles for:
<ul>
    <li>Data Quality</li>
    <li>EPC Analysis (fund only)</li>
    <li>NZC (fund only)</li>
    <li>Action Plans</li>
</ul>
</p>

<br>
<p>
For the <b>Portfolio</b> page we made a scrollable table. We show 10 assets at a time, and display their consumption details for each ultity, the DQ figures for the asset, their action plans count by status as well as the fund, energy rating score and any labels needed (ie sold asset tag). The user can filter assets in this screen by their location, energy rating, property sector and fund, so they can only view the assets they wish to. The user is also able to sort the utility values so they can easily see their best and/or worst performing assets
</p>
