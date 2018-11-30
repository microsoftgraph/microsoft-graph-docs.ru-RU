---
title: Получение календаря
description: 'Получение свойств и связей объекта calendar. Календарь может иметь одно для пользователя '
ms.openlocfilehash: b4dd218e25d154fa1641a7a62d3b79790a15f7da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074776"
---
# <a name="get-calendar"></a><span data-ttu-id="2958f-104">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="2958f-104">Get calendar</span></span>

> <span data-ttu-id="2958f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2958f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2958f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2958f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2958f-107">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2958f-107">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="2958f-108">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="2958f-108">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="2958f-109">Существует два сценария, где приложения можно получить календаря другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2958f-109">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="2958f-110">Если приложение имеет разрешения приложения, или,</span><span class="sxs-lookup"><span data-stu-id="2958f-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="2958f-111">Если приложение имеет соответствующей делегированных [разрешений](#permissions) от одного пользователя и другой пользователь общий календарь с этим пользователем или, получает делегированный доступ для пользователя, который.</span><span class="sxs-lookup"><span data-stu-id="2958f-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="2958f-112">В разделе [сведения и примеры](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="2958f-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="2958f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2958f-113">Permissions</span></span>
<span data-ttu-id="2958f-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2958f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2958f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2958f-116">Permission type</span></span>      | <span data-ttu-id="2958f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2958f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2958f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2958f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2958f-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2958f-119">Calendars.Read</span></span>    |
|<span data-ttu-id="2958f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2958f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2958f-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2958f-121">Calendars.Read</span></span>    |
|<span data-ttu-id="2958f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2958f-122">Application</span></span> | <span data-ttu-id="2958f-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2958f-123">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="2958f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2958f-124">HTTP request</span></span>
<span data-ttu-id="2958f-125"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2958f-125"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="2958f-126">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2958f-126">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="2958f-127">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="2958f-127">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2958f-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2958f-128">Optional query parameters</span></span>
<span data-ttu-id="2958f-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2958f-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2958f-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2958f-130">Request headers</span></span>
| <span data-ttu-id="2958f-131">Имя</span><span class="sxs-lookup"><span data-stu-id="2958f-131">Name</span></span>       | <span data-ttu-id="2958f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2958f-132">Type</span></span> | <span data-ttu-id="2958f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2958f-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2958f-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="2958f-134">Authorization</span></span>  | <span data-ttu-id="2958f-135">string</span><span class="sxs-lookup"><span data-stu-id="2958f-135">string</span></span>  | <span data-ttu-id="2958f-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2958f-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2958f-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2958f-138">Request body</span></span>
<span data-ttu-id="2958f-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2958f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2958f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2958f-140">Response</span></span>

<span data-ttu-id="2958f-141">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2958f-141">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2958f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="2958f-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2958f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="2958f-143">Request</span></span>
<span data-ttu-id="2958f-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2958f-144">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="2958f-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="2958f-145">Response</span></span>
<span data-ttu-id="2958f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2958f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
