Configuring cron jobs in cPanel
===================================
cPanel controls domains and has an option to configure cron jobs. Here is everything you need to configure cron jobs in cPanel.
cPanel formats pages based on styles. This document is based on the sundaymorning style. The location of options might vary if you use a different style. You can change the style using the Change Style option in cPanel. In the sundaymorning and Crimson smoke themes, you select Advanced then Cron jobs.
 
WHM, Web Host Manager, is the cPanel product for controlling domains in a Virtual Private Server. If there is no cron option in your cPanel, you may have to add cron in WHM. Cron may be in different places in the various Cpanel themes.
You may be offered the option of standard or an advanced Unix style user interface. You may see an error message similar to the following.
/usr/bin/crontab permissions are wrong. Please set to 4755
The Unix style interface dumps you in a page where you can enter a command the same as described on the main Configuring cron jobs page.
The standard page lets you select the number of minutes, hours, days, or months from selection lists and add the final part of the command.
The following image shows the add new cron job section of the cron page including the drip down selection boxes and the final text box for your command. Some of the boxes are explained next.
 
The Common Settings drop down lets you select every hour, every day, and other useful options. Select Once a day (0 0 * * *) as an example. That sets the minute and hour options to zero indicating midnight. The same selection sets day, month, and weekday to * to indicate every day of every month on every day of the week.
You can then change the minute or hour to a less busy time. For example, some Australian sites are busy at midnight handling requests from America where it is the start of the business day.
An easy way to start the Drupal cron job is to execute the file in some way. Lynx is a text based Web browser that accepts a URL as a parameter. You can start Lynx from cron and specify the Drupal cron job in the source parameter.
