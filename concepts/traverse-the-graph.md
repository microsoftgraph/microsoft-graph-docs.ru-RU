---
title: Доступ к данным и методам с помощью Microsoft Graph
description: Помимо чтения и записи данных с помощью API Microsoft Graph, вы можете использовать шаблоны запросов для просмотра ресурсов в Microsoft Graph. Документ метаданных поможет вам разобраться в модели данных ресурсов и отношений в Microsoft Graph.
localization_priority: Priority
scenarios: getting-started
ms.custom: graphiamtop20
ms.openlocfilehash: 57cdb0d482a2f0d2ba127a97dc3231056be13e24
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053888"
---
# <a name="access-data-and-methods-by-navigating-microsoft-graph"></a><span data-ttu-id="936bb-104">Доступ к данным и методам с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="936bb-104">Access data and methods by navigating Microsoft Graph</span></span>

<span data-ttu-id="936bb-p102">Помимо чтения и записи данных с помощью API Microsoft Graph, вы можете использовать шаблоны запросов для просмотра ресурсов в Microsoft Graph. Документ метаданных поможет вам разобраться в модели данных ресурсов и отношений в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="936bb-p102">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="936bb-107">Метаданные API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="936bb-107">Microsoft Graph API metadata</span></span>

<span data-ttu-id="936bb-p103">Документ метаданных ($metadata) публикуется в корневом каталоге службы. По указанным ниже URL-адресам можно просмотреть сервисный документ для версии 1.0 и бета-версии API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="936bb-p103">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="936bb-110">**Метаданные API Microsoft Graph 1.0**</span><span class="sxs-lookup"><span data-stu-id="936bb-110">**Microsoft Graph API v1.0 metadata**</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="936bb-111">**Метаданные API Microsoft Graph (бета-версия)**</span><span class="sxs-lookup"><span data-stu-id="936bb-111">**Microsoft Graph API beta metadata**</span></span>

