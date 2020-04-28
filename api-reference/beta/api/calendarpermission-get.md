---
title: Получение Календарпермиссион
description: Получение свойств и связей объекта календарпермиссион.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8481cecf256d9cd85f9c444f0550ea7c43d37d0b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440901"
---
# <a name="get-calendarpermission"></a><span data-ttu-id="41fcb-103">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="41fcb-103">Get calendarPermission</span></span>

<span data-ttu-id="41fcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41fcb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41fcb-105">Получение указанного объекта разрешений для календаря пользователя или группы, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="41fcb-105">Get the specified permissions object of a user or group calendar that has been shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="41fcb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41fcb-106">Permissions</span></span>

<span data-ttu-id="41fcb-107">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="41fcb-107">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="41fcb-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41fcb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41fcb-109">Календарь</span><span class="sxs-lookup"><span data-stu-id="41fcb-109">Calendar</span></span> | <span data-ttu-id="41fcb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41fcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41fcb-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41fcb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41fcb-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="41fcb-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="41fcb-113">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="41fcb-113">user calendar</span></span> | <span data-ttu-id="41fcb-114">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fcb-114">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="41fcb-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fcb-115">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="41fcb-116">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41fcb-116">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="41fcb-117">календарь группы</span><span class="sxs-lookup"><span data-stu-id="41fcb-117">group calendar</span></span> | <span data-ttu-id="41fcb-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41fcb-118">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="41fcb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41fcb-119">Not supported.</span></span> | <span data-ttu-id="41fcb-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41fcb-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41fcb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41fcb-121">HTTP request</span></span>

<span data-ttu-id="41fcb-122">Получение указанных разрешений для основного календаря пользователя:</span><span class="sxs-lookup"><span data-stu-id="41fcb-122">Get the specified permissions of a user's primary calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="41fcb-123">Получение указанных разрешений для календаря группы:</span><span class="sxs-lookup"><span data-stu-id="41fcb-123">Get the specified permissions of a group calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/calendar/calendarPermissions/{id}
```

<span data-ttu-id="41fcb-124">Получение указанных разрешений для календаря пользователя, содержащего идентифицированное событие:</span><span class="sxs-lookup"><span data-stu-id="41fcb-124">Get the specified permissions of the user calendar that contains the identified event:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/calendar/calendarPermissions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41fcb-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="41fcb-125">Optional query parameters</span></span>

<span data-ttu-id="41fcb-126">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="41fcb-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="41fcb-127">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="41fcb-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="41fcb-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41fcb-128">Request headers</span></span>

| <span data-ttu-id="41fcb-129">Имя</span><span class="sxs-lookup"><span data-stu-id="41fcb-129">Name</span></span>      |<span data-ttu-id="41fcb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="41fcb-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41fcb-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41fcb-131">Authorization</span></span> | <span data-ttu-id="41fcb-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="41fcb-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="41fcb-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41fcb-133">Request body</span></span>

<span data-ttu-id="41fcb-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41fcb-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41fcb-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="41fcb-135">Response</span></span>

<span data-ttu-id="41fcb-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [календарпермиссион](../resources/calendarpermission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41fcb-136">If successful, this method returns a `200 OK` response code and the requested [calendarPermission](../resources/calendarpermission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41fcb-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="41fcb-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41fcb-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="41fcb-138">Request</span></span>

<span data-ttu-id="41fcb-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41fcb-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41fcb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="41fcb-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/calendar/calendarPermissions/{id}
```
# <a name="c"></a>[<span data-ttu-id="41fcb-141">C#</span><span class="sxs-lookup"><span data-stu-id="41fcb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarpermission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41fcb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41fcb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarpermission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41fcb-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41fcb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarpermission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41fcb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="41fcb-144">Response</span></span>

<span data-ttu-id="41fcb-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="41fcb-145">The following is an example of the response.</span></span>

> <span data-ttu-id="41fcb-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41fcb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
