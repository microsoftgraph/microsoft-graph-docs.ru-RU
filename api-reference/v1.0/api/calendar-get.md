---
title: Вывод календаря
description: 'Получение свойств и связей объекта calendar. Это может быть календарь для ресурса user '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7af1c3679ab9c6d4d75e8618acf17d653619b869
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434904"
---
# <a name="get-calendar"></a><span data-ttu-id="d3b21-104">Вывод календаря</span><span class="sxs-lookup"><span data-stu-id="d3b21-104">Get calendar</span></span>

<span data-ttu-id="d3b21-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b21-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3b21-106">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="d3b21-106">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="d3b21-107">Это может быть календарь для [пользователя](../resources/user.md) или стандартный календарь для [группы](../resources/group.md) Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d3b21-107">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="d3b21-108">Существует два сценария, в которых приложение может получить календарь другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="d3b21-108">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="d3b21-109">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="d3b21-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="d3b21-110">если у приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним календарем или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="d3b21-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="d3b21-111">См. [подробные сведения и пример](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="d3b21-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

## <a name="permissions"></a><span data-ttu-id="d3b21-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3b21-112">Permissions</span></span>
<span data-ttu-id="d3b21-113">В зависимости от типа календаря, к которому относится событие, а также от требуемого типа разрешений (делегированные или разрешения приложений), для вызова этого API необходимо одно из указанных ниже разрешений.</span><span class="sxs-lookup"><span data-stu-id="d3b21-113">Depending on the type of calendar that the event is in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="d3b21-114">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3b21-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3b21-115">Календарь</span><span class="sxs-lookup"><span data-stu-id="d3b21-115">Calendar</span></span> | <span data-ttu-id="d3b21-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3b21-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d3b21-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3b21-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3b21-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3b21-118">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="d3b21-119">календарь пользователя</span><span class="sxs-lookup"><span data-stu-id="d3b21-119">user calendar</span></span> | <span data-ttu-id="d3b21-120">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3b21-120">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d3b21-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3b21-121">Calendars.Read, Calendars.ReadWrite</span></span> | <span data-ttu-id="d3b21-122">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3b21-122">Calendars.Read, Calendars.ReadWrite</span></span> |
| <span data-ttu-id="d3b21-123">календарь группы</span><span class="sxs-lookup"><span data-stu-id="d3b21-123">group calendar</span></span> | <span data-ttu-id="d3b21-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3b21-124">Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="d3b21-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3b21-125">Not supported.</span></span> | <span data-ttu-id="d3b21-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3b21-126">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d3b21-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3b21-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d3b21-128">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d3b21-128">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="d3b21-129">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d3b21-129">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}
```
<span data-ttu-id="d3b21-130">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="d3b21-130">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3b21-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3b21-131">Optional query parameters</span></span>
<span data-ttu-id="d3b21-132">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3b21-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d3b21-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3b21-133">Request headers</span></span>
| <span data-ttu-id="d3b21-134">Имя</span><span class="sxs-lookup"><span data-stu-id="d3b21-134">Name</span></span>       | <span data-ttu-id="d3b21-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d3b21-135">Type</span></span> | <span data-ttu-id="d3b21-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d3b21-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d3b21-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3b21-137">Authorization</span></span>  | <span data-ttu-id="d3b21-138">string</span><span class="sxs-lookup"><span data-stu-id="d3b21-138">string</span></span>  | <span data-ttu-id="d3b21-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3b21-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3b21-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3b21-141">Request body</span></span>
<span data-ttu-id="d3b21-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3b21-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3b21-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3b21-143">Response</span></span>

<span data-ttu-id="d3b21-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3b21-144">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3b21-145">Пример</span><span class="sxs-lookup"><span data-stu-id="d3b21-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3b21-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3b21-146">Request</span></span>
<span data-ttu-id="d3b21-147">В приведенном ниже примере описывается вывод календаря по умолчанию для пользователя, находящегося в системе. </span><span class="sxs-lookup"><span data-stu-id="d3b21-147">The following example gets the signed-in user's default calendar.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3b21-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3b21-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="d3b21-149">C#</span><span class="sxs-lookup"><span data-stu-id="d3b21-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3b21-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3b21-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3b21-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3b21-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3b21-152">Java</span><span class="sxs-lookup"><span data-stu-id="d3b21-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d3b21-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3b21-153">Response</span></span>
<span data-ttu-id="d3b21-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3b21-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "isDefaultCalendar": false,
    "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
