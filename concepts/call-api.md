---
title: Вызов API Microsoft Graph
description: 'Для доступа к ресурсу Microsoft Graph и работы с ним необходимо вызвать и указать URL-адреса ресурса, используя одну из указанных ниже операций.   '
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
ms.openlocfilehash: 627fb614f8084abe6980ed095a7a55adfa6a3f12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970418"
---
# <a name="calling-the-microsoft-graph-api"></a><span data-ttu-id="131f6-103">Вызов API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="131f6-103">Calling the Microsoft Graph API</span></span>

<span data-ttu-id="131f6-104">Для доступа к ресурсу Microsoft Graph и работы с ним необходимо вызвать и указать URL-адреса ресурса, используя одну из указанных ниже операций.</span><span class="sxs-lookup"><span data-stu-id="131f6-104">To access and manipulate a Microsoft Graph resource, you call and specify the resource URLs using one of the following operations:</span></span>   

- <span data-ttu-id="131f6-105">GET</span><span class="sxs-lookup"><span data-stu-id="131f6-105">GET</span></span>
- <span data-ttu-id="131f6-106">POST</span><span class="sxs-lookup"><span data-stu-id="131f6-106">POST</span></span>
- <span data-ttu-id="131f6-107">PATCH</span><span class="sxs-lookup"><span data-stu-id="131f6-107">PATCH</span></span>
- <span data-ttu-id="131f6-108">PUT</span><span class="sxs-lookup"><span data-stu-id="131f6-108">PUT</span></span>
- <span data-ttu-id="131f6-109">DELETE</span><span class="sxs-lookup"><span data-stu-id="131f6-109">DELETE</span></span> 

<span data-ttu-id="131f6-110">Во всех запросах API Microsoft Graph используется следующий базовый шаблон URL-адреса:</span><span class="sxs-lookup"><span data-stu-id="131f6-110">All Microsoft Graph API requests use the following basic URL pattern:</span></span>

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

<span data-ttu-id="131f6-111">В этом URL-адресе:</span><span class="sxs-lookup"><span data-stu-id="131f6-111">For this URL:</span></span>

- <span data-ttu-id="131f6-112">`https://graph.microsoft.com` — это конечная точка API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="131f6-112">`https://graph.microsoft.com` is the Microsoft Graph API endpoint.</span></span>
- <span data-ttu-id="131f6-113">`{version}` — это целевая версия службы, например `v1.0` или `beta`.</span><span class="sxs-lookup"><span data-stu-id="131f6-113">`{version}` is the target service version, for example, `v1.0` or `beta`.</span></span>
- <span data-ttu-id="131f6-114">`{resource}` — это сегмент ресурсов или путь, например:</span><span class="sxs-lookup"><span data-stu-id="131f6-114">`{resource}` is resource segment or path, such as:</span></span>
  - <span data-ttu-id="131f6-115">`users`, `groups`, `devices`, `organization`</span><span class="sxs-lookup"><span data-stu-id="131f6-115">`users`, `groups`, `devices`, `organization`</span></span>
  - <span data-ttu-id="131f6-116">псевдоним `me`, который сопоставляется с вошедшим пользователем;</span><span class="sxs-lookup"><span data-stu-id="131f6-116">The alias `me`, which resolves to the signed-in user</span></span>
   - <span data-ttu-id="131f6-117">ресурсы, принадлежащие пользователю, такие как `me/events`, `me/drive` или `me/messages`;</span><span class="sxs-lookup"><span data-stu-id="131f6-117">The resources belonging to a user, such as `me/events`, `me/drive` or `me/messages`</span></span>
  - <span data-ttu-id="131f6-118">псевдоним `myOrganization`, который сопоставляется с клиентом организации вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="131f6-118">The alias `myOrganization`, which resolves to the tenant of the organization signed-in user</span></span>
- <span data-ttu-id="131f6-119">`[query_parameters]` представляет дополнительные параметры запроса, такие как `$filter` и `$select`.</span><span class="sxs-lookup"><span data-stu-id="131f6-119">`[query_parameters]` represents additional query parameters such as `$filter` and `$select`.</span></span>

<span data-ttu-id="131f6-p101">При желании вы также можете указать клиент в составе запроса. Если используется псевдоним `me`, не указывайте клиент. Список распространенных запросов см. в статье [Обзор Microsoft Graph](overview.md).</span><span class="sxs-lookup"><span data-stu-id="131f6-p101">Optionally, you can also specify the tenant as part of your request. When using `me`, do not specify the tenant. For a list of common requests, see [Overview of Microsoft Graph](overview.md).</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="131f6-123">Метаданные API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="131f6-123">Microsoft Graph API metadata</span></span>
<span data-ttu-id="131f6-p102">Документ метаданных ($metadata) публикуется в корневом каталоге службы. Например, по указанным ниже URL-адресам можно просмотреть сервисный документ для версии 1.0 и бета-версии.</span><span class="sxs-lookup"><span data-stu-id="131f6-p102">The metadata document ($metadata) is published at the service root. For example, you can view the service document for the v1.0 and beta versions via the following URLs.</span></span>

