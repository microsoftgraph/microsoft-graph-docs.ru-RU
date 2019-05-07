---
title: Вывод календаря
description: 'Получение свойств и связей объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: dbdad8b4ff5bc639fd19ffa4e85e0e1c9ba257be
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635899"
---
# <a name="get-calendar"></a><span data-ttu-id="794da-104">Вывод календаря</span><span class="sxs-lookup"><span data-stu-id="794da-104">Get calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="794da-105">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="794da-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="794da-106">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="794da-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="794da-107">Существует два сценария, в которых приложение может получить календарь другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="794da-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="794da-108">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="794da-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="794da-109">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="794da-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="794da-110">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="794da-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="794da-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="794da-111">Permissions</span></span>
<span data-ttu-id="794da-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="794da-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794da-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="794da-114">Permission type</span></span>      | <span data-ttu-id="794da-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="794da-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="794da-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="794da-116">Delegated (work or school account)</span></span> | <span data-ttu-id="794da-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="794da-117">Calendars.Read</span></span>    |
|<span data-ttu-id="794da-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="794da-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="794da-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="794da-119">Calendars.Read</span></span>    |
|<span data-ttu-id="794da-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="794da-120">Application</span></span> | <span data-ttu-id="794da-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="794da-121">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="794da-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="794da-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="794da-123">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="794da-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="794da-124">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="794da-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="794da-125">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="794da-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="794da-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="794da-126">Optional query parameters</span></span>
<span data-ttu-id="794da-127">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="794da-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="794da-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="794da-128">Request headers</span></span>
| <span data-ttu-id="794da-129">Имя</span><span class="sxs-lookup"><span data-stu-id="794da-129">Name</span></span>       | <span data-ttu-id="794da-130">Тип</span><span class="sxs-lookup"><span data-stu-id="794da-130">Type</span></span> | <span data-ttu-id="794da-131">Описание</span><span class="sxs-lookup"><span data-stu-id="794da-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="794da-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="794da-132">Authorization</span></span>  | <span data-ttu-id="794da-133">string</span><span class="sxs-lookup"><span data-stu-id="794da-133">string</span></span>  | <span data-ttu-id="794da-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="794da-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="794da-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="794da-136">Request body</span></span>
<span data-ttu-id="794da-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="794da-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="794da-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="794da-138">Response</span></span>

<span data-ttu-id="794da-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="794da-139">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="794da-140">Пример</span><span class="sxs-lookup"><span data-stu-id="794da-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="794da-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="794da-141">Request</span></span>
<span data-ttu-id="794da-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="794da-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar
```

##### <a name="response"></a><span data-ttu-id="794da-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="794da-143">Response</span></span>
<span data-ttu-id="794da-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="794da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="794da-147">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="794da-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="794da-148">Языках</span><span class="sxs-lookup"><span data-stu-id="794da-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_calendar-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="794da-149">Язык</span><span class="sxs-lookup"><span data-stu-id="794da-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_calendar-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/calendar-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
