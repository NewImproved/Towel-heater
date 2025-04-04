# Towel-heater

Core Functionality
This configuration creates a comprehensive control system for a towel heater (called "Handdukstork" in Swedish) with multiple scheduling options and safety features.
Control Methods

Manual Control

Direct on/off toggle switch
Safety timer that automatically turns off the heater after 4 hours


Scheduled Operation

One-time schedule: Run the heater once at a specific time
Workday schedule: Automatically run the heater on workdays at a set time



Configuration Components

Timer: A 4-hour safety timer that turns off the heater automatically
Input Fields:

Time selectors for one-time and workday schedules
Adjustable run time setting (3-5 hours)
Toggle switches for manual control and schedule activation



Smart Features

Calculated Start Times: The system automatically calculates when to start the heater (1 hour before the set time)
Status Indicators:

Current heater status
Time until next scheduled use
Calculated start and stop times



Safety and Recovery Features

Automatic shutoff when the timer expires
Timer restart when Home Assistant restarts if the heater is already on
Automatic disabling of one-time schedule after completion

Automations
The system includes multiple automations to handle:

Turning the heater on/off based on manual control
Starting/stopping based on schedules
Synchronizing UI state with actual heater state
Safety timer management
Recovery after system restart

The physical device appears to be a Shelly 1PM smart switch (entity ID: switch.shelly1pm_34945476550b) that controls power to the towel heater.
