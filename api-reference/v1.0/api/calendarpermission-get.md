---
title: Получение Календарпермиссион
description: Получение свойств и связей объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ab5fefbb2b88511d6b40aaf80772f582975eec02
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070309"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="27e9f-103">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="27e9f-103">Get calendarPermission</span></span>

<span data-ttu-id="27e9f-104">Получение указанного объекта разрешений для календаря пользователя или группы, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="27e9f-104">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="27e9f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27e9f-105">Permissions</span></span>

<span data-ttu-id="27e9f-106">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="27e9f-106">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="27e9f-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27e9f-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27e9f-108">Календарь</span><span class="sxs-lookup"><span data-stu-id="27e9f-108">Calendar</span></span> | <span data-ttu-id="27e9f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27e9f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="27e9f-110">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27e9f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27e9f-111">Приложение</span><span class="sxs-lookup"><span data-stu-id="27e9f-111">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="27e9f-112">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="27e9f-112">user calendar</span></span> | <span data-ttu-id="27e9f-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27e9f-113">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="27e9f-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27e9f-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="27e9f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27e9f-115">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="27e9f-116">календарь группы</span><span class="sxs-lookup"><span data-stu-id="27e9f-116">group calendar</span></span> | <span data-ttu-id="27e9f-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27e9f-117">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="27e9f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27e9f-118">Not supported.</span></span> | <span data-ttu-id="27e9f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27e9f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27e9f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27e9f-120">HTTP request</span></span>

<span data-ttu-id="27e9f-121">Получение указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="27e9f-121">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="27e9f-122">Получение указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="27e9f-122">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="27e9f-123">Получение указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="27e9f-123">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27e9f-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27e9f-124">Optional query parameters</span></span>

<span data-ttu-id="27e9f-125">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="27e9f-125">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="27e9f-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="27e9f-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="27e9f-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27e9f-127">Request headers</span></span>

| <span data-ttu-id="27e9f-128">Имя</span><span class="sxs-lookup"><span data-stu-id="27e9f-128">Name</span></span>      |<span data-ttu-id="27e9f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="27e9f-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27e9f-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27e9f-130">Authorization</span></span> | <span data-ttu-id="27e9f-131">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="27e9f-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="27e9f-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27e9f-132">Request body</span></span>

<span data-ttu-id="27e9f-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27e9f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27e9f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="27e9f-134">Response</span></span>

<span data-ttu-id="27e9f-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27e9f-135">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27e9f-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="27e9f-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27e9f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="27e9f-137">Request</span></span>

<span data-ttu-id="27e9f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27e9f-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="27e9f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="27e9f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="27e9f-140">C#</span><span class="sxs-lookup"><span data-stu-id="27e9f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27e9f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27e9f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27e9f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27e9f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27e9f-143">Java</span><span class="sxs-lookup"><span data-stu-id="27e9f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarpermission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27e9f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="27e9f-144">Response</span></span>

<span data-ttu-id="27e9f-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27e9f-145">The following is an example of the response.</span></span>

> <span data-ttu-id="27e9f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27e9f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

