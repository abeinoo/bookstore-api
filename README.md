# README

Things you may want to cover:

* Ruby version
 - ruby 2.3.1p112
* Rails version
 - Rails 5.0.3 
* System dependencies
 - ember-cli: 2.13.2
 - node: 7.10.0

* Configuration
 -  use active_model_serializers gem
  - create on config/initializers/json_api.rb
  - ActiveModelSerializers.config.adapter = :json
  - Configuration to return json to ember

 - We need to create what is called an adapter
  - for more information about adapter
   - https://emberigniter.com/fit-any-backend-into-ember-custom-adapters-serializers/
  - we will override a function called pathForType that will underscore (and pluralize) on               "app/adapters/application.js"
  
 - Let’s boot Ember CLI server. We are going to use the --proxy flag to let it know our backend is listening at port 
  - "ember server --proxy http://localhost:3000"
  - OR set "proxy": "http://localhost:3000" on  "ember-cli"
 
 - User ember inspector
  - https://guides.emberjs.com/v2.5.0/ember-inspector/installation/

 - To get start with ember
  - https://emberigniter.com/getting-started-ember-cli-data-down-actions-up-tutorial/
  - https://guides.emberjs.com/v2.5.0/getting-started/quick-start/