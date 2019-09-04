---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 521529be7cb515a7618f30203f3abf24534a5cfb
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726174"
---
# <a name="get-mailfolder"></a><span data-ttu-id="42426-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="42426-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42426-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="42426-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="42426-105">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="42426-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="42426-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="42426-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="42426-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="42426-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="42426-108">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="42426-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="42426-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42426-109">Permissions</span></span>

<span data-ttu-id="42426-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42426-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42426-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42426-112">Permission type</span></span>      | <span data-ttu-id="42426-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42426-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42426-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42426-114">Delegated (work or school account)</span></span> | <span data-ttu-id="42426-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42426-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42426-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42426-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42426-117">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42426-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="42426-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42426-118">Application</span></span> | <span data-ttu-id="42426-119">Mail. ReadBasic. ALL, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42426-119">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="42426-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42426-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42426-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="42426-121">Optional query parameters</span></span>

<span data-ttu-id="42426-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="42426-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42426-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42426-123">Request headers</span></span>

| <span data-ttu-id="42426-124">Имя</span><span class="sxs-lookup"><span data-stu-id="42426-124">Name</span></span>          | <span data-ttu-id="42426-125">Тип</span><span class="sxs-lookup"><span data-stu-id="42426-125">Type</span></span>   | <span data-ttu-id="42426-126">Описание</span><span class="sxs-lookup"><span data-stu-id="42426-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="42426-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="42426-127">Authorization</span></span> | <span data-ttu-id="42426-128">string</span><span class="sxs-lookup"><span data-stu-id="42426-128">string</span></span> | <span data-ttu-id="42426-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42426-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42426-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42426-131">Request body</span></span>

<span data-ttu-id="42426-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="42426-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42426-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="42426-133">Response</span></span>

<span data-ttu-id="42426-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="42426-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42426-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="42426-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="42426-136">Пример 1: получение почтовой папки</span><span class="sxs-lookup"><span data-stu-id="42426-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="42426-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="42426-137">Request</span></span>

<span data-ttu-id="42426-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42426-138">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="42426-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="42426-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42426-140">C#</span><span class="sxs-lookup"><span data-stu-id="42426-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42426-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42426-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42426-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="42426-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="42426-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="42426-143">Response</span></span>

<span data-ttu-id="42426-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42426-144">The following is an example of the response.</span></span>

> <span data-ttu-id="42426-145">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42426-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42426-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42426-146">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="42426-147">Пример 2: Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="42426-147">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="42426-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="42426-148">Request</span></span>

<span data-ttu-id="42426-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42426-149">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="42426-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="42426-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="42426-151">C#</span><span class="sxs-lookup"><span data-stu-id="42426-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="42426-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42426-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="42426-153">Цель — C</span><span class="sxs-lookup"><span data-stu-id="42426-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="42426-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="42426-154">Response</span></span>

<span data-ttu-id="42426-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="42426-155">The following is an example of the response.</span></span>

> <span data-ttu-id="42426-156">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42426-156">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="42426-157">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42426-157">All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
