# most-data-mysql (in progress - separate adapter from most-data core)
Most Web Framework MySQL Adapter
##Install
$ npm install most-data-mysql
##Usage
Register Oracle adapter on app.json as follows:

    "adapterTypes": [
        ...
        { "name":"MySQL Data Adapter", "invariantName": "mysql", "type":"most-data-mysql" }
        ...
    ],
    adapters: [
        ...
        { "name":"development", "invariantName":"mysql", "default":true,
            "options": {
              "host":"localhost",
              "port":1521,
              "user":"user",
              "password":"password"
            }
        }
        ...
    ]

If you are intended to use MySQL data adapter as the default database adapter set the property "default" to true.