<span data-ttu-id="131f6-126">Метаданные API Microsoft Graph `v1.0`.</span><span class="sxs-lookup"><span data-stu-id="131f6-126">Microsoft Graph API `v1.0` metadata.</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```
<span data-ttu-id="131f6-127">Метаданные API Microsoft Graph `beta`.</span><span class="sxs-lookup"><span data-stu-id="131f6-127">Microsoft Graph API `beta` metadata.</span></span>
```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="131f6-128">Метаданные помогают просматривать и анализировать модель данных Microsoft Graph, в том числе типы и наборы сущностей, сложные типы и перечисления, входящие в состав запроса и пакетов ответа, отправляемых в службу Microsoft Graph и из нее.</span><span class="sxs-lookup"><span data-stu-id="131f6-128">The metadata allows you to see and understand the data model of Microsoft Graph, including the entity types and sets, complex types, and enums that make up the request and response packets sent to and from Microsoft Graph.</span></span>
<span data-ttu-id="131f6-129">С помощью метаданных вы сможете понять связи между сущностями в Microsoft Graph и создать URL-адреса для перехода между ними.</span><span class="sxs-lookup"><span data-stu-id="131f6-129">You can use the metadata to understand the realtionships between entities in Microsoft Graph and establish URLs that navigate between entities.</span></span>
<span data-ttu-id="131f6-130">Такая взаимосвязь на основе навигации является уникальной характеристикой Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="131f6-130">This navigation-based interconnectedness gives Microsoft Graph its unique character.</span></span>

<span data-ttu-id="131f6-131">Названия ресурсов URL-адреса пути, параметры запросов, а также параметры и значения действий указываются без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="131f6-131">Path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span> <span data-ttu-id="131f6-132">Однако назначаемые значения, идентификаторы объектов и другие значения в кодировке base64 указываются с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="131f6-132">However, values you assign, entity IDs, and other base64-encoded values are case-sensitive.</span></span>

<span data-ttu-id="131f6-133">В следующих разделах представлено несколько базовых шаблонов программирования вызовов к API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="131f6-133">The following sections show a few basic programming pattern calls to the Microsoft Graph API.</span></span>

## <a name="navigate-from-a-set-to-a-member"></a><span data-ttu-id="131f6-134">Переход от набора к элементу</span><span class="sxs-lookup"><span data-stu-id="131f6-134">Navigate from a set to a member</span></span>

<span data-ttu-id="131f6-p105">Чтобы просмотреть сведения о пользователе, необходимо получить объект `User` из коллекции `users` для конкретного пользователя, на которого указывает идентификатор, используя HTTPS-запрос GET. Для объекта `User` в качестве идентификатора можно использовать свойство `id` или `userPrincipalName`. В следующем примере запроса в качестве идентификатора пользователя используется значение `userPrincipalName`.</span><span class="sxs-lookup"><span data-stu-id="131f6-p105">To view the information about a user, you get the `User` entity from the `users` collection to the specific user identified by its identifier, using an HTTPS GET request. For a `User` entity, either the `id` or `userPrincipalName` property can be used as the identifier. The following example request uses the `userPrincipalName` value as the user's id.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="131f6-138">При успешном выполнении действия вы получите ответ 200 OK, содержащий полезные данные с представлением ресурса user, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="131f6-138">If successful, you should get a 200 OK response containing the user resource representation in the payload, as shown as follows:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```


## <a name="project-from-an-entity-to-properties"></a><span data-ttu-id="131f6-139">Проекция из объекта на свойства</span><span class="sxs-lookup"><span data-stu-id="131f6-139">Project from an entity to properties</span></span>
<span data-ttu-id="131f6-p106">Чтобы получить только биографические сведения пользователя, например предоставленное им описание в разделе _Обо мне_ и указанные навыки, вы можете добавить в предыдущий запрос параметр _select_. Например:</span><span class="sxs-lookup"><span data-stu-id="131f6-p106">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the _select_ query parameter to the previous request. For example:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="131f6-142">При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="131f6-142">The successful response returns the 200 OK status and a payload of the following format:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```

<span data-ttu-id="131f6-143">Здесь возвращаются не наборы свойств для объекта `user`, а только свойства `aboutMe`, `displayName` и `skills`.</span><span class="sxs-lookup"><span data-stu-id="131f6-143">Here, instead of the entire property sets on the `user` entity, only the `aboutMe`, `displayName`, and `skills` properties are returned.</span></span>

## <a name="traverse-to-another-resource-via-relationship"></a><span data-ttu-id="131f6-144">Переход к другому ресурсу с помощью отношения</span><span class="sxs-lookup"><span data-stu-id="131f6-144">Traverse to another resource via relationship</span></span>
<span data-ttu-id="131f6-p107">Руководитель состоит в отношении `directReports` со своими подчиненными. Чтобы запросить список подчиненных пользователя, можно использовать приведенный ниже HTTPS-запрос GET для перехода к целевому объекту с помощью отношения.</span><span class="sxs-lookup"><span data-stu-id="131f6-p107">A manager holds a `directReports` relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="131f6-147">При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="131f6-147">The successful response returns the 200 OK status and a payload of the following format:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

<span data-ttu-id="131f6-p108">Аналогичным образом вы можете воспользоваться отношением, чтобы перейти к связанным ресурсам. Например, отношение `user => messages` позволяет перейти от пользователя Azure AD к набору сообщений Outlook. В приведенном ниже примере показано, как это сделать в вызове API REST:</span><span class="sxs-lookup"><span data-stu-id="131f6-p108">Similarly, you can follow a relationship to navigate to related resources. For example, the `user => messages` relationship enables traversal from an Azure AD User to a set of Outlook mail messages. The following example shows how to do this in a REST API call:</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
<span data-ttu-id="131f6-151">При успешном ответе возвращаются состояние 200 OK и полезные данные в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="131f6-151">The successful response returns the 200 OK status and a payload of the following format:</span></span>


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```

