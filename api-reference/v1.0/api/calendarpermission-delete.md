---
title: Удаление Календарпермиссион
description: Удаление Календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9dd829cf780af8d4720bae487296cd547c6852e9
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806619"
---
# <a name="delete-calendarpermission"></a><span data-ttu-id="78920-103">Удаление Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="78920-103">Delete calendarPermission</span></span>

<span data-ttu-id="78920-104">Удаление Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="78920-104">Delete calendarPermission.</span></span>

## <a name="permissions"></a><span data-ttu-id="78920-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="78920-105">Permissions</span></span>

<span data-ttu-id="78920-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78920-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="78920-108">Permission type</span></span>      | <span data-ttu-id="78920-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="78920-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78920-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="78920-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78920-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78920-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78920-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="78920-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78920-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78920-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="78920-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="78920-114">Application</span></span> | <span data-ttu-id="78920-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78920-115">Calendars.ReadWrite</span></span> |
## <a name="http-request"></a><span data-ttu-id="78920-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="78920-116">HTTP request</span></span>

<span data-ttu-id="78920-117">Удаление указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="78920-117">Delete the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="78920-118">Удаление указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="78920-118">Delete the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="78920-119">Удаление указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="78920-119">Delete the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="78920-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="78920-120">Request headers</span></span>

| <span data-ttu-id="78920-121">Имя</span><span class="sxs-lookup"><span data-stu-id="78920-121">Name</span></span>          | <span data-ttu-id="78920-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78920-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="78920-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="78920-123">Authorization</span></span> | <span data-ttu-id="78920-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="78920-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="78920-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="78920-125">Request body</span></span>

<span data-ttu-id="78920-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="78920-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78920-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="78920-127">Response</span></span>

<span data-ttu-id="78920-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="78920-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78920-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="78920-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78920-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="78920-131">Request</span></span>

<span data-ttu-id="78920-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="78920-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="78920-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="78920-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendarpermission"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="78920-134">C#</span><span class="sxs-lookup"><span data-stu-id="78920-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78920-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78920-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78920-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78920-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78920-137">Java</span><span class="sxs-lookup"><span data-stu-id="78920-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78920-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="78920-138">Response</span></span>

<span data-ttu-id="78920-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="78920-139">The following is an example of the response.</span></span>

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
