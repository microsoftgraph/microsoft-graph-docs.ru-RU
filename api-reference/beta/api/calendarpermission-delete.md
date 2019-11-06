---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e9d0483fd37f9b81b1808c1e2c33557fc2a17679
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994907"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="f02ca-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="f02ca-103">Delete calendarPermission</span></span>

<span data-ttu-id="f02ca-104">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="f02ca-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="f02ca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f02ca-105">Permissions</span></span>

<span data-ttu-id="f02ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f02ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f02ca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f02ca-108">Permission type</span></span>      | <span data-ttu-id="f02ca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f02ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f02ca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f02ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f02ca-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f02ca-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f02ca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f02ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f02ca-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f02ca-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f02ca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f02ca-114">Application</span></span> | <span data-ttu-id="f02ca-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f02ca-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="f02ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f02ca-116">HTTP request</span></span>

<span data-ttu-id="f02ca-117">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="f02ca-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="f02ca-118">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="f02ca-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="f02ca-119">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="f02ca-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f02ca-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f02ca-120">Request headers</span></span>

| <span data-ttu-id="f02ca-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f02ca-121">Name</span></span>          | <span data-ttu-id="f02ca-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f02ca-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f02ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f02ca-123">Authorization</span></span> | <span data-ttu-id="f02ca-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f02ca-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f02ca-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f02ca-125">Request body</span></span>

<span data-ttu-id="f02ca-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f02ca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f02ca-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f02ca-127">Response</span></span>

<span data-ttu-id="f02ca-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f02ca-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f02ca-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f02ca-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f02ca-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f02ca-131">Request</span></span>

<span data-ttu-id="f02ca-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f02ca-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f02ca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f02ca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f02ca-134">C#</span><span class="sxs-lookup"><span data-stu-id="f02ca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f02ca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f02ca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f02ca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f02ca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f02ca-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f02ca-137">Response</span></span>

<span data-ttu-id="f02ca-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f02ca-138">The following is an example of the response.</span></span>

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
