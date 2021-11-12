---
title: 'Добавление пользовательских данных в группы с помощью расширений схемы '
description: 'В этой статье рассматривается пример использования *расширений схемы*. '
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 8e024e625258dca2eda46dd0b9cdde6bbefb6cbc
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60934795"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a>Добавление пользовательских данных в группы с помощью расширений схемы 

В этой статье рассматривается пример использования *расширений схемы*. 

Представьте, что вы — разработчик в компании Graph Learn, создающей программное обеспечение для управления обучением, а именно учебные курсы и материалы для предприятий.  Благодаря богатым возможностям совместной работы, группы Microsoft 365 отлично подходят для записи упражнений и предоставления содержимого участникам онлайн- и аудиторных курсов.  Вы можете обозначить группы Microsoft 365, используемые для учебных курсов, соответствующим образом, чтобы другие разработчики могли находить ваши группы и дополнять функциональными возможностями ваши учебные курсы.

Для этого сценария в этой статье показано, как:

1. просмотреть доступные определения расширений схемы;
2. зарегистрировать определение расширения схемы, ориентированное на группы для учебных курсов;
3. создать группу с расширенными данными на основе зарегистрированного определения расширения схемы;
4. добавить, обновить или удалить пользовательские данные в существующей группе с помощью определения расширения схемы;
5. считать данные групп и расширений.

>**Примечание.** В этой статье показано, как создавать и считывать значения расширений схемы для ресурса **group** (шаги 3–5).  Такие же методы поддерживаются для типов ресурсов **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** и **user**.  Вы можете выполнять операции, представленные примерами запросов в этой статье, для любого из этих ресурсов. Обратите внимание, что тип ресурса **administrativeUnit** доступен только в конечной точке бета-версии.

## <a name="1-view-available-schema-extensions"></a>1. Просмотр доступных расширений схемы
Во-первых, разработчику может понадобиться найти другие определения расширений схемы, которые может повторно использовать приложение.  В этом случае нужно выполнить запрос для ресурса **schemaExtension**.  
В приведенном ниже примере показан запрос на получение определенного расширения схемы с учетом **id**.

Обратите внимание, что параметру **status** для возвращенного в ответе расширения задано значение **Available**. Это означает, что любое приложение, у которого есть разрешение на доступ к ресурсам в свойстве **targetTypes**, может использовать и обновлять расширение с дополнительными изменениями. Как правило, эта операция возвращает любые расширения схемы, соответствующие указанному фильтру, независимо от значения **status**. Поэтому нужно проверить состояние расширения, прежде чем его использовать.


### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-get"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```

### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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

При создании определения расширения схемы нужно предоставить строку для свойства **id**. Это можно сделать двумя способами. В следующем примере показан предпочтительный способ с использованием запоминающегося доменного имени (`graphlearn.com`), проверенного в клиенте. Объедините проверенное доменное имя (`graphlearn`) с именем для расширения схемы (`courses`) и назначьте **id** с использованием полученной строки, `graphlearn_courses`.  

Затем укажите описание (необходимо для поиска), целевые типы (ресурсы, к которым применимо это расширение) и настраиваемые свойства, из которых состоит схема.  В этом примере укажите настраиваемые свойства `courseId`, `courseName` и `courseType`, а также их типы.

См. [пример другого способа назначения **id** в запросе](/graph/api/schemaextension-post-schemaextensions#request-2), где требуется указать только имя схемы.

Обратите внимание, что при первоначальном создании расширение схемы имеет состояние **InDevelopment**. Во время разработки расширения такое состояние можно сохранять. Пока оно не изменится, только ваше приложение, создавшее расширение, сможет его обновлять, внося дополнительные изменения, или удалять. Когда вы будете готовы предоставить доступ к расширению другим приложениям, установите для параметра **status** значение **Available**.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createExtension"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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

### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
{
    "id": "graphlearn_courses",
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
Создайте _новую_ группу и расширьте ее, добавив дополнительные данные с помощью зарегистрированного определения расширения схемы `graphlearn_courses`.  Это стандартный запрос ```POST``` для ресурса **group** с дополнительным расширением сложного типа `graphlearn_courses`, определенным в теле запроса.  В ответе не будут отражены никакие расширения данных. Необходимо с помощью параметра ```$select``` указать имя расширения в операции ```GET```.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createGroupWithExtension"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
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
### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
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

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a>4. Добавление, обновление и удаление пользовательских данных существующей группы
Вы можете расширить существующий экземпляр _group_ и добавить в него пользовательские данные с помощью дополнительного расширения сложного типа `graphlearn_courses`, определенного в теле запроса ```PATCH```.  

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-updateGroupWithExtension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```

### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

Если вы хотите обновить значения данных расширения, поместите весь сложный тип расширения в тексте запроса ```PATCH``` (так же, как и при добавлении пользовательских данных к существующему ресурсу).

Вы также можете удалить пользовательские данные, добавленные в экземпляр ресурса, задав для соответствующего свойства расширения значение null. 

Чтобы удалить расширение схемы из экземпляра ресурса, задайте для сложного типа расширения значение null.


## <a name="5-get-a-group-and-its-extension-data"></a>5. Получение экземпляра group и его данных расширения
Удобный способ найти группу (или группы) — применить `$filter` с указанием определенных значений свойства расширения, например идентификатора или имени расширения. 

Затем, чтобы получить пользовательские данные группы, примените `$select`, чтобы включить расширение с указанием имени (в данном случае `graphlearn_courses`).

Приведенный ниже пример запроса ищет группу с расширением `graphlearn_courses`, для которой значение свойства `courseId` соответствует `123`, и получает свойства группы **displayName**, **id** и **description**, а также пользовательские данные расширения `graphlearn_courses`. (Выполняя реальный запрос, по необходимости применяйте URL-кодировку.)

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-getGroupSelectExtension"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](extensibility-overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](extensibility-open-users.md).
- [Домены Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/domains)
- [Добавление и проверка домена для Microsoft 365](/microsoft-365/admin/setup/add-domain)
- [Тип ресурса schemaExtension](/graph/api/resources/schemaextension)