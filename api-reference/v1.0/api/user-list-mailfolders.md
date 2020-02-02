---
title: Список объектов mailFolder
description: 'Получение коллекции папок почты в корневой папке вошедшего пользователя. '
author: angelgolfer-ms
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 1b802b636ce4a2a7e3b0b4b3c9c3c145842a9670
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652230"
---
# <a name="list-mailfolders"></a><span data-ttu-id="3977e-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="3977e-103">List mailFolders</span></span>

<span data-ttu-id="3977e-104">Получение коллекции папок почты непосредственно в корневой папке вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3977e-104">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="3977e-105">Возвращаемая коллекция включает все [папки поиска почты](../resources/mailsearchfolder.md), расположенные непосредственно в корневой папке.</span><span class="sxs-lookup"><span data-stu-id="3977e-105">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="3977e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3977e-106">Permissions</span></span>
<span data-ttu-id="3977e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3977e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3977e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3977e-109">Permission type</span></span>      | <span data-ttu-id="3977e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3977e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3977e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3977e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3977e-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3977e-112">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3977e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3977e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3977e-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3977e-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3977e-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3977e-115">Application</span></span> | <span data-ttu-id="3977e-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3977e-116">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3977e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3977e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3977e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3977e-118">Optional query parameters</span></span>
<span data-ttu-id="3977e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3977e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3977e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3977e-120">Request headers</span></span>
| <span data-ttu-id="3977e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3977e-121">Header</span></span>       | <span data-ttu-id="3977e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3977e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3977e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3977e-123">Authorization</span></span>  | <span data-ttu-id="3977e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3977e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3977e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3977e-126">Content-Type</span></span>   | <span data-ttu-id="3977e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3977e-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3977e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3977e-128">Request body</span></span>
<span data-ttu-id="3977e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3977e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3977e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3977e-130">Response</span></span>

<span data-ttu-id="3977e-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3977e-131">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3977e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3977e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3977e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3977e-133">Request</span></span>
<span data-ttu-id="3977e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3977e-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3977e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3977e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3977e-136">C#</span><span class="sxs-lookup"><span data-stu-id="3977e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3977e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3977e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3977e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3977e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3977e-139">Java</span><span class="sxs-lookup"><span data-stu-id="3977e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3977e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3977e-140">Response</span></span>
<span data-ttu-id="3977e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3977e-141">Here is an example of the response.</span></span>

><span data-ttu-id="3977e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3977e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/mailFolders",
    "value": [
        {
            "id": "AQMkADYAAAIBXQAAAA==",
            "displayName": "Archive",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71
        },
        {
            "id": "AQMkADYAAAIBGQAAAA==",
            "displayName": "Junk Email",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