```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="936bb-112">Метаданные позволяют разобраться в модели данных Microsoft Graph, в том числе типах объектов, сложных типах и перечислениях, из которых состоят ресурсы, представленные в пакетах запросов и откликов.</span><span class="sxs-lookup"><span data-stu-id="936bb-112">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span>

<span data-ttu-id="936bb-113">С помощью метаданных можно узнать об отношениях между объектами в Microsoft Graph и создать URL-адреса для перехода между ними.</span><span class="sxs-lookup"><span data-stu-id="936bb-113">You can use the metadata to learn the realtionships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

> [!NOTE]
> - <span data-ttu-id="936bb-114">Используйте идентификаторы ресурсов в том же регистре, в котором они возвращаются из API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="936bb-114">Use resource IDs in the same case as they are returned from Microsoft Graph APIs.</span></span>
> - <span data-ttu-id="936bb-115">Считайте, что идентификаторы ресурсов, назначаемые значения и другие значения в кодировке base64 указываются _с учетом регистра_.</span><span class="sxs-lookup"><span data-stu-id="936bb-115">Assume resource IDs, values you assign, and other base-64-encoded values are _case-sensitive_.</span></span>
> - <span data-ttu-id="936bb-116">Считайте, что имена ресурсов URL-адреса пути, параметры запросов, имена действий и функций, их параметры текста запроса, включая названия и значения свойств API указываются _без учета регистра_.</span><span class="sxs-lookup"><span data-stu-id="936bb-116">Assume path URL resource names, query parameters, action and function names, their request body parameters, including any API property names and values, are _not case-sensitive_.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="936bb-117">Просмотр коллекции ресурсов</span><span class="sxs-lookup"><span data-stu-id="936bb-117">View a collection of resources</span></span>

<span data-ttu-id="936bb-118">Microsoft Graph позволяет просматривать ресурсы в клиенте с помощью HTTP-запросов `GET`.</span><span class="sxs-lookup"><span data-stu-id="936bb-118">Microsoft Graph lets you view resources in a tenant using HTTP `GET` queries.</span></span> <span data-ttu-id="936bb-119">Отклик на запрос включает свойства каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="936bb-119">The query response includes properties of each resource.</span></span> <span data-ttu-id="936bb-120">Каждый ресурс объекта определяется по соответствующему идентификатору.</span><span class="sxs-lookup"><span data-stu-id="936bb-120">Entity resources are each identified by its ID.</span></span> <span data-ttu-id="936bb-121">ИД ресурса может быть GUID, его формат обычно зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="936bb-121">The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span>

<span data-ttu-id="936bb-122">Например, можно получить коллекцию ресурсов [user](/graph/api/resources/user?view=graph-rest-1.0), определенных в клиенте:</span><span class="sxs-lookup"><span data-stu-id="936bb-122">For example, you can get the collection of users defined in a tenant:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-p105">При успешном выполнении запроса будет получен отклик 200 OK, который содержит полезные данные с коллекцией ресурсов **user**. Каждый объект user идентифицируется по свойству **id** и сопровождается свойствами по умолчанию. Полезные данные, показанные ниже, усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="936bb-p105">If successful, you'll get a 200 OK response that contains the collection of **user** resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

<span data-ttu-id="936bb-p106">Microsoft Graph позволяет также просматривать коллекции, переходя к нужному отношению, которым связаны ресурсы. Например, применяя свойство навигации **mailFolders** объекта user, вы можете запрашивать коллекцию ресурсов [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="936bb-p106">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) resources in the user's mailbox:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-p107">При успешном выполнении запроса будет получен отклик 200 OK, который содержит полезные данные с коллекцией ресурсов [mailFolder](/graph/api/resources/user?view=graph-rest-1.0). Каждый объект **mailFolder** определяется по его свойству **id** и сопровождается другими свойствами. Полезные данные, показанные ниже, усечены для краткости.</span><span class="sxs-lookup"><span data-stu-id="936bb-p107">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](/graph/api/resources/user?view=graph-rest-1.0) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="936bb-131">Просмотр ресурса из коллекции по идентификатору</span><span class="sxs-lookup"><span data-stu-id="936bb-131">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="936bb-132">Еще раз приведем ресурс **user** в качестве примера. Чтобы просмотреть сведения об определенном пользователе, отправьте HTTPS-запрос GET, указав идентификатор объекта user.</span><span class="sxs-lookup"><span data-stu-id="936bb-132">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a user entity, you can use either the id or userPrincipalName property as the identifier. The following request example uses the userPrincipalName value as the user's ID.</span></span> <span data-ttu-id="936bb-133">Для объекта **user** в качестве идентификатора можно использовать свойство **id** или **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="936bb-133">For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier.</span></span>

<span data-ttu-id="936bb-134">В следующем примере запроса в качестве идентификатора используется значение **userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="936bb-134">The following example request uses the \*\*\*\* value as the user's id.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-135">При успешном выполнении запроса будет получен отклик 200 OK, содержащий полезные данные с представлением ресурса user, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="936bb-135">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

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

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="936bb-136">Чтение определенных свойств ресурса</span><span class="sxs-lookup"><span data-stu-id="936bb-136">Read specific properties of a resource</span></span>
<span data-ttu-id="936bb-137">Чтобы получить только биографические данные пользователя, например предоставленное им описание в разделе _Обо мне_ и набор квалификационных навыков, в предыдущий запрос можно добавить параметр [$select](query-parameters.md), как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="936bb-137">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query-parameters.md) query parameter to the previous request, as shown in the following example.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-138">При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="936bb-138">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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
<span data-ttu-id="936bb-139">Здесь возвращаются не полные наборы свойств для объекта **user**, а только основные свойства **aboutMe**, **displayName** и **skills**.</span><span class="sxs-lookup"><span data-stu-id="936bb-139">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="936bb-140">Чтение отдельных свойств ресурсов в коллекции</span><span class="sxs-lookup"><span data-stu-id="936bb-140">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="936bb-141">Вы можете не только просматривать отдельные свойства одного ресурса, но и получить все ее ресурсы только с указанными свойствами, применив к коллекции аналогичный параметр запроса [$select](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="936bb-141">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query-parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

<span data-ttu-id="936bb-142">Например, чтобы запросить имена элементов на диске вошедшего пользователя, можно отправить следующий HTTPS-запрос GET.</span><span class="sxs-lookup"><span data-stu-id="936bb-142">For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-143">При успешном ответе возвращаются код состояния 200 OK и полезные данные, содержащие только имена общих файлов, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="936bb-143">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="936bb-144">Переход от одного ресурса к другому с помощью отношения</span><span class="sxs-lookup"><span data-stu-id="936bb-144">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="936bb-p109">Руководитель состоит в отношении **directReports** со своими подчиненными. Чтобы запросить список подчиненных пользователя, можно использовать приведенный ниже HTTPS-запрос GET для перехода к целевому объекту с помощью отношения.</span><span class="sxs-lookup"><span data-stu-id="936bb-p109">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span>

```no-highlight
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="936bb-147">При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="936bb-147">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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

