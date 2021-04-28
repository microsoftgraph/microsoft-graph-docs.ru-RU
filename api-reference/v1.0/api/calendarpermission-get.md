---
title: Get calendarPermission
description: Получите свойства и связи объекта calendarpermission.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4bfbf5fa07b0eb3ad61ceeb60572f229ba872617
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051622"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="3a0de-103">Get calendarPermission</span><span class="sxs-lookup"><span data-stu-id="3a0de-103">Get calendarPermission</span></span>

<span data-ttu-id="3a0de-104">Получите указанный объект разрешений пользователя или группового календаря, который был общим.</span><span class="sxs-lookup"><span data-stu-id="3a0de-104">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a0de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a0de-105">Permissions</span></span>

<span data-ttu-id="3a0de-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="3a0de-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="3a0de-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a0de-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a0de-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="3a0de-108">Calendar</span></span> | <span data-ttu-id="3a0de-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a0de-109">Delegated (work or school account)</span></span> | <span data-ttu-id="3a0de-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a0de-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a0de-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a0de-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="3a0de-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="3a0de-112">user calendar</span></span> | <span data-ttu-id="3a0de-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a0de-113">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="3a0de-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a0de-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="3a0de-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a0de-115">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="3a0de-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="3a0de-116">group calendar</span></span> | <span data-ttu-id="3a0de-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a0de-117">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="3a0de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a0de-118">Not supported.</span></span> | <span data-ttu-id="3a0de-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a0de-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a0de-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a0de-120">HTTP request</span></span>

<span data-ttu-id="3a0de-121">Получите указанные разрешения основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="3a0de-121">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="3a0de-122">Получите указанные разрешения группового календаря:</span><span class="sxs-lookup"><span data-stu-id="3a0de-122">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="3a0de-123">Получите указанные разрешения пользовательского календаря, который содержит указанное событие:</span><span class="sxs-lookup"><span data-stu-id="3a0de-123">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a0de-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a0de-124">Optional query parameters</span></span>

<span data-ttu-id="3a0de-125">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3a0de-125">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3a0de-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3a0de-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a0de-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a0de-127">Request headers</span></span>

| <span data-ttu-id="3a0de-128">Имя</span><span class="sxs-lookup"><span data-stu-id="3a0de-128">Name</span></span>      |<span data-ttu-id="3a0de-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3a0de-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a0de-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a0de-130">Authorization</span></span> | <span data-ttu-id="3a0de-131">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3a0de-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a0de-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a0de-132">Request body</span></span>

<span data-ttu-id="3a0de-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a0de-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a0de-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a0de-134">Response</span></span>

<span data-ttu-id="3a0de-135">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [calendarPermission](../resources/calendarpermission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3a0de-135">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a0de-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a0de-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a0de-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a0de-137">Request</span></span>

<span data-ttu-id="3a0de-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a0de-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a0de-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a0de-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="3a0de-140">C#</span><span class="sxs-lookup"><span data-stu-id="3a0de-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a0de-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a0de-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a0de-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a0de-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a0de-143">Java</span><span class="sxs-lookup"><span data-stu-id="3a0de-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3a0de-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a0de-144">Response</span></span>

<span data-ttu-id="3a0de-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a0de-145">The following is an example of the response.</span></span>

> <span data-ttu-id="3a0de-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a0de-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

