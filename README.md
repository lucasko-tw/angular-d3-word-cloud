D3 Angular Word Cloud
===============================================================
### Word Cloud
![Word Cloud](https://github.com/lucasko-tw/angular-d3-word-cloud/blob/master/word-cloud.png)

### Include Package/Resource
```HTML
 <script src="bower_components/angular/angular.js"></script>
 <script src="bower_components/d3/d3.min.js"></script>
 <script src="bower_components/d3-cloud/build/d3.layout.cloud.js"></script>
 <script src="d3_word_cloud.js"></script>
```

### Define Words
```HTML
<script>
    angular.module('myApp', ['wc'])
            .controller('myCtrl', function ($scope) {
                $scope.name = 'Top Weak Password:';
                $scope.tags = [
                    {"key": "123456", "value": 30},
                    {"key": "password", "value": 29},
                    {"key": "qwerty", "value": 27},
                    {"key": "football", "value": 25},
                    {"key": "1234", "value": 23},
                    {"key": "welcome", "value": 21},
                    {"key": "abc123", "value": 19},
                    {"key": "1qaz2wsx", "value": 17},
                    {"key": "master", "value": 15},
                    {"key": "login", "value": 13},
                    {"key": "monkey", "value": 13},
                    {"key": "letmein", "value": 12},
                    {"key": "starwars", "value": 11},
                    {"key": "mustang", "value": 10},
                    {"key": "always", "value": 14},
                    {"key": "access", "value": 13},
                    {"key": "shadow", "value": 13},
                    {"key": "michael", "value": 12},
                    {"key": "batman", "value": 11},
                    {"key": "trustno1", "value": 10}
                ];
            });
</script>

```

and, set div for word cloud.

```HTML
<div ng-app="myApp" ng-controller="myCtrl">
    <p>Name: {{name}}</p>
    <word-cloud tags="tags"></word-cloud>
</div>
```

More Details for Preparing.
-------------------------------------
### Install npm

Download and install node-v6.9.1.pkg 

### Install bower

	sudo npm install -g bower

### Install d3 package

	bower install d3-cloud-ng

After install, you will find folder under home that is called 'bower_components'


