---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1bd8a4f49d329cb4123f0ffcde142b2591c60132
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728743"
---
# <a name="get-mailfolder"></a><span data-ttu-id="bc181-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="bc181-103">Get mailFolder</span></span>

<span data-ttu-id="bc181-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="bc181-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="bc181-105">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="bc181-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="bc181-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="bc181-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bc181-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="bc181-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bc181-108">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="bc181-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bc181-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc181-109">Permissions</span></span>
<span data-ttu-id="bc181-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc181-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc181-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc181-112">Permission type</span></span>      | <span data-ttu-id="bc181-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc181-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc181-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc181-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bc181-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc181-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bc181-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc181-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc181-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc181-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bc181-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc181-118">Application</span></span> | <span data-ttu-id="bc181-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc181-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc181-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc181-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc181-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc181-121">Optional query parameters</span></span>
<span data-ttu-id="bc181-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc181-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc181-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc181-123">Request headers</span></span>
| <span data-ttu-id="bc181-124">Имя</span><span class="sxs-lookup"><span data-stu-id="bc181-124">Name</span></span>       | <span data-ttu-id="bc181-125">Тип</span><span class="sxs-lookup"><span data-stu-id="bc181-125">Type</span></span> | <span data-ttu-id="bc181-126">Описание</span><span class="sxs-lookup"><span data-stu-id="bc181-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc181-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc181-127">Authorization</span></span>  | <span data-ttu-id="bc181-128">string</span><span class="sxs-lookup"><span data-stu-id="bc181-128">string</span></span>  | <span data-ttu-id="bc181-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc181-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc181-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc181-131">Request body</span></span>
<span data-ttu-id="bc181-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc181-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc181-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc181-133">Response</span></span>

<span data-ttu-id="bc181-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bc181-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="bc181-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="bc181-135">Examples</span></span>
### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="bc181-136">Пример 1. Получение папки почты</span><span class="sxs-lookup"><span data-stu-id="bc181-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="bc181-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc181-137">Request</span></span>

<span data-ttu-id="bc181-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc181-138">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bc181-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc181-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc181-140">C#</span><span class="sxs-lookup"><span data-stu-id="bc181-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc181-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc181-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc181-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc181-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bc181-143">Java</span><span class="sxs-lookup"><span data-stu-id="bc181-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc181-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc181-144">Response</span></span>

<span data-ttu-id="bc181-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc181-145">The following is an example of the response.</span></span>

> <span data-ttu-id="bc181-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bc181-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc181-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc181-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60,
  "wellKnownName": "inbox"
}
```

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="bc181-148">Пример 2. Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="bc181-148">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="bc181-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc181-149">Request</span></span>

<span data-ttu-id="bc181-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc181-150">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bc181-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc181-151">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc181-152">C#</span><span class="sxs-lookup"><span data-stu-id="bc181-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc181-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc181-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc181-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc181-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bc181-155">Java</span><span class="sxs-lookup"><span data-stu-id="bc181-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc181-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc181-156">Response</span></span>

<span data-ttu-id="bc181-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc181-157">The following is an example of the response.</span></span>

> <span data-ttu-id="bc181-158">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bc181-158">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bc181-159">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc181-159">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
