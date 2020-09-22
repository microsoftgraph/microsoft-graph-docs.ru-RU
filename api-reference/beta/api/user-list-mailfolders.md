---
title: Список объектов mailFolder
description: Получение всех почтовых папок в почтовом ящике вошедшего пользователя.
localization_priority: Normal
doc_type: apiPageType
author: svpsiva
ms.prod: outlook
ms.openlocfilehash: 757fb07765bcbe693909d422c5d4bdad2bd0c9e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016900"
---
# <a name="list-mailfolders"></a><span data-ttu-id="9ed8d-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="9ed8d-103">List mailFolders</span></span>

<span data-ttu-id="9ed8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ed8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed8d-105">Получение всех почтовых папок в почтовом ящике вошедшего пользователя, в том числе любых [папках поиска почты](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9ed8d-105">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed8d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed8d-106">Permissions</span></span>
<span data-ttu-id="9ed8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed8d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed8d-109">Permission type</span></span>      | <span data-ttu-id="9ed8d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ed8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ed8d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ed8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ed8d-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed8d-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ed8d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ed8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed8d-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed8d-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9ed8d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ed8d-115">Application</span></span> | <span data-ttu-id="9ed8d-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed8d-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed8d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ed8d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ed8d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ed8d-118">Optional query parameters</span></span>
<span data-ttu-id="9ed8d-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9ed8d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ed8d-120">Request headers</span></span>
| <span data-ttu-id="9ed8d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ed8d-121">Header</span></span>       | <span data-ttu-id="9ed8d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ed8d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ed8d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ed8d-123">Authorization</span></span>  | <span data-ttu-id="9ed8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ed8d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ed8d-126">Content-Type</span></span>   | <span data-ttu-id="9ed8d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ed8d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ed8d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ed8d-128">Request body</span></span>
<span data-ttu-id="9ed8d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ed8d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed8d-130">Response</span></span>

<span data-ttu-id="9ed8d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-131">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ed8d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9ed8d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ed8d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ed8d-133">Request</span></span>
<span data-ttu-id="9ed8d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed8d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed8d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="9ed8d-136">C#</span><span class="sxs-lookup"><span data-stu-id="9ed8d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed8d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed8d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed8d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed8d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9ed8d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed8d-139">Response</span></span>
<span data-ttu-id="9ed8d-140">Ниже приведен пример ответа, который включает в себя **маилсеарчфолдер** , который является дочерней папкой в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="9ed8d-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="9ed8d-141">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ed8d-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ed8d-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "archive"
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory"
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems"
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts"
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox"
        },
        {
            "@odata.type": "#microsoft.graph.mailSearchFolder",
            "id": "AAMkADYRAAAZg1yTAAA=",
            "displayName": "Weekly digests",
            "parentFolderId": "AQMkADYAAAIBDAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 4,
            "totalItemCount": 5,
            "wellKnownName": null,
            "isSupported": true,
            "filterQuery": "contains(subject, 'weekly digest')"
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "junkemail"
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox"
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


