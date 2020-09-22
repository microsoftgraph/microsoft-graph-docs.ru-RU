---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3004f53cbe37c9f3891f350d1cb7946280ed859e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987514"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="486e8-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="486e8-103">Delete calendarPermission</span></span>

<span data-ttu-id="486e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="486e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="486e8-105">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="486e8-105">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="486e8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="486e8-106">Permissions</span></span>

<span data-ttu-id="486e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="486e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="486e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="486e8-109">Permission type</span></span>      | <span data-ttu-id="486e8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="486e8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="486e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="486e8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="486e8-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="486e8-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="486e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="486e8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="486e8-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="486e8-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="486e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="486e8-115">Application</span></span> | <span data-ttu-id="486e8-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="486e8-116">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="486e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="486e8-117">HTTP request</span></span>

<span data-ttu-id="486e8-118">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="486e8-118">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="486e8-119">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="486e8-119">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="486e8-120">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="486e8-120">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="486e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="486e8-121">Request headers</span></span>

| <span data-ttu-id="486e8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="486e8-122">Name</span></span>          | <span data-ttu-id="486e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="486e8-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="486e8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="486e8-124">Authorization</span></span> | <span data-ttu-id="486e8-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="486e8-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="486e8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="486e8-126">Request body</span></span>

<span data-ttu-id="486e8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="486e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="486e8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="486e8-128">Response</span></span>

<span data-ttu-id="486e8-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="486e8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="486e8-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="486e8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="486e8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="486e8-132">Request</span></span>

<span data-ttu-id="486e8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="486e8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="486e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="486e8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="486e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="486e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="486e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="486e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="486e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="486e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="486e8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="486e8-138">Response</span></span>

<span data-ttu-id="486e8-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="486e8-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


