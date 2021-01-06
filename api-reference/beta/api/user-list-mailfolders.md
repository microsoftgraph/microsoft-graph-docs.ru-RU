---
title: Список объектов mailFolder
description: Получите все почтовые папки в почтовом ящике пользователя, выписав его.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: c2cf43dc9d01ba2de2a3426cce84aaf3f92bbbb3
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768218"
---
# <a name="list-mailfolders"></a><span data-ttu-id="da2bf-103">Список объектов mailFolder</span><span class="sxs-lookup"><span data-stu-id="da2bf-103">List mailFolders</span></span>

<span data-ttu-id="da2bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da2bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da2bf-105">Получите все почтовые папки в почтовом ящике указанного пользователя, включая все папки [поиска почты.](../resources/mailsearchfolder.md)</span><span class="sxs-lookup"><span data-stu-id="da2bf-105">Get all the mail folders in the specified user's mailbox, including any [mail search folders](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="da2bf-106">По умолчанию эта операция не возвращает скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="da2bf-106">By default, this operation does not return hidden folders.</span></span> <span data-ttu-id="da2bf-107">Используйте параметр запроса _includeHiddenFolders,_ чтобы включить их в ответ.</span><span class="sxs-lookup"><span data-stu-id="da2bf-107">Use a query parameter _includeHiddenFolders_ to include them in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="da2bf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da2bf-108">Permissions</span></span>
<span data-ttu-id="da2bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da2bf-111">Permission type</span></span>      | <span data-ttu-id="da2bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da2bf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da2bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da2bf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da2bf-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da2bf-114">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da2bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da2bf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da2bf-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da2bf-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da2bf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="da2bf-117">Application</span></span> | <span data-ttu-id="da2bf-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da2bf-118">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da2bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da2bf-119">HTTP request</span></span>

<span data-ttu-id="da2bf-120">Чтобы получить все почтовые папки в почтовом ящике указанного пользователя, за исключением скрытых папок:</span><span class="sxs-lookup"><span data-stu-id="da2bf-120">To get all the mail folders in the specified user's mailbox, excluding those that are hidden:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```

<span data-ttu-id="da2bf-121">Чтобы включить _скрытые_ почтовые папки в ответ:</span><span class="sxs-lookup"><span data-stu-id="da2bf-121">To include _hidden_ mail folders in the response:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/?includeHiddenFolders=true
GET /users/{id | userPrincipalName}/mailFolders/?includeHiddenFolders=true
```

## <a name="query-parameters"></a><span data-ttu-id="da2bf-122">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="da2bf-122">Query parameters</span></span>
<span data-ttu-id="da2bf-123">Чтобы получить список всех объектов mailFolders, включая скрытые (их свойство **isHidden** имеет true), в URL-адресе запроса укажите параметр запроса как , как показано в разделе `includeHiddenFolders` `true` [HTTP-запроса.](#http-request)</span><span class="sxs-lookup"><span data-stu-id="da2bf-123">To return a list of all mailFolders including those that are hidden (their **isHidden** property is true), in the request URL, specify the `includeHiddenFolders` query parameter as `true`, as shown in the [HTTP request](#http-request) section.</span></span>

<span data-ttu-id="da2bf-124">Этот метод также поддерживает [параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da2bf-124">This method also supports [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da2bf-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da2bf-125">Request headers</span></span>
| <span data-ttu-id="da2bf-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da2bf-126">Header</span></span>       | <span data-ttu-id="da2bf-127">Значение</span><span class="sxs-lookup"><span data-stu-id="da2bf-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da2bf-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da2bf-128">Authorization</span></span>  | <span data-ttu-id="da2bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da2bf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da2bf-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da2bf-131">Request body</span></span>
<span data-ttu-id="da2bf-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da2bf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da2bf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2bf-133">Response</span></span>

<span data-ttu-id="da2bf-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da2bf-134">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="da2bf-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="da2bf-135">Examples</span></span>

### <a name="example-1-list-mail-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="da2bf-136">Пример 1. Список папок почты в почтовом ящике пользователя, выписав его</span><span class="sxs-lookup"><span data-stu-id="da2bf-136">Example 1: List mail folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="da2bf-137">В этом примере в **ответ включается объект mailSearchFolder.**</span><span class="sxs-lookup"><span data-stu-id="da2bf-137">This example includes a **mailSearchFolder** object in the response.</span></span> <span data-ttu-id="da2bf-138">Папка поиска почты — это папка под папкой "Входящие" с отображаемым именем "Еженедельные дайджесты".</span><span class="sxs-lookup"><span data-stu-id="da2bf-138">The mail search folder is a child folder under the Inbox with the display name "Weekly digests".</span></span>

#### <a name="request"></a><span data-ttu-id="da2bf-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="da2bf-139">Request</span></span>
<span data-ttu-id="da2bf-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da2bf-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da2bf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="da2bf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders
```
# <a name="c"></a>[<span data-ttu-id="da2bf-142">C#</span><span class="sxs-lookup"><span data-stu-id="da2bf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da2bf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da2bf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da2bf-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da2bf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da2bf-145">Java</span><span class="sxs-lookup"><span data-stu-id="da2bf-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="da2bf-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2bf-146">Response</span></span>
<span data-ttu-id="da2bf-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da2bf-147">Here is an example of the response.</span></span> 

><span data-ttu-id="da2bf-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da2bf-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
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


### <a name="example-2-include-hidden-folders-in-the-signed-in-users-mailbox"></a><span data-ttu-id="da2bf-149">Пример 2. Включив скрытые папки в почтовый ящик во включенного пользователя</span><span class="sxs-lookup"><span data-stu-id="da2bf-149">Example 2: Include hidden folders in the signed-in user's mailbox</span></span>

<span data-ttu-id="da2bf-150">В следующем примере параметр запроса используется для получения списка почтовых папок, `includeHiddenFolders` включая скрытые почтовые папки.</span><span class="sxs-lookup"><span data-stu-id="da2bf-150">The next example uses the `includeHiddenFolders` query parameter to get a list of mail folders including hidden mail folders.</span></span> <span data-ttu-id="da2bf-151">Ответ включает папку "Clutters", для нее **задав для isHidden** задав true.</span><span class="sxs-lookup"><span data-stu-id="da2bf-151">The response includes the "Clutters" folder that has the **isHidden** set to true.</span></span>

#### <a name="request"></a><span data-ttu-id="da2bf-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="da2bf-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="da2bf-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="da2bf-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_hiddenmailfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/?includeHiddenFolders=true
```
# <a name="c"></a>[<span data-ttu-id="da2bf-154">C#</span><span class="sxs-lookup"><span data-stu-id="da2bf-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-hiddenmailfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da2bf-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da2bf-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-hiddenmailfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da2bf-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da2bf-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-hiddenmailfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da2bf-157">Java</span><span class="sxs-lookup"><span data-stu-id="da2bf-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-hiddenmailfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da2bf-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="da2bf-158">Response</span></span>
<span data-ttu-id="da2bf-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da2bf-159">Here is an example of the response.</span></span>

><span data-ttu-id="da2bf-160">**Примечание.** Показанный здесь объект ответа сокращен для учитаемости и не включает все папки по умолчанию в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="da2bf-160">**Note:** The response object shown here is shortened for readability, and doesn't include all the default folders in a user mailbox.</span></span>
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
