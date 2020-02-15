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

6. Experience (for a Junior Dev it means all kinds of experience: coding tests, projects from courses,
freelance projects - wherever they had the opportunity to demonstrate skills they have.
Also it would be awesome if you add links to source code)
7. Education (including courses, seminars, lectures, online learning)
8. English (elaborate on what kind of practice you had, if any, how long it lasted and so on)
