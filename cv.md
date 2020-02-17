## Curriculum Vitae

1. Evgeniy Y
2. Email: yues.it@yandex.ru
3. My goal is to become a guru Frontend Developer
4. My key skills: 
    * C# .NET Framework;
    * MS SQL;
    * ASP.NET;
    * MS SharePoint;
    * basic JavaScript;
    * basic Vue.js;
    * basic jQuery;
    * Bootstrap, CSS, HTML;
    * SVN, TFS;
    * Jira.
5. VueJs:
```
var dataComponent = {
	employeeBirthday: []
};

var emplBirthdayComponent = Vue.component('employee-birthday-component', {
	data: function () {
		return dataComponent;
	},
	created: function () {
        this.getEmployeeBirthday();
	},
	methods: {
		getEmployeeBirthday: function () {
			try {
				$.ajax({
					type: "GET",
                    url: "/TestTaskPages/EmployeesBirthday.aspx/GetEmployeeWithNearBirthday",
					contentType: "application/json; charset=utf-8",
                    success: function (data) {

                        if (data.d && data.d.length > 0) {
							dataComponent.employeeBirthday = data.d;
						}
					},
					error: function (XMLHttpRequest, textStatus, errorThrown) {
						console.log("Request Error:" + textStatus + errorThrown);
					}
				});
			} catch (ex) {
				console.log("Error:" + ex);
			}
		}
	}
});


var app = new Vue({
    el: '#employeeBirthdayApp',
	data: {
	}
});
```

6. August 2018 — currently, Web-developer.
Development, support and installation of solutions for the internal corporate portal on the MS SharePoint 2016 platform using 	.NET C #, ASP.NET, SQL, JS, VueJS, PowerShell;
7. Novosibirsk State Technical University, Faculty of Business, Applied Informatics.
8. English (courses at work, 1 year, elementary level).
