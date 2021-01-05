---
title: Список объектов mailFolder
description: Получите все почтовые папки в почтовом ящике пользователя, выписав его.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 7c8a73244b23b5fae115a844173d2ce3c7cb190f
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753958"
---
# <a name="list-mailfolders"></a><span data-ttu-id="03409-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="03409-103">List mailFolders</span></span>

<span data-ttu-id="03409-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03409-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03409-105">Получите все почтовые папки в почтовом ящике указанного пользователя, включая все папки [поиска почты.](../resources/mailsearchfolder.md)</span><span class="sxs-lookup"><span data-stu-id="03409-105">Get all the mail folders in the specified user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="03409-106">По умолчанию эта операция не возвращает скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="03409-106">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="03409-107">Используйте параметр _запроса includeHiddenFolders,_ чтобы включить их в ответ.</span><span class="sxs-lookup"><span data-stu-id="03409-107">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="03409-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03409-108">Permissions</span></span>
<span data-ttu-id="03409-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03409-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03409-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03409-111">Permission type</span></span>      | <span data-ttu-id="03409-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03409-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03409-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03409-113">Delegated (work or school account)</span></span> | <span data-ttu-id="03409-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03409-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="03409-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03409-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03409-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03409-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="03409-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03409-117">Application</span></span> | <span data-ttu-id="03409-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03409-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="03409-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03409-119">HTTP request</span></span>

<span data-ttu-id="03409-120">Чтобы получить все почтовые папки в почтовом ящике указанного пользователя, за исключением скрытых папок:</span><span class="sxs-lookup"><span data-stu-id="03409-120">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="03409-121">Чтобы включить _скрытые_ почтовые папки в ответ:</span><span class="sxs-lookup"><span data-stu-id="03409-121">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="query-parameters"></a><span data-ttu-id="03409-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="03409-122">Query parameters</span></span>
<span data-ttu-id="03409-123">Чтобы получить список всех объектов mailFolders, включая скрытые (их свойство **isHidden** имеет true), в URL-адресе запроса укажите параметр запроса как , как показано в разделе `includeHiddenFolders` `true` [HTTP-запроса.](#http-request)</span><span class="sxs-lookup"><span data-stu-id="03409-123">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="03409-124">Этот метод также поддерживает [параметры запроса OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="03409-124">This method also supports [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03409-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03409-125">Request headers</span></span>
| <span data-ttu-id="03409-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03409-126">Header</span></span>       | <span data-ttu-id="03409-127">Значение</span><span class="sxs-lookup"><span data-stu-id="03409-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03409-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03409-128">Authorization</span></span>  | <span data-ttu-id="03409-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03409-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03409-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03409-131">Request body</span></span>
<span data-ttu-id="03409-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03409-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03409-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="03409-133">Response</span></span>

<span data-ttu-id="03409-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03409-134">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="03409-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="03409-135">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="03409-136">Пример 1. Список папок почты в почтовом ящике пользователя, выписав его</span><span class="sxs-lookup"><span data-stu-id="03409-136">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="03409-137">В этом примере в **ответ включается объект mailSearchFolder.**</span><span class="sxs-lookup"><span data-stu-id="03409-137">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="03409-138">Папка поиска почты — это папка под папкой "Входящие" с отображаемым именем "Еженедельные дайджесты".</span><span class="sxs-lookup"><span data-stu-id="03409-138">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="03409-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="03409-139">Request</span></span>
<span data-ttu-id="03409-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03409-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="03409-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="03409-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="03409-142">C#</span><span class="sxs-lookup"><span data-stu-id="03409-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03409-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03409-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03409-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03409-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03409-145">Java</span><span class="sxs-lookup"><span data-stu-id="03409-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="03409-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="03409-146">Response</span></span>
<span data-ttu-id="03409-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03409-147">Here is an example of the response.</span></span> 

><span data-ttu-id="03409-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="03409-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
            "wellKnownName": "archive",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBFQAAAA==",
            "displayName": "Conversation History",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCgAAAA==",
            "displayName": "Deleted Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "deleteditems",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDwAAAA==",
            "displayName": "Drafts",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "drafts",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBDAAAAA==",
            "displayName": "Inbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 1,
            "unreadItemCount": 70,
            "totalItemCount": 71,
            "wellKnownName": "inbox",
            "isHidden": false
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
            "isHidden": false,
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
            "wellKnownName": "junkemail",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCwAAAA==",
            "displayName": "Outbox",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "outbox",
            "isHidden": false
        },
        {
            "id": "AQMkADYAAAIBCQAAAA==",
            "displayName": "Sent Items",
            "parentFolderId": "AQMkADYAAAIBCAAAAA==",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "sentitems",
            "isHidden": false
        }
    ]
}
```


### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="03409-149">Пример 2. Включив скрытые папки в почтовый ящик во включенного пользователя</span><span class="sxs-lookup"><span data-stu-id="03409-149">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="03409-150">В следующем примере параметр запроса используется для получения списка почтовых папок, `includeHiddenFolders` включая скрытые почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="03409-150">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="03409-151">Ответ включает папку "Clutters", для нее **задав для isHidden** задав true.</span><span class="sxs-lookup"><span data-stu-id="03409-151">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="03409-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="03409-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```

#### <a name="response"></a><span data-ttu-id="03409-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="03409-153">Response</span></span>
<span data-ttu-id="03409-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03409-154">Here is an example of the response.</span></span>

><span data-ttu-id="03409-155">**Примечание.** Показанный здесь объект ответа сокращен для учитаемости и не включает все папки по умолчанию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="03409-155">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Clutters",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 0,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": null,
            "isHidden": true
        },
        {
            "id": "AAMkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWAAA=",
            "displayName": "Conversation History",
            "parentFolderId": "AAMkADg3NTY5MDg4LWMzYmQtEIAAA=",
            "childFolderCount": 1,
            "unreadItemCount": 0,
            "totalItemCount": 0,
            "wellKnownName": "conversationhistory",
            "isHidden": false
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