## <a name="project-from-entities-to-properties"></a><span data-ttu-id="131f6-152">Проекция из объектов на свойства</span><span class="sxs-lookup"><span data-stu-id="131f6-152">Project from entities to properties</span></span>
<span data-ttu-id="131f6-p109">Помимо проекции из одного объекта на его свойства, вы также можете применить такой же параметр запроса `select` к коллекции объектов, чтобы спроецировать их на коллекцию некоторых их свойств. Например, чтобы запросить имена элементов на диске вошедшего пользователя, вы можете отправить следующий HTTPS-запрос GET:</span><span class="sxs-lookup"><span data-stu-id="131f6-p109">In addition to projection from a single entity to its properties, you can also apply the similar `select` query option to an entity collection to project them to a collection of some of their properties. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="131f6-155">При успешном ответе возвращается код состояния 200 OK и полезные данные, содержащие имена и типы общих файлов, как показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="131f6-155">The successful response returns a 200 OK status code and a payload containing the names and types of the shared files, as shown in the following example:</span></span>

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a><span data-ttu-id="131f6-156">Запрос подмножества пользователей с помощью параметра фильтрации</span><span class="sxs-lookup"><span data-stu-id="131f6-156">Query a subset of users with the filtering query option</span></span>
<span data-ttu-id="131f6-p110">Чтобы найти сотрудников, занимающих определенную должность в организации, можно перейти из коллекции пользователей, а затем указать параметр запроса _filter_. Пример:</span><span class="sxs-lookup"><span data-stu-id="131f6-p110">To find the employees of a specific job title within an organization, you can navigate from the users collection and then specify a _filter_ query option. An example is shown as follows:</span></span>

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="131f6-159">При успешном ответе возвращаются код состояния 200 OK и список пользователей, занимающих указанную должность (`'Helper'`), как показано в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="131f6-159">The successful response returns the 200 OK status code and a list of users with the specified job title (`'Helper'`), as shown in the following example:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a><span data-ttu-id="131f6-160">Вызов действий и функций</span><span class="sxs-lookup"><span data-stu-id="131f6-160">Call actions or functions</span></span>
<span data-ttu-id="131f6-p111">Microsoft Graph также поддерживает _действия_ и _функции_ для управления ресурсами с использованием методов, которые сложно совмещать со стандартными методами HTTP. Например, с помощью приведенного ниже HTTPS-запроса POST вошедший пользователь (`me`) может отправить электронное сообщение.</span><span class="sxs-lookup"><span data-stu-id="131f6-p111">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not a simple fit with standard HTTP methods. For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>
```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

<span data-ttu-id="131f6-163">Полезные данные запроса содержат входные данные для действия `sendMail`, которые также определены в документе $metadata.</span><span class="sxs-lookup"><span data-stu-id="131f6-163">The request payload contains the input to the `sendMail` action, which is also defined in the $metadata.</span></span>

## <a name="use-microsoft-graph-client-libraries"></a><span data-ttu-id="131f6-164">Использование клиентских библиотек Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="131f6-164">Use Microsoft Graph client libraries</span></span>
<span data-ttu-id="131f6-p112">Вам нравятся возможности и удобство пакетов SDK? Вы всегда можете вызывать Microsoft Graph с помощью REST API, но мы также предоставляем пакеты SDK для многих популярных платформ.</span><span class="sxs-lookup"><span data-stu-id="131f6-p112">Like the power and ease of SDKs? While you can always call Microsoft Graph using the REST API, we also provide SDKs for many popular platforms.</span></span>

<span data-ttu-id="131f6-167">Изучите наши [примеры кода и пакеты SDK](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="131f6-167">Explore our [code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
