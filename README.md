# ESPDailyTaskNTP
Schedule one task every day twice at the same time. Deepsleep in-between

Daily task with 12 hr instead of 24 hr

a;sp replace line 61 of SNTPtime library
  _tempDateTime.hour = _time % 24;
to
  _tempDateTime.hour = _time % 12;
