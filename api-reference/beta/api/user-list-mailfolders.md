---
title: Список объектов mailFolder
description: Получение всех почтовых папок в почтовом ящике вошедшего пользователя.
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 6c218346a50666af625013b4b8ca1959c046d991
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409006"
---
# <a name="list-mailfolders"></a><span data-ttu-id="b1d35-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="b1d35-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1d35-104">Получение всех почтовых папок в почтовом ящике вошедшего пользователя, в том числе любых [папках поиска почты](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="b1d35-104">Get all the mail folders in the signed-in user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1d35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d35-105">Permissions</span></span>
<span data-ttu-id="b1d35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1d35-108">Permission type</span></span>      | <span data-ttu-id="b1d35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1d35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1d35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1d35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1d35-111">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1d35-111">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b1d35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1d35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1d35-113">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1d35-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b1d35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1d35-114">Application</span></span> | <span data-ttu-id="b1d35-115">Mail. ReadBasic. ALL, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1d35-115">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1d35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1d35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1d35-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1d35-117">Optional query parameters</span></span>
<span data-ttu-id="b1d35-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1d35-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1d35-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1d35-119">Request headers</span></span>
| <span data-ttu-id="b1d35-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1d35-120">Header</span></span>       | <span data-ttu-id="b1d35-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1d35-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1d35-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1d35-122">Authorization</span></span>  | <span data-ttu-id="b1d35-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1d35-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1d35-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1d35-125">Content-Type</span></span>   | <span data-ttu-id="b1d35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1d35-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1d35-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1d35-127">Request body</span></span>
<span data-ttu-id="b1d35-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1d35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1d35-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d35-129">Response</span></span>

<span data-ttu-id="b1d35-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1d35-130">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1d35-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b1d35-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1d35-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1d35-132">Request</span></span>
<span data-ttu-id="b1d35-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1d35-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b1d35-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d35-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1d35-135">C#</span><span class="sxs-lookup"><span data-stu-id="b1d35-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1d35-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1d35-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1d35-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1d35-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b1d35-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1d35-138">Response</span></span>
<span data-ttu-id="b1d35-139">Ниже приведен пример ответа, который включает в себя **маилсеарчфолдер** , который является дочерней папкой в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="b1d35-139">Here is an example of the response which includes a **mailSearchFolder** that is a child folder under the Inbox.</span></span> <span data-ttu-id="b1d35-140">Примечание. Представленный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b1d35-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1d35-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1d35-141">All of the properties will be returned from an actual call.</span></span>
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
