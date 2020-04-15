---
title: Список объектов mailFolder
description: 'Получение коллекции папок почты в корневой папке вошедшего пользователя. '
author: svpsiva
localization_priority: Priority
doc_type: apiPageType
ms.prod: outlook
ms.openlocfilehash: 3d232f130da7ef2e036f542ff40dd06af163a071
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376771"
---
# <a name="list-mailfolders"></a><span data-ttu-id="3feb3-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="3feb3-103">List mailFolders</span></span>

<span data-ttu-id="3feb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3feb3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3feb3-105">Получение коллекции папок почты непосредственно в корневой папке вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3feb3-105">Get the mail folder collection directly under the root folder of the signed-in user.</span></span> <span data-ttu-id="3feb3-106">Возвращаемая коллекция включает все [папки поиска почты](../resources/mailsearchfolder.md), расположенные непосредственно в корневой папке.</span><span class="sxs-lookup"><span data-stu-id="3feb3-106">The returned collection includes any [mail search folders](../resources/mailsearchfolder.md) directly under the root.</span></span>

## <a name="permissions"></a><span data-ttu-id="3feb3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3feb3-107">Permissions</span></span>
<span data-ttu-id="3feb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3feb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3feb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3feb3-110">Permission type</span></span>      | <span data-ttu-id="3feb3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3feb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3feb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3feb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3feb3-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3feb3-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3feb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3feb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3feb3-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3feb3-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="3feb3-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3feb3-116">Application</span></span> | <span data-ttu-id="3feb3-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3feb3-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3feb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3feb3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3feb3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3feb3-119">Optional query parameters</span></span>
<span data-ttu-id="3feb3-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3feb3-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3feb3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3feb3-121">Request headers</span></span>
| <span data-ttu-id="3feb3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3feb3-122">Header</span></span>       | <span data-ttu-id="3feb3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3feb3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3feb3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3feb3-124">Authorization</span></span>  | <span data-ttu-id="3feb3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3feb3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3feb3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3feb3-127">Content-Type</span></span>   | <span data-ttu-id="3feb3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3feb3-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3feb3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3feb3-129">Request body</span></span>
<span data-ttu-id="3feb3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3feb3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3feb3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3feb3-131">Response</span></span>

<span data-ttu-id="3feb3-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3feb3-132">If successful, this method returns a `200 OK` response code and a collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3feb3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3feb3-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3feb3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3feb3-134">Request</span></span>
<span data-ttu-id="3feb3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3feb3-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3feb3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="3feb3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="3feb3-137">C#</span><span class="sxs-lookup"><span data-stu-id="3feb3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3feb3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3feb3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3feb3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3feb3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3feb3-140">Java</span><span class="sxs-lookup"><span data-stu-id="3feb3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3feb3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="3feb3-141">Response</span></span>
<span data-ttu-id="3feb3-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3feb3-142">Here is an example of the response.</span></span>

><span data-ttu-id="3feb3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3feb3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
