---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af2cc42c2ee72f1a57a1e0f9402209c107e259f4
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967300"
---
# <a name="get-mailfolder"></a><span data-ttu-id="0b2e9-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="0b2e9-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b2e9-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="0b2e9-105">Существует два сценария, где приложение может получить почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="0b2e9-106">если у приложения есть разрешения для приложений;</span><span class="sxs-lookup"><span data-stu-id="0b2e9-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0b2e9-107">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0b2e9-108">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="0b2e9-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b2e9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b2e9-109">Permissions</span></span>

<span data-ttu-id="0b2e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b2e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b2e9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b2e9-112">Permission type</span></span>      | <span data-ttu-id="0b2e9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b2e9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b2e9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b2e9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0b2e9-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b2e9-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0b2e9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b2e9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b2e9-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b2e9-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0b2e9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b2e9-118">Application</span></span> | <span data-ttu-id="0b2e9-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b2e9-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b2e9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b2e9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b2e9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b2e9-121">Optional query parameters</span></span>

<span data-ttu-id="0b2e9-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b2e9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b2e9-123">Request headers</span></span>

| <span data-ttu-id="0b2e9-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0b2e9-124">Name</span></span>          | <span data-ttu-id="0b2e9-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0b2e9-125">Type</span></span>   | <span data-ttu-id="0b2e9-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0b2e9-126">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="0b2e9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b2e9-127">Authorization</span></span> | <span data-ttu-id="0b2e9-128">string</span><span class="sxs-lookup"><span data-stu-id="0b2e9-128">string</span></span> | <span data-ttu-id="0b2e9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b2e9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b2e9-131">Request body</span></span>

<span data-ttu-id="0b2e9-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b2e9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b2e9-133">Response</span></span>

<span data-ttu-id="0b2e9-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b2e9-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b2e9-135">Examples</span></span>

### <a name="example-1-get-a-mail-folder"></a><span data-ttu-id="0b2e9-136">В примере 1: Получение папки почты</span><span class="sxs-lookup"><span data-stu-id="0b2e9-136">Example 1: Get a mail folder</span></span>

#### <a name="request"></a><span data-ttu-id="0b2e9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b2e9-137">Request</span></span>

<span data-ttu-id="0b2e9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="0b2e9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b2e9-139">Response</span></span>

<span data-ttu-id="0b2e9-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2e9-141">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b2e9-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-142">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-mail-search-folder"></a><span data-ttu-id="0b2e9-143">Пример 2: Получение папки поиска почты</span><span class="sxs-lookup"><span data-stu-id="0b2e9-143">Example 2: Get a mail search folder</span></span>

#### <a name="request"></a><span data-ttu-id="0b2e9-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b2e9-144">Request</span></span>

<span data-ttu-id="0b2e9-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a><span data-ttu-id="0b2e9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b2e9-146">Response</span></span>

<span data-ttu-id="0b2e9-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-147">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2e9-148">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0b2e9-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b2e9-149">All the properties will be returned from an actual call.</span></span>

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
  "sourceFolderIDs": [
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
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
