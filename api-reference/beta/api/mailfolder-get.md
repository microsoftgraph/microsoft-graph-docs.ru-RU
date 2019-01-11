---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8301f5ff1cef7602b3e9d488c67daec8ac277cce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856653"
---
# <a name="get-mailfolder"></a><span data-ttu-id="b7c05-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="b7c05-103">Get mailFolder</span></span>

> <span data-ttu-id="b7c05-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7c05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7c05-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7c05-106">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="b7c05-106">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="b7c05-107">Существует два сценария, где приложение может получить почтовой папки другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7c05-107">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="b7c05-108">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="b7c05-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b7c05-109">Если приложение имеет соответствующий делегированных [разрешений](#permissions) от одного пользователя и другой пользователь доступ к папке почты с этим пользователем или, предоставленное делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="b7c05-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b7c05-110">В разделе [сведения и примеры](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="b7c05-110">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b7c05-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c05-111">Permissions</span></span>
<span data-ttu-id="b7c05-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c05-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c05-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c05-114">Permission type</span></span>      | <span data-ttu-id="b7c05-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7c05-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c05-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7c05-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b7c05-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c05-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7c05-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7c05-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7c05-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c05-119">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b7c05-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7c05-120">Application</span></span> | <span data-ttu-id="b7c05-121">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c05-121">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7c05-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7c05-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7c05-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7c05-123">Optional query parameters</span></span>
<span data-ttu-id="b7c05-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c05-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7c05-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7c05-125">Request headers</span></span>
| <span data-ttu-id="b7c05-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b7c05-126">Name</span></span>       | <span data-ttu-id="b7c05-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b7c05-127">Type</span></span> | <span data-ttu-id="b7c05-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c05-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b7c05-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c05-129">Authorization</span></span>  | <span data-ttu-id="b7c05-130">string</span><span class="sxs-lookup"><span data-stu-id="b7c05-130">string</span></span>  | <span data-ttu-id="b7c05-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7c05-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7c05-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7c05-133">Request body</span></span>
<span data-ttu-id="b7c05-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7c05-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c05-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c05-135">Response</span></span>
<span data-ttu-id="b7c05-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7c05-136">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="b7c05-137">Пример 1</span><span class="sxs-lookup"><span data-stu-id="b7c05-137">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="b7c05-138">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="b7c05-138">Request 1</span></span>
<span data-ttu-id="b7c05-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c05-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-1"></a><span data-ttu-id="b7c05-140">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="b7c05-140">Response 1</span></span>
<span data-ttu-id="b7c05-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c05-141">The following is an example of the response.</span></span>
 ><span data-ttu-id="b7c05-142">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="b7c05-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7c05-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7c05-143">All the properties will be returned from an actual call.</span></span>
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

## <a name="example-2"></a><span data-ttu-id="b7c05-144">Пример 2</span><span class="sxs-lookup"><span data-stu-id="b7c05-144">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="b7c05-145">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="b7c05-145">Request 2</span></span>
<span data-ttu-id="b7c05-146">Ниже приведен пример папки поиска запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c05-146">The following is a search folder example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailSearchfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

#### <a name="response-2"></a><span data-ttu-id="b7c05-147">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="b7c05-147">Response 2</span></span>
<span data-ttu-id="b7c05-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c05-148">The following is an example of the response.</span></span>
 ><span data-ttu-id="b7c05-149">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="b7c05-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7c05-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7c05-150">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
