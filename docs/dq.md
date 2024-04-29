# Data Quality



<br>

## Motivations

'Old' Data Quality has a few issues which needed changing.
<p>
Firstly the code structure has an element of 'whackamole', where changing one thing often has many unintended consequences. 'DQ bugs are like the hydra, fix one and 2 more appear' - Rory, March/April 2024.
<br>
Secondly the metric was a combination of 2 calculations, one for an area based figure, and the other for a time based figure, meaning the percentages made little sense.
</p>
Bugs reported with data quality included - negative percentages, percentages greater than 100%, percentages not summing to 100% and data inconsistencies between pages which showed DQ

<br>

## Change Summary

A complete delta of the methodology can be found on <a href="https://evorasiera.atlassian.net/wiki/spaces/SPEC/pages/2591457296/Delta+-+Data+Coverage+Methodology">Confluence.</a>
<br>
Short summary is:
<ul>
    <li>DQ will now be 2 metrics, <b>Coverage</b> (area based calc) and <strong>Completeness</strong> (time based calc)</li>
    <li>Maximum area has been reworked to ensure <em>unique</em> meter setups are divided by the correct figure</li>
    <li>Will be calculated by a series of sums (no averaging), as an asset is a group of meters, and a fund is a sum of assets</li>
</ul>

<br>

## Coverage

This is <b>area-based</b>. Thus the coverage figure for a utility will be the sum of all meters for that utility (with reporting data in the period) divided by the larger of:
<ul>
    <li>The asset GIA/NLA</li>
    <li>The sum of the meters for that utility<li>
</ul>
For assigning this to landlord or tenant the same holds true but the divisors are dependant on the expected area the meters cover. We usually expect the landlord to cover any missing are, unless we explicity can see the asset has a gap in a tenant space or .

<br>

## Completeness

<p>This is <b>time based</b>. Simply put this is a sum of days covered by the data entered into a consumption record. We have 4 categories for these to fall into:
<ul>
    <li>Actual - where we know this is an accurate consumption record - eg meter reading</li>
    <li>Supplier estimate - where we see a supplier has estimated the value</li>
    <li>Calculated estimate - where we see the record has been estimated by some form of calculation</li>
    <li>Missing - where there is no consumption record or no obvious source of the consumption data</li>
</ul>
This is divided by the number of expected days in the chosen time period, ie for a year it would be 365/366, for 3 months it could be 91 etcetera.<br>
For a single utility this could be just one meter or a sum of multiple. This sum is then used per utility for an asset and fund.
</p>