---
title: 'Добавление пользовательских данных в группы с помощью расширений схемы '
description: 'В этой статье мы рассмотрим подробный пример использования *расширений схемы*. '
author: dkershaw10
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 28ef904429f90d0e1c1182887946c967739566bc
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053783"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a><span data-ttu-id="e41b0-103">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="e41b0-103">Add custom data to groups using schema extensions</span></span> 

<span data-ttu-id="e41b0-104">В этой статье мы рассмотрим подробный пример использования *расширений схемы*.</span><span class="sxs-lookup"><span data-stu-id="e41b0-104">We're going to walk you through an example to demonstrate how to use *schema extensions*.</span></span> 

<span data-ttu-id="e41b0-p101">Представьте, что вы — разработчик в компании Graph Learn, создающей программное обеспечение для управления обучением, а именно учебные курсы и материалы для предприятий.  Благодаря богатым возможностям совместной работы, группы Office 365 отлично подходят для записи упражнений и предоставления содержимого участникам онлайн- и аудиторных курсов.  Вы можете обозначить группы Office 365, используемые для учебных курсов, соответствующим образом, чтобы другие разработчики могли находить ваши группы и дополнять функциональными возможностями ваши учебные курсы.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p101">Imagine you're a developer in a Learning Management Software company called “Graph Learn” that builds training courses and materials for businesses.  Office 365 groups, with their rich collaborative experiences, is a fantastic way to deliver course content and record exercises among participants for both online courses and instructor-led courses.  You may want to make those Office 365 groups used for training courses easily identifiable as training courses, which will allow other developers to discover your groups and build rich experiences on top of your learning courses.</span></span>

<span data-ttu-id="e41b0-108">В этой статье мы покажем, как можно сделать следующее:</span><span class="sxs-lookup"><span data-stu-id="e41b0-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="e41b0-109">просмотреть доступные определения расширений схемы;</span><span class="sxs-lookup"><span data-stu-id="e41b0-109">View available schema extension definitions that you could use.</span></span>
2. <span data-ttu-id="e41b0-110">зарегистрировать определение расширения схемы, ориентированное на группы для учебных курсов;</span><span class="sxs-lookup"><span data-stu-id="e41b0-110">Register a schema extension definition that targets groups for training courses.</span></span>
3. <span data-ttu-id="e41b0-111">создать группу с расширенными данными на основе зарегистрированного определения расширения схемы;</span><span class="sxs-lookup"><span data-stu-id="e41b0-111">Create a new group with extended data based on the schema extension definition that you just registered.</span></span>
4. <span data-ttu-id="e41b0-112">добавить, обновить или удалить пользовательские данные в существующей группе с помощью определения расширения схемы;</span><span class="sxs-lookup"><span data-stu-id="e41b0-112">Add, update, or remove custom data in an existing group based on a schema extension definition.</span></span>
5. <span data-ttu-id="e41b0-113">считать данные групп и расширений.</span><span class="sxs-lookup"><span data-stu-id="e41b0-113">Read back a group and the extension data.</span></span>

><span data-ttu-id="e41b0-p102">**Примечание.** В этой статье показано, как создавать и считывать значения расширений схемы для ресурса **group** (шаги 3–5).  Такие же методы поддерживаются для типов ресурсов **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** и **user**.  Поэтому можно выполнять такие же операции, как представленные приведенными ниже запросами, для любого из этих ресурсов. Обратите внимание, что тип ресурса **administrativeUnit** доступен только в конечной точке бета-версии.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p102">**Note:** This topic shows you how to create and read schema extension values on a **group** resource (steps 3-5).  The same methods are supported for the **administrativeUnit**, **device**, **event**, **message**, **organization**, **post**, and **user** resource types as well.  So you can carry out similar operations as the example requests below on any of those resources. Note that **administrativeUnit** is available only in the beta endpoint.</span></span>

