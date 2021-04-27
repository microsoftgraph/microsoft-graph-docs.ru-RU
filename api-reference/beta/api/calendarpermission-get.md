---
title: Get calendarPermission
description: Получите свойства и связи объекта calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e6286ec91e3ef75cf9ae5d35992a8794392d2ede
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047688"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="b9f1f-103">Get calendarPermission</span><span class="sxs-lookup"><span data-stu-id="b9f1f-103">Get calendarPermission</span></span>

<span data-ttu-id="b9f1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f1f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9f1f-105">Получите указанный объект разрешений пользователя или группового календаря, который был общим.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-105">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f1f-106">Permissions</span></span>

<span data-ttu-id="b9f1f-107">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b9f1f-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f1f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9f1f-109">Календарь</span><span class="sxs-lookup"><span data-stu-id="b9f1f-109">Calendar</span></span> | <span data-ttu-id="b9f1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f1f-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f1f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f1f-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9f1f-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b9f1f-113">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="b9f1f-113">user calendar</span></span> | <span data-ttu-id="b9f1f-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f1f-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b9f1f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f1f-115">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b9f1f-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9f1f-116">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b9f1f-117">календарь группы</span><span class="sxs-lookup"><span data-stu-id="b9f1f-117">group calendar</span></span> | <span data-ttu-id="b9f1f-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f1f-118">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b9f1f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-119">Not supported.</span></span> | <span data-ttu-id="b9f1f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f1f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f1f-121">HTTP request</span></span>

<span data-ttu-id="b9f1f-122">Получите указанные разрешения основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="b9f1f-122">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b9f1f-123">Получите указанные разрешения группового календаря:</span><span class="sxs-lookup"><span data-stu-id="b9f1f-123">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="b9f1f-124">Получите указанные разрешения пользовательского календаря, который содержит указанное событие:</span><span class="sxs-lookup"><span data-stu-id="b9f1f-124">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f1f-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9f1f-125">Optional query parameters</span></span>

<span data-ttu-id="b9f1f-126">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b9f1f-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b9f1f-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f1f-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f1f-128">Request headers</span></span>

| <span data-ttu-id="b9f1f-129">Имя</span><span class="sxs-lookup"><span data-stu-id="b9f1f-129">Name</span></span>      |<span data-ttu-id="b9f1f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f1f-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9f1f-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9f1f-131">Authorization</span></span> | <span data-ttu-id="b9f1f-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b9f1f-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9f1f-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9f1f-133">Request body</span></span>

<span data-ttu-id="b9f1f-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f1f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f1f-135">Response</span></span>

<span data-ttu-id="b9f1f-136">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [calendarPermission](../resources/calendarpermission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-136">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9f1f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9f1f-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9f1f-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f1f-138">Request</span></span>

<span data-ttu-id="b9f1f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9f1f-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f1f-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="b9f1f-141">C#</span><span class="sxs-lookup"><span data-stu-id="b9f1f-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9f1f-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9f1f-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9f1f-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9f1f-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9f1f-144">Java</span><span class="sxs-lookup"><span data-stu-id="b9f1f-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9f1f-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f1f-145">Response</span></span>

<span data-ttu-id="b9f1f-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-146">The following is an example of the response.</span></span>

> <span data-ttu-id="b9f1f-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9f1f-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "emailAddress": {
    "name": "My Organization",
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "write",
  "allowedRoles": [
    "none",
    "freeBusyRead",
    "limitedRead",
    "read",
    "write"
  ],
  "id": "RGVmYXVsdA=="
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarPermission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


