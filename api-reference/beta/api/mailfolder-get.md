---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: baee4635954070b8e6f80b53fc1f0d489327328a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049284"
---
# <a name="get-mailfolder"></a><span data-ttu-id="ffa81-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="ffa81-103">Get mailFolder</span></span>

<span data-ttu-id="ffa81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffa81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffa81-105">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="ffa81-105">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="ffa81-106">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="ffa81-106">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="ffa81-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="ffa81-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ffa81-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="ffa81-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ffa81-109">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="ffa81-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffa81-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffa81-110">Permissions</span></span>

<span data-ttu-id="ffa81-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffa81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffa81-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffa81-113">Permission type</span></span>      | <span data-ttu-id="ffa81-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffa81-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffa81-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffa81-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ffa81-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffa81-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ffa81-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffa81-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffa81-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffa81-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ffa81-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="ffa81-119">Application</span></span> | <span data-ttu-id="ffa81-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ffa81-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffa81-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffa81-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffa81-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffa81-122">Optional query parameters</span></span>

<span data-ttu-id="ffa81-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffa81-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffa81-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffa81-124">Request headers</span></span>

| <span data-ttu-id="ffa81-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ffa81-125">Name</span></span>          | <span data-ttu-id="ffa81-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ffa81-126">Type</span></span>   | <span data-ttu-id="ffa81-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ffa81-127">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="ffa81-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffa81-128">Authorization</span></span> | <span data-ttu-id="ffa81-129">string</span><span class="sxs-lookup"><span data-stu-id="ffa81-129">string</span></span> | <span data-ttu-id="ffa81-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffa81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffa81-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffa81-132">Request body</span></span>

<span data-ttu-id="ffa81-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffa81-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffa81-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffa81-134">Response</span></span>

<span data-ttu-id="ffa81-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffa81-135">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffa81-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="ffa81-136">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="ffa81-137">Пример 1. Получение папки почты</span><span class="sxs-lookup"><span data-stu-id="ffa81-137">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="ffa81-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffa81-138">Request</span></span>

<span data-ttu-id="ffa81-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffa81-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ffa81-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffa81-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="c"></a>[<span data-ttu-id="ffa81-141">C#</span><span class="sxs-lookup"><span data-stu-id="ffa81-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffa81-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffa81-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffa81-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffa81-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffa81-144">Java</span><span class="sxs-lookup"><span data-stu-id="ffa81-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="ffa81-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffa81-145">Response</span></span>

<span data-ttu-id="ffa81-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ffa81-146">The following is an example of the response.</span></span>

> <span data-ttu-id="ffa81-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ffa81-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "wellKnownName": "inbox",
  "isHidden": false
}
```

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="ffa81-148">Пример 2. Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="ffa81-148">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="ffa81-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffa81-149">Request</span></span>

<span data-ttu-id="ffa81-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffa81-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ffa81-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffa81-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="c"></a>[<span data-ttu-id="ffa81-152">C#</span><span class="sxs-lookup"><span data-stu-id="ffa81-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffa81-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffa81-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffa81-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffa81-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffa81-155">Java</span><span class="sxs-lookup"><span data-stu-id="ffa81-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ffa81-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffa81-156">Response</span></span>

<span data-ttu-id="ffa81-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ffa81-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ffa81-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ffa81-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "isHidden": false,
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
