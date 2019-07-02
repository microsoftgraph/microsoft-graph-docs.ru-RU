---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33932d16ac51f385a66adfd6fd8010069b650bf2
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417740"
---
# <a name="get-mailfolder"></a><span data-ttu-id="29f9c-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="29f9c-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f9c-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="29f9c-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="29f9c-105">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="29f9c-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="29f9c-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="29f9c-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="29f9c-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="29f9c-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="29f9c-108">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="29f9c-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="29f9c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29f9c-109">Permissions</span></span>

<span data-ttu-id="29f9c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29f9c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29f9c-112">Permission type</span></span>      | <span data-ttu-id="29f9c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29f9c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29f9c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29f9c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="29f9c-115">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29f9c-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="29f9c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29f9c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29f9c-117">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29f9c-117">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="29f9c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29f9c-118">Application</span></span> | <span data-ttu-id="29f9c-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29f9c-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="29f9c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29f9c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="29f9c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29f9c-121">Optional query parameters</span></span>

<span data-ttu-id="29f9c-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="29f9c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29f9c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29f9c-123">Request headers</span></span>

| <span data-ttu-id="29f9c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="29f9c-124">Name</span></span>          | <span data-ttu-id="29f9c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="29f9c-125">Type</span></span>   | <span data-ttu-id="29f9c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="29f9c-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="29f9c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="29f9c-127">Authorization</span></span> | <span data-ttu-id="29f9c-128">string</span><span class="sxs-lookup"><span data-stu-id="29f9c-128">string</span></span> | <span data-ttu-id="29f9c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29f9c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29f9c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29f9c-131">Request body</span></span>

<span data-ttu-id="29f9c-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29f9c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29f9c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="29f9c-133">Response</span></span>

<span data-ttu-id="29f9c-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29f9c-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29f9c-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="29f9c-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="29f9c-136">Пример 1: получение почтовой папки</span><span class="sxs-lookup"><span data-stu-id="29f9c-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="29f9c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="29f9c-137">Request</span></span>

<span data-ttu-id="29f9c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29f9c-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="29f9c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="29f9c-139">Response</span></span>

<span data-ttu-id="29f9c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29f9c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="29f9c-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29f9c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29f9c-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29f9c-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29f9c-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="29f9c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29f9c-144">C#</span><span class="sxs-lookup"><span data-stu-id="29f9c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29f9c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="29f9c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="29f9c-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="29f9c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="29f9c-147">Пример 2: Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="29f9c-147">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="29f9c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="29f9c-148">Request</span></span>

<span data-ttu-id="29f9c-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29f9c-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="29f9c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="29f9c-150">Response</span></span>

<span data-ttu-id="29f9c-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29f9c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="29f9c-152">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29f9c-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29f9c-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29f9c-153">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29f9c-154">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="29f9c-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29f9c-155">C#</span><span class="sxs-lookup"><span data-stu-id="29f9c-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29f9c-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="29f9c-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="29f9c-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="29f9c-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
