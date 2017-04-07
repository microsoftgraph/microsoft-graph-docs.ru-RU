# <a name="add-custom-data-to-groups-using-schema-extensions-preview"></a>Добавление пользовательских данных в группы с помощью расширений схемы (предварительная версия)

В этой статье мы подробно рассмотрим пример использования *расширений схемы*. 

Представьте, что вы разработчик в компании Graph Learn, разрабатывающей программное обеспечение для управления обучением, а именно учебные курсы и материалы для предприятий.  Благодаря богатым возможностям совместной работы, группы Office 365 отлично подходят для предоставления участникам содержимого курсов и записи упражнений как в онлайн-курсах, так и под руководством преподавателя.  Вы можете обозначить группы Office 365, используемые для учебных курсов, соответствующим образом, чтобы другие разработчики могли находить ваши группы и создавать многофункциональные системы на основе ваших учебных курсов.

В этой статье мы покажем вам, как:

1. просмотреть доступные определения расширений схемы;
2. зарегистрировать определение расширения схемы, предназначенное для групп учебных курсов;
3. создать группу с расширенными данными на основе зарегистрированного определения расширения схемы;
4. добавить и обновить пользовательские данные для существующей группы на основе определения расширения схемы;
5. считать данные групп и расширений.

>**Примечание.** В этой статье показано, как создавать и считывать значения расширений схемы для ресурса **group** (шаги 3–5).  Такие же методы поддерживаются для типов ресурсов **device**, **event**, **message**, **post** и **user**.  Поэтому можно выполнять такие же операции, как представленные приведенными ниже запросами, для любого из этих ресурсов.

## <a name="1-view-available-schema-extensions"></a>1. Просмотр доступных расширений схемы
Во-первых, разработчику может понадобиться найти другие определения расширений схемы, которые может повторно использовать приложение.  В этом случае нужно выполнить запрос для ресурса **schemaExtension**.  
В приведенном ниже примере показан запрос на получение определенного расширения схемы с учетом **id**.

Обратите внимание, что параметру **status** для возвращенного в отклике расширения задано значение **Available**. Это означает, что любое приложение, у которого есть разрешение на доступ к ресурсам в свойстве **targetTypes**, может использовать и обновлять расширение с дополнительными изменениями. Как правило, эта операция возвращает любые расширения схемы, соответствующие указанному фильтру, независимо от значения **status**. Поэтому нужно проверить состояние расширения, прежде чем его использовать.


##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/schemaExtensions/$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a>Ответ
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a>2. Регистрация определения расширения схемы, описывающего учебный курс
Если вам не удастся найти расширение схемы, *соответствующее* вашим потребностям, вы можете создать и зарегистрировать новое определение расширения для учебных курсов в ресурсе **group**.  

При создании определения расширения схемы нужно предоставить строку для свойства **id**. Это можно сделать двумя способами. В следующем примере показан предпочтительный способ с использованием запоминающегося доменного имени (`graphlearn.com`), проверенного в клиенте. Объедините проверенное доменное имя (`graphlearn`) с именем для расширения схемы (`courses`) и назначьте **id** с использованием полученной строки, `graphlearn_courses`.  Укажите также описание (обеспечивающее удобство поиска), целевые типы (ресурсы, к которым применимо это расширение) и настраиваемые свойства, из которых состоит схема.  В этом примере укажите настраиваемые свойства `courseId`, `courseName` и `courseType`, а также их типы.

См. [пример другого способа назначения **id** в запросе](../api-reference/beta/api/schemaextension_post_schemaextensions.md#request-2), где требуется указать только имя схемы.

Обратите внимание, что при первоначальном создании расширение схемы имеет состояние **InDevelopment**. Во время разработки расширения такое состояние можно сохранять. Пока оно не изменится, только ваше приложение, создавшее расширение, сможет его обновлять, внося дополнительные изменения, или удалять. Когда вы будете готовы предоставить доступ к расширению другим приложениям, установите для параметра **status** значение **Available**.

##### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json
{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
##### <a name="response"></a>Ответ
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_course",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="3-create-a-new-group-with-extended-data"></a>3. Создание новой группы с расширенными данными 
Создайте новую группу, содержащую дополнительные данные, с помощью зарегистрированного определения расширения схемы `graphlearn_courses`.  Это стандартный запрос ```POST``` для ресурса **group** с дополнительным расширением сложного типа `graphlearn_courses`, определенным в теле запроса.  В отклике не будут отражены никакие расширения данных. Необходимо с помощью параметра ```$select``` указать имя расширения в операции ```GET```.

##### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a>Ответ
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-or-update-custom-data-to-an-existing-group"></a>4. Добавление или изменение пользовательских данных в существующей группе
Как и в предыдущем примере, мы можем расширить существующий ресурс group с помощью дополнительного расширения сложного типа `graphlearn_courses`, определенного в теле запроса ```PATCH```.  

##### <a name="request"></a>Запрос
```http
PATCH https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a>Ответ
```http
HTTP/1.1 204 No Content
```

Если вы хотите обновить значения данных расширения, поместите весь сложный тип расширения в тексте запроса ```PATCH``` (так же, как и при добавлении пользовательских данных к существующему ресурсу).

## <a name="5-get-a-group-and-its-extension-data"></a>5. Получение экземпляра group и его данных расширения
Чтобы получить экземпляр group **и** его данные расширения, необходимо использовать `$select` для указания имени расширения, в данном случае `graphlearn_courses`.

#### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355?$select=displayName,id,description,graphlearn_courses
```

##### <a name="response"></a>Отклик
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](extensibility_open_users.md)
- [Домены Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [Добавление и проверка домена для НОВОГО плана Office 365](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [Тип ресурса schemaExtension](../api-reference/beta/resources/schemaextension.md)
- [Перечисление schemaExtensions](../api-reference/beta/api/schemaextension_list.md)
- [Создание schemaExtension](../api-reference/beta/api/schemaextension_post_schemaextensions.md)
- [Получение schemaExtension](../api-reference/beta/api/schemaextension_get.md)
- [Обновление schemaExtension](../api-reference/beta/api/schemaextension_update.md)
- [Удаление schemaExtension](../api-reference/beta/api/schemaextension_delete.md)
