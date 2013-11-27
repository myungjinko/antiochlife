require 'resque_scheduler/tasks'

web:    bundle exec thin start -p $PORT
worker: bundle exec rake resque:work QUEUE=*
clock:  bundle exec rake resque:scheduler