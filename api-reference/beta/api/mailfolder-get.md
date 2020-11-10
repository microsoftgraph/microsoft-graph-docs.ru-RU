---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a18c39825ad13349f6efc8360fe3037ca0cc7dbe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979389"
---
# <a name="get-mailfolder"></a><span data-ttu-id="9fc11-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="9fc11-103">Get mailFolder</span></span>

<span data-ttu-id="9fc11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fc11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc11-105">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="9fc11-105">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="9fc11-106">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="9fc11-106">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="9fc11-107">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="9fc11-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9fc11-108">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="9fc11-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9fc11-109">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="9fc11-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="9fc11-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc11-110">Permissions</span></span>

<span data-ttu-id="9fc11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fc11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fc11-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fc11-113">Permission type</span></span>      | <span data-ttu-id="9fc11-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fc11-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fc11-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fc11-115">Delegated (work or school account)</span></span> | <span data-ttu-id="9fc11-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fc11-116">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9fc11-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fc11-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fc11-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fc11-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9fc11-119">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9fc11-119">Application</span></span> | <span data-ttu-id="9fc11-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9fc11-120">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fc11-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fc11-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9fc11-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9fc11-122">Optional query parameters</span></span>

<span data-ttu-id="9fc11-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9fc11-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9fc11-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fc11-124">Request headers</span></span>

| <span data-ttu-id="9fc11-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9fc11-125">Name</span></span>          | <span data-ttu-id="9fc11-126">Тип</span><span class="sxs-lookup"><span data-stu-id="9fc11-126">Type</span></span>   | <span data-ttu-id="9fc11-127">Описание</span><span class="sxs-lookup"><span data-stu-id="9fc11-127">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="9fc11-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fc11-128">Authorization</span></span> | <span data-ttu-id="9fc11-129">string</span><span class="sxs-lookup"><span data-stu-id="9fc11-129">string</span></span> | <span data-ttu-id="9fc11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fc11-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fc11-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9fc11-132">Request body</span></span>

<span data-ttu-id="9fc11-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9fc11-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fc11-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc11-134">Response</span></span>

<span data-ttu-id="9fc11-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc11-135">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fc11-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="9fc11-136">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="9fc11-137">Пример 1. Получение папки почты</span><span class="sxs-lookup"><span data-stu-id="9fc11-137">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="9fc11-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc11-138">Request</span></span>

<span data-ttu-id="9fc11-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc11-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9fc11-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc11-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```
# <a name="c"></a>[<span data-ttu-id="9fc11-141">C#</span><span class="sxs-lookup"><span data-stu-id="9fc11-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fc11-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fc11-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fc11-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fc11-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fc11-144">Java</span><span class="sxs-lookup"><span data-stu-id="9fc11-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="9fc11-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc11-145">Response</span></span>

<span data-ttu-id="9fc11-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc11-146">The following is an example of the response.</span></span>

> <span data-ttu-id="9fc11-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fc11-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="9fc11-149">Пример 2. Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="9fc11-149">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="9fc11-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fc11-150">Request</span></span>

<span data-ttu-id="9fc11-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fc11-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9fc11-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fc11-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```
# <a name="c"></a>[<span data-ttu-id="9fc11-153">C#</span><span class="sxs-lookup"><span data-stu-id="9fc11-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailsearchfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fc11-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fc11-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailsearchfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fc11-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fc11-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailsearchfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fc11-156">Java</span><span class="sxs-lookup"><span data-stu-id="9fc11-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailsearchfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fc11-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fc11-157">Response</span></span>

<span data-ttu-id="9fc11-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9fc11-158">The following is an example of the response.</span></span>

> <span data-ttu-id="9fc11-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fc11-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
