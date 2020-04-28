---
title: Вывод календаря
description: 'Получение свойств и связей объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6d1573ca89abf845f49a9ca817c4d82b2aa80090
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376098"
---
# <a name="get-calendar"></a><span data-ttu-id="b0733-104">Вывод календаря</span><span class="sxs-lookup"><span data-stu-id="b0733-104">Get calendar</span></span>

<span data-ttu-id="b0733-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0733-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0733-106">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="b0733-106">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="b0733-107">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="b0733-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="b0733-108">Существует два сценария, в которых приложение может получить календарь другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="b0733-108">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="b0733-109">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="b0733-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b0733-110">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="b0733-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b0733-111">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="b0733-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


## <a name="permissions"></a><span data-ttu-id="b0733-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0733-112">Permissions</span></span>
<span data-ttu-id="b0733-113">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="b0733-113">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="b0733-114">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0733-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0733-115">Календарь</span><span class="sxs-lookup"><span data-stu-id="b0733-115">Calendar</span></span> | <span data-ttu-id="b0733-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0733-116">Delegated (work or school account)</span></span> | <span data-ttu-id="b0733-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0733-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0733-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b0733-118">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="b0733-119">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="b0733-119">user calendar</span></span> | <span data-ttu-id="b0733-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0733-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b0733-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0733-121">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="b0733-122">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0733-122">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="b0733-123">календарь группы</span><span class="sxs-lookup"><span data-stu-id="b0733-123">group calendar</span></span> | <span data-ttu-id="b0733-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0733-124">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="b0733-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0733-125">Not supported.</span></span> | <span data-ttu-id="b0733-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0733-126">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b0733-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0733-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="b0733-128">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0733-128">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="b0733-129">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b0733-129">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="b0733-130">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b0733-130">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0733-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0733-131">Optional query parameters</span></span>
<span data-ttu-id="b0733-132">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0733-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0733-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0733-133">Request headers</span></span>
| <span data-ttu-id="b0733-134">Имя</span><span class="sxs-lookup"><span data-stu-id="b0733-134">Name</span></span>       | <span data-ttu-id="b0733-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b0733-135">Type</span></span> | <span data-ttu-id="b0733-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b0733-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b0733-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0733-137">Authorization</span></span>  | <span data-ttu-id="b0733-138">string</span><span class="sxs-lookup"><span data-stu-id="b0733-138">string</span></span>  | <span data-ttu-id="b0733-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0733-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0733-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0733-141">Request body</span></span>
<span data-ttu-id="b0733-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0733-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0733-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0733-143">Response</span></span>

<span data-ttu-id="b0733-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0733-144">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0733-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b0733-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0733-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0733-146">Request</span></span>
<span data-ttu-id="b0733-147">В приведенном ниже примере описывается вывод календаря по умолчанию для пользователя, находящегося в системе. </span><span class="sxs-lookup"><span data-stu-id="b0733-147">The following example gets the signed-in user's default calendar.</span></span>


# <a name="http"></a>[<span data-ttu-id="b0733-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0733-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="b0733-149">C#</span><span class="sxs-lookup"><span data-stu-id="b0733-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0733-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0733-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0733-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0733-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0733-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0733-152">Response</span></span>
<span data-ttu-id="b0733-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0733-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "calendarGroupId":null,
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "allowedOnlineMeetingProviders": [
                "teamsForBusiness"
            ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
    }
}

```

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
  ]
}
-->