## <a name="1-view-available-schema-extensions"></a><span data-ttu-id="e41b0-118">1. Просмотр доступных расширений схемы</span><span class="sxs-lookup"><span data-stu-id="e41b0-118">1. View available schema extensions</span></span>
<span data-ttu-id="e41b0-p103">Во-первых, разработчику может понадобиться найти другие определения расширений схемы, которые может повторно использовать приложение.  В этом случае нужно выполнить запрос для ресурса **schemaExtension**.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p103">First, as a developer, you might want to find any other schema extension definitions that our app could reuse.  This can be done by querying the **schemaExtension** resource.</span></span>  
<span data-ttu-id="e41b0-121">В приведенном ниже примере показан запрос на получение определенного расширения схемы с учетом **id**.</span><span class="sxs-lookup"><span data-stu-id="e41b0-121">In the example below, you're going to query for a specific schema extension by **id**.</span></span>

<span data-ttu-id="e41b0-p104">Обратите внимание, что параметру **status** для возвращенного в ответе расширения задано значение **Available**. Это означает, что любое приложение, у которого есть разрешение на доступ к ресурсам в свойстве **targetTypes**, может использовать и обновлять расширение с дополнительными изменениями. Как правило, эта операция возвращает любые расширения схемы, соответствующие указанному фильтру, независимо от значения **status**. Поэтому нужно проверить состояние расширения, прежде чем его использовать.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p104">Notice that the extension returned in the response has **Available** as the **status** value, which indicates that any app which has permission to the resources in the **targetTypes** property can use and update the extension with additive changes. In general, this operation returns any schema extensions that satisfy the specified filter regardless of **status**, so do check the extension status before using it.</span></span>


##### <a name="request"></a><span data-ttu-id="e41b0-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="e41b0-124">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="e41b0-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e41b0-125">Response</span></span>
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
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a><span data-ttu-id="e41b0-126">2. Регистрация определения расширения схемы, описывающего учебный курс</span><span class="sxs-lookup"><span data-stu-id="e41b0-126">2. Register a schema extension definition that describes a training course</span></span>
<span data-ttu-id="e41b0-127">Если вам не удастся найти расширение схемы, *соответствующее* вашим потребностям, вы можете создать и зарегистрировать новое определение расширения для учебных курсов в ресурсе **group**.</span><span class="sxs-lookup"><span data-stu-id="e41b0-127">If you can't find a schema extension that *is* appropriate for your needs, you can create and register a new extension definition for training courses on the **group** resource.</span></span>  

<span data-ttu-id="e41b0-p105">При создании определения расширения схемы нужно предоставить строку для свойства **id**. Это можно сделать двумя способами. В следующем примере показан предпочтительный способ с использованием запоминающегося доменного имени (`graphlearn.com`), проверенного в клиенте. Объедините проверенное доменное имя (`graphlearn`) с именем для расширения схемы (`courses`) и назначьте **id** с использованием полученной строки, `graphlearn_courses`.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p105">When creating a schema extension definition, you should provide a string for the **id** property. There are two ways to do this. The following example shows the preferred way, which uses a vanity domain name (`graphlearn.com`) that has been verified with your tenant. Concatenate the verified domain name (`graphlearn`) with a name for the schema extension (`courses`), and assign **id** with the resultant string, `graphlearn_courses`.</span></span>  

<span data-ttu-id="e41b0-p106">Затем укажите описание (необходимо для поиска), целевые типы (ресурсы, к которым применимо это расширение) и настраиваемые свойства, из которых состоит схема.  В этом примере укажите настраиваемые свойства `courseId`, `courseName` и `courseType`, а также их типы.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p106">Then, specify a description (to enable discoverability), target types (defining which resources this extension applies to), and the custom properties that make up the schema.  In this example, specify the `courseId`, `courseName` and `courseType` custom properties and their types.</span></span>

