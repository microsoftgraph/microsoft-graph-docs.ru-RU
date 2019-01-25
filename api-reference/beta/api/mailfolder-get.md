---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: eee7adf677696fbf2dc969262604b817c7cddabe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529910"
---
# <a name="get-mailfolder"></a><span data-ttu-id="ca73c-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="ca73c-103">Get mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca73c-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="ca73c-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="ca73c-105">Существует два сценария, где приложение может получить почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca73c-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="ca73c-106">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="ca73c-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ca73c-107">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="ca73c-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ca73c-108">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="ca73c-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="ca73c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca73c-109">Permissions</span></span>
<span data-ttu-id="ca73c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca73c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca73c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca73c-112">Permission type</span></span>      | <span data-ttu-id="ca73c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca73c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca73c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca73c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ca73c-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca73c-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca73c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca73c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca73c-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca73c-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ca73c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca73c-118">Application</span></span> | <span data-ttu-id="ca73c-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca73c-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca73c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca73c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca73c-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca73c-121">Optional query parameters</span></span>
<span data-ttu-id="ca73c-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ca73c-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca73c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca73c-123">Request headers</span></span>
| <span data-ttu-id="ca73c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ca73c-124">Name</span></span>       | <span data-ttu-id="ca73c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ca73c-125">Type</span></span> | <span data-ttu-id="ca73c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ca73c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca73c-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca73c-127">Authorization</span></span>  | <span data-ttu-id="ca73c-128">string</span><span class="sxs-lookup"><span data-stu-id="ca73c-128">string</span></span>  | <span data-ttu-id="ca73c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca73c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca73c-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca73c-131">Request body</span></span>
<span data-ttu-id="ca73c-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca73c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca73c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca73c-133">Response</span></span>
<span data-ttu-id="ca73c-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca73c-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="ca73c-135">Пример 1</span><span class="sxs-lookup"><span data-stu-id="ca73c-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="ca73c-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="ca73c-136">Request 1</span></span>
<span data-ttu-id="ca73c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca73c-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="ca73c-138">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="ca73c-138">Response 1</span></span>
<span data-ttu-id="ca73c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca73c-139">The following is an example of the response.</span></span>
 ><span data-ttu-id="ca73c-140">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca73c-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ca73c-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca73c-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

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

## <a name="example-2"></a><span data-ttu-id="ca73c-142">Пример 2</span><span class="sxs-lookup"><span data-stu-id="ca73c-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="ca73c-143">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="ca73c-143">Request 2</span></span>
<span data-ttu-id="ca73c-144">Ниже приведен пример папки поиска запроса.</span><span class="sxs-lookup"><span data-stu-id="ca73c-144">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="ca73c-145">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="ca73c-145">Response 2</span></span>
<span data-ttu-id="ca73c-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ca73c-146">The following is an example of the response.</span></span>
 ><span data-ttu-id="ca73c-147">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca73c-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ca73c-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca73c-148">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

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
