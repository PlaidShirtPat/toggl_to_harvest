# Convert Toggl Time Entries to Harvest

This is a very simple import tool for converting Toggl http://toggl.com time
entry CSV exports to a format that you can import into Harvest
http://www.getharvest.com/

Toggl should dump record that look similar to:

    0-User,1-Client,2-Project,3-Description,4-Billable,5-Start time,6-End time,7-Duration,8-Tags,9-Task,10-Amount (USD)
    Rain48,CatalogChoice,catalogchoice.org,braintree,Yes,06/21/2011 14:43,06/21/2011 17:28,02:45:20,"","",220.44

To use this simply:

    git clone git://github.com/wiseleyb/toggl_to_harvest.git
    cd toggl_to_harvest
    ruby convert.rb _toggl-csv-file_

It will spit out a harvest compatible file with _harvest.csv.  Example:

    ruby convert.rb toggltime.csv
    >> toggltime_harvest.csv

If you have any questions:  wiseleyb@gmail.com