<span data-ttu-id="e41b0-134">См. [пример другого способа назначения **id** в запросе](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2), где требуется указать только имя схемы.</span><span class="sxs-lookup"><span data-stu-id="e41b0-134">See an [example of the other way to assign **id** in the request](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2), that requires you to provide only a schema name.</span></span>

<span data-ttu-id="e41b0-p107">Обратите внимание, что при первоначальном создании расширение схемы имеет состояние **InDevelopment**. Во время разработки расширения такое состояние можно сохранять. Пока оно не изменится, только ваше приложение, создавшее расширение, сможет его обновлять, внося дополнительные изменения, или удалять. Когда вы будете готовы предоставить доступ к расширению другим приложениям, установите для параметра **status** значение **Available**.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p107">Notice that when you initially create a schema extension, its status is **InDevelopment**. While you're developing the extension, you can keep it in this status, during which only your app that created it can update it with additive changes or delete it. When you are ready to share the extension for use by other apps, set **status** to **Available**.</span></span>

##### <a name="request"></a><span data-ttu-id="e41b0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e41b0-138">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e41b0-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e41b0-139">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
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

## <a name="3-create-a-new-group-with-extended-data"></a><span data-ttu-id="e41b0-140">3. Создание новой группы с расширенными данными</span><span class="sxs-lookup"><span data-stu-id="e41b0-140">3. Create a new group with extended data</span></span> 
<span data-ttu-id="e41b0-p108">Создайте _новую_ группу и расширьте ее, добавив дополнительные данные с помощью зарегистрированного определения расширения схемы `graphlearn_courses`.  Это стандартный запрос ```POST``` для ресурса **group** с дополнительным расширением сложного типа `graphlearn_courses`, определенным в теле запроса.  В ответе не будут отражены никакие расширения данных. Необходимо с помощью параметра ```$select``` указать имя расширения в операции ```GET```.</span><span class="sxs-lookup"><span data-stu-id="e41b0-p108">Create a _new_ group and extend it with extra data using the `graphlearn_courses` schema extension definition that we just registered.  This is a standard ```POST``` to the **group** resource, with the additional `graphlearn_courses` complex type extension defined in the request body.  The response will not mirror back any data extensions. We need to explicitly ```$select``` the extension by name using a ```GET``` operation.</span></span>

##### <a name="request"></a><span data-ttu-id="e41b0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="e41b0-145">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="e41b0-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="e41b0-146">Response</span></span>
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

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a><span data-ttu-id="e41b0-147">4. Добавление, обновление и удаление пользовательских данных существующей группы</span><span class="sxs-lookup"><span data-stu-id="e41b0-147">4. Add, update, or remove custom data in an existing group</span></span>
<span data-ttu-id="e41b0-148">Вы можете расширить существующий экземпляр _group_ и добавить в него пользовательские данные с помощью дополнительного расширения сложного типа `graphlearn_courses`, определенного в теле запроса ```PATCH```.</span><span class="sxs-lookup"><span data-stu-id="e41b0-148">You can extend and add custom data to an _existing_ group instance with the additional `graphlearn_courses` complex type extension defined in the body of a ```PATCH``` request.</span></span>  

##### <a name="request"></a><span data-ttu-id="e41b0-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e41b0-149">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
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
##### <a name="response"></a><span data-ttu-id="e41b0-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="e41b0-150">Response</span></span>
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="e41b0-151">Если вы хотите обновить значения данных расширения, поместите весь сложный тип расширения в тексте запроса ```PATCH``` (так же, как и при добавлении пользовательских данных к существующему ресурсу).</span><span class="sxs-lookup"><span data-stu-id="e41b0-151">If you want to update the values of the extension data, put the entire extension complex type in the body of a ```PATCH``` request (similar to adding custom data to an existing resource).</span></span>