<span data-ttu-id="936bb-p110">Аналогичным образом можно переходить к ресурсам, используя их отношения. Например, отношение user-messages позволяет перейти от пользователя Azure Active Directory (AD) к набору сообщений Outlook. В приведенном ниже примере показано, как это сделать в вызове REST API.</span><span class="sxs-lookup"><span data-stu-id="936bb-p110">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```no-highlight
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```


<span data-ttu-id="936bb-151">При успешном выполнении запроса в отклике возвращаются полезные данные и состояние 200 OK, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="936bb-151">The successful response returns the 200 OK status and a payload, as shown.</span></span>


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
<span data-ttu-id="936bb-152">Чтобы просмотреть все отношения для ресурса, откройте метаданные, найдите параметр `EntityType` и просмотрите все его свойства `NavigationProperty`.</span><span class="sxs-lookup"><span data-stu-id="936bb-152">You can see all the relationships on a given resource by going to the metadata, finding the EntityType, and looking at all NavigationProperties for that EntityType.</span></span>

## <a name="call-actions-and-functions"></a><span data-ttu-id="936bb-153">Вызов действий и функций</span><span class="sxs-lookup"><span data-stu-id="936bb-153">Call actions or functions</span></span>
<span data-ttu-id="936bb-154">Microsoft Graph также поддерживает _действия_ и _функции_ для выполнения с ресурсами действий, отличных от простых операций CRUD (создание, чтение, обновление и удаление).</span><span class="sxs-lookup"><span data-stu-id="936bb-154">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations.</span></span> <span data-ttu-id="936bb-155">Они часто имеют форму HTTPS-запросов POST, принимающих аргументы для действия или функции.</span><span class="sxs-lookup"><span data-stu-id="936bb-155">They are often in the shape of HTTPS POST requests in order to intake arguments for the action or function.</span></span> <span data-ttu-id="936bb-156">Например, с помощью указанного ниже действия вошедший пользователь (`me`) может отправить сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="936bb-156">For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>

```no-highlight
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
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
          "address": "garthf@contoso.onmicrosoft.com"
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

<span data-ttu-id="936bb-p112">Вы можете просмотреть все доступные функции в метаданных. Они отображаются как функции или действия.</span><span class="sxs-lookup"><span data-stu-id="936bb-p112">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="936bb-159">Использование пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="936bb-159">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="936bb-p113">Вам нравятся возможности и удобство пакетов SDK? Вы всегда можете вызывать Microsoft Graph с помощью REST API, но мы также предоставляем пакеты SDK для многих популярных платформ. Обзор доступных пакетов SDK см. в разделе [Примеры кода и пакеты SDK](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="936bb-p113">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="936bb-163">См. также</span><span class="sxs-lookup"><span data-stu-id="936bb-163">See also</span></span>

- [<span data-ttu-id="936bb-164">Использование API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="936bb-164">Use the Microsoft Graph API</span></span>](use-the-api.md)
- [<span data-ttu-id="936bb-165">Получение токенов аутентификации</span><span class="sxs-lookup"><span data-stu-id="936bb-165">Get auth tokens</span></span>](/graph/auth)
