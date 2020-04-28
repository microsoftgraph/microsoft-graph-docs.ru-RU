---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 662efaae4fade948b88d716af664ce157705fef6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440915"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="1d979-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="1d979-103">Delete calendarPermission</span></span>

<span data-ttu-id="1d979-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d979-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d979-105">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="1d979-105">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d979-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d979-106">Permissions</span></span>

<span data-ttu-id="1d979-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d979-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d979-109">Permission type</span></span>      | <span data-ttu-id="1d979-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d979-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d979-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d979-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d979-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d979-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1d979-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d979-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d979-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d979-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1d979-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d979-115">Application</span></span> | <span data-ttu-id="1d979-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1d979-116">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="1d979-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d979-117">HTTP request</span></span>

<span data-ttu-id="1d979-118">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="1d979-118">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1d979-119">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="1d979-119">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="1d979-120">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="1d979-120">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1d979-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d979-121">Request headers</span></span>

| <span data-ttu-id="1d979-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1d979-122">Name</span></span>          | <span data-ttu-id="1d979-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d979-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1d979-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d979-124">Authorization</span></span> | <span data-ttu-id="1d979-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1d979-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d979-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d979-126">Request body</span></span>

<span data-ttu-id="1d979-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d979-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d979-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d979-128">Response</span></span>

<span data-ttu-id="1d979-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1d979-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d979-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="1d979-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d979-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d979-132">Request</span></span>

<span data-ttu-id="1d979-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d979-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1d979-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d979-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="1d979-135">C#</span><span class="sxs-lookup"><span data-stu-id="1d979-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d979-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d979-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d979-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d979-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d979-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d979-138">Response</span></span>

<span data-ttu-id="1d979-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1d979-139">The following is an example of the response.</span></span>

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