<span data-ttu-id="e41b0-152">Вы также можете удалить пользовательские данные, добавленные в экземпляр ресурса, задав для соответствующего свойства расширения значение null.</span><span class="sxs-lookup"><span data-stu-id="e41b0-152">You can also remove custom data added to a resource instance by setting the corresponding extension property to null.</span></span> 

<span data-ttu-id="e41b0-153">Чтобы удалить расширение схемы из экземпляра ресурса, задайте для сложного типа расширения значение null.</span><span class="sxs-lookup"><span data-stu-id="e41b0-153">To remove a schema extension from a resource instance, set the extension complex type in that instance to null.</span></span>


## <a name="5-get-a-group-and-its-extension-data"></a><span data-ttu-id="e41b0-154">5. Получение экземпляра group и его данных расширения</span><span class="sxs-lookup"><span data-stu-id="e41b0-154">5. Get a group and its extension data</span></span>
<span data-ttu-id="e41b0-155">Удобный способ найти группу (или группы) — применить `$filter` с указанием определенных значений свойства расширения, например идентификатора или имени расширения.</span><span class="sxs-lookup"><span data-stu-id="e41b0-155">A handy way to look for a group (or groups) is to use `$filter` to match for specific extension property values, such as an extension name or ID.</span></span> 

<span data-ttu-id="e41b0-156">Затем, чтобы получить пользовательские данные группы, примените `$select`, чтобы включить расширение с указанием имени (в данном случае `graphlearn_courses`).</span><span class="sxs-lookup"><span data-stu-id="e41b0-156">Then, to get the custom data in a group, use `$select` to include the extension by name (in this case by `graphlearn_courses`).</span></span>

<span data-ttu-id="e41b0-p109">Приведенный ниже пример запроса ищет группу с расширением `graphlearn_courses`, для которой значение свойства `courseId` соответствует `123`, и получает свойства группы **displayName**, **id** и **description**, а также пользовательские данные расширения `graphlearn_courses`. (Выполняя реальный запрос, по необходимости применяйте URL-кодировку.)</span><span class="sxs-lookup"><span data-stu-id="e41b0-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

#### <a name="request"></a><span data-ttu-id="e41b0-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e41b0-159">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a><span data-ttu-id="e41b0-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="e41b0-160">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
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

## <a name="see-also"></a><span data-ttu-id="e41b0-161">См. также</span><span class="sxs-lookup"><span data-stu-id="e41b0-161">See also</span></span>

- [<span data-ttu-id="e41b0-162">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e41b0-162">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="e41b0-163">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e41b0-163">Add custom data to users using open extensions (preview)</span></span>](extensibility-open-users.md)
- [<span data-ttu-id="e41b0-164">Домены Office 365</span><span class="sxs-lookup"><span data-stu-id="e41b0-164">Office 365 domains</span></span>](https://technet.microsoft.com/ru-RU/library/office-365-domains.aspx)
- [<span data-ttu-id="e41b0-165">Добавление и проверка домена для НОВОГО плана Office 365</span><span class="sxs-lookup"><span data-stu-id="e41b0-165">Adding and Verifying a Domain for the NEW Office 365</span></span>](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="e41b0-166">Тип ресурса schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e41b0-166">schemaExtension resource type</span></span>](/graph/api/resources/schemaextension?view=graph-rest-1.0)
- [<span data-ttu-id="e41b0-167">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="e41b0-167">List schemaExtensions</span></span>](/graph/api/schemaextension-list?view=graph-rest-1.0)
- [<span data-ttu-id="e41b0-168">Создание schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e41b0-168">Create schemaExtension</span></span>](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0)
- [<span data-ttu-id="e41b0-169">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e41b0-169">Get schemaExtension</span></span>](/graph/api/schemaextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="e41b0-170">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e41b0-170">Update schemaExtension</span></span>](/graph/api/schemaextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="e41b0-171">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="e41b0-171">Delete schemaExtension</span></span>](/graph/api/schemaextension-delete?view=graph-rest-1.0)
