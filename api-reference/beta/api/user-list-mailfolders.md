---
title: Список объектов mailFolder
description: Получение всех почтовых папок в почтовом ящике вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: c006e1f4b8714c332b9a1d3144c660784fda11f5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867243"
---
# <a name="list-mailfolders"></a><span data-ttu-id="85fee-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="85fee-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85fee-104">Получение всех почтовых папок в почтовом ящике вошедшего пользователя, в том числе любых [папках поиска почты](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="85fee-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85fee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85fee-105">Permissions</span></span>
<span data-ttu-id="85fee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85fee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85fee-108">Permission type</span></span>      | <span data-ttu-id="85fee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85fee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85fee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85fee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85fee-111">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85fee-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="85fee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85fee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85fee-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85fee-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="85fee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85fee-114">Application</span></span> | <span data-ttu-id="85fee-115">Mail. ReadBasic. ALL, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85fee-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85fee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85fee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85fee-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85fee-117">Optional query parameters</span></span>
<span data-ttu-id="85fee-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85fee-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="85fee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85fee-119">Request headers</span></span>
| <span data-ttu-id="85fee-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85fee-120">Header</span></span>       | <span data-ttu-id="85fee-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85fee-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85fee-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85fee-122">Authorization</span></span>  | <span data-ttu-id="85fee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85fee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85fee-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85fee-125">Content-Type</span></span>   | <span data-ttu-id="85fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85fee-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85fee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85fee-127">Request body</span></span>
<span data-ttu-id="85fee-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85fee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85fee-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="85fee-129">Response</span></span>

<span data-ttu-id="85fee-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85fee-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85fee-131">Пример</span><span class="sxs-lookup"><span data-stu-id="85fee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85fee-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="85fee-132">Request</span></span>
<span data-ttu-id="85fee-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85fee-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="85fee-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="85fee-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="85fee-135">C#</span><span class="sxs-lookup"><span data-stu-id="85fee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85fee-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="85fee-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85fee-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="85fee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="85fee-138">Java</span><span class="sxs-lookup"><span data-stu-id="85fee-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85fee-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="85fee-139">Response</span></span>
<span data-ttu-id="85fee-140">Ниже приведен пример ответа, который включает в себя **маилсеарчфолдер** , который является дочерней папкой в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="85fee-140">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="85fee-141">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="85fee-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="85fee-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85fee-142">All of the properties will be returned from an actual call.</span></span>
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
