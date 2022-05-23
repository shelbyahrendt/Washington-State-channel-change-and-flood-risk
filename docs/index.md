# What is "channel-driven" flooding?
Flood hazards in most basins are typically assumed to be driven by the frequency and intensity of high discharge events, but changes in a river’s conveyance capacity can also contribute substantially to flood hazards. Take the channel shown in the figure below where Q-bankfull is the bankfull flow capacity of the channel. This river section can flood by two mechanisms. 1: it can experience a discharge event 'Q' that exceeds Q-bankfull, or 2: sediment can deposit in the channel changing the channel's conveyance capacity and causing water to flow overbank for what was previously a Q-bankfull event. It's these changes in channel conveyance capacity that we are trying to understand in order to improve flood risk predictions.

<img src="https://i.imgur.com/FN0xYpt.png" alt="flood mechanisms"/>

*Fig 1: Flood hazards driven by 1) discharge and 2) channel conveyance changes over time*

# Analyzing Channel Conveyance Change

Here we analyze historic channel conveyance changes for 50 United States Geological Survey (USGS) gauging stations across western Washington state. Channel conveyance changes are reported in units of flow and represent an estimate in the change in streamflow the channel is able to convey at bankfull capacity. The figure below shows dots at each gauging location that are sized by the relative magnitude of channel conveyance change. These datapoints are normalized by the Q-bankfull for each channel in order to compare fractional changes in channel conveyance between rivers of different sizes.

Hovering your mouse over a given datapoint, you can see the time series of channel conveyance change used to compute the dotsize representing magnitude of change. Changes are with respect to the bankfull conveyance capacity in 2015. Sites with linear changes in channel conveyance are fit with a linear trend and sites that show non-linear or "unsteady" changes to channel conveyance are fit with a 10-point moving median. Tendencies towards positive conveyance values indicate that the channel is increasing it's ability to convey flow, and tendencies towards negative conveynace values indicate that less water will be able to flow through the channel over time.

<iframe src="channel_change_map.html"
    sandbox="allow-same-origin allow-scripts"
    width="800"
    height="800"
    scrolling="yes"
    seamless="seamless"
    frameborder="0">
</iframe>

*Fig 2: Map of channel conveyance change through time at Western Washington study gages. Dots are sized by relative magnitude of changes*

<iframe src="streamflow_change_map.html"
    sandbox="allow-same-origin allow-scripts"
    width="800"
    height="800"
    scrolling="yes"
    seamless="seamless"
    frameborder="0">
</iframe>

*Fig 3: Map of streamflow change through time at Western Washington study gages. Dots are sized by relative magnitude of changes*

# References

This website accompanies the submitted manuscript: S. Ahrendt, A. Horner-Devine, B. Collins, J. Morgan,  E. Istanbulluoglu, *Channel conveyance variability can influence flood risk as much as streamflow variability in western Washington State*

Raw data is obtained from the USGS National Weather Information Service online server: https://waterdata.usgs.gov/nwis

Processed data to create the plots shown in Fig 2 and Fig 3 is available in this website's base respository: https://github.com/shelbyahrendt/Washington-State-channel-change-and-flood-risk/tree/main/study_data

Interactive plot graphics were developed with the support of the Risk \& Resilience DAT/Artathon: https://datartathon.com
