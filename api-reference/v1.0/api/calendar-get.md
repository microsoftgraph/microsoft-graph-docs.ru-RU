---
title: Вывод календаря
description: 'Получение свойств и связей объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 999811a315572ca08ec27450dfa1b09bec91b4b2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726552"
---
# <a name="get-calendar"></a><span data-ttu-id="eb324-104">Вывод календаря</span><span class="sxs-lookup"><span data-stu-id="eb324-104">Get calendar</span></span>

<span data-ttu-id="eb324-105">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="eb324-105">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="eb324-106">Это может быть календарь для ресурса [user](../resources/user.md) или стандартный календарь для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="eb324-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="eb324-107">Существует два сценария, в которых приложение может получить календарь другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="eb324-107">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="eb324-108">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="eb324-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="eb324-109">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="eb324-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="eb324-110">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="eb324-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb324-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb324-111">Permissions</span></span>
<span data-ttu-id="eb324-112">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="eb324-112">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="eb324-113">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb324-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb324-114">Календарь</span><span class="sxs-lookup"><span data-stu-id="eb324-114">Calendar</span></span> | <span data-ttu-id="eb324-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb324-115">Delegated (work or school account)</span></span> | <span data-ttu-id="eb324-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb324-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb324-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="eb324-117">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="eb324-118">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="eb324-118">user calendar</span></span> | <span data-ttu-id="eb324-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb324-119">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="eb324-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb324-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="eb324-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb324-121">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="eb324-122">календарь группы</span><span class="sxs-lookup"><span data-stu-id="eb324-122">group calendar</span></span> | <span data-ttu-id="eb324-123">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb324-123">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="eb324-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb324-124">Not supported.</span></span> | <span data-ttu-id="eb324-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb324-125">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="eb324-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb324-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="eb324-127">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eb324-127">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="eb324-128">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="eb324-128">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="eb324-129">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="eb324-129">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eb324-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb324-130">Optional query parameters</span></span>
<span data-ttu-id="eb324-131">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eb324-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eb324-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb324-132">Request headers</span></span>
| <span data-ttu-id="eb324-133">Имя</span><span class="sxs-lookup"><span data-stu-id="eb324-133">Name</span></span>       | <span data-ttu-id="eb324-134">Тип</span><span class="sxs-lookup"><span data-stu-id="eb324-134">Type</span></span> | <span data-ttu-id="eb324-135">Описание</span><span class="sxs-lookup"><span data-stu-id="eb324-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eb324-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb324-136">Authorization</span></span>  | <span data-ttu-id="eb324-137">string</span><span class="sxs-lookup"><span data-stu-id="eb324-137">string</span></span>  | <span data-ttu-id="eb324-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb324-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb324-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb324-140">Request body</span></span>
<span data-ttu-id="eb324-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb324-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb324-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb324-142">Response</span></span>

<span data-ttu-id="eb324-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eb324-143">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eb324-144">Пример</span><span class="sxs-lookup"><span data-stu-id="eb324-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb324-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb324-145">Request</span></span>
<span data-ttu-id="eb324-146">В приведенном ниже примере описывается вывод календаря по умолчанию для пользователя, находящегося в системе. </span><span class="sxs-lookup"><span data-stu-id="eb324-146">The following example gets the signed-in user's default calendar.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eb324-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb324-147">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb324-148">C#</span><span class="sxs-lookup"><span data-stu-id="eb324-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb324-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb324-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb324-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb324-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="eb324-151">Java</span><span class="sxs-lookup"><span data-stu-id="eb324-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eb324-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb324-152">Response</span></span>
<span data-ttu-id="eb324-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb324-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
    "id": "AAMkAGI2TGuLAAA=",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
