# <a name="get-calendar"></a><span data-ttu-id="99342-101">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="99342-101">Get calendar</span></span>

<span data-ttu-id="99342-102">Получение свойств и связей объекта [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="99342-102">Get the properties and relationships of a [calendar](../resources/calendar.md) object.</span></span> <span data-ttu-id="99342-103">Это может быть календарь для ресурса [user](../resources/user.md) или календарь по умолчанию для ресурса [group](../resources/group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="99342-103">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span>

<span data-ttu-id="99342-104">Существует два сценария, в которых программа может получить календарь другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="99342-104">There are two scenarios where an app can get another user's calendar:</span></span>

* <span data-ttu-id="99342-105">Если программа имеет разрешения для приложения, или</span><span class="sxs-lookup"><span data-stu-id="99342-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="99342-106">Если у программы есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился календарем с этим пользователем или предоставил этому пользователю делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="99342-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="99342-107">См. [подробности и пример](../../../concepts/outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="99342-107">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="99342-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99342-108">Permissions</span></span>
<span data-ttu-id="99342-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="99342-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="99342-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99342-111">Permission type</span></span>      | <span data-ttu-id="99342-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99342-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99342-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99342-113">Delegated (work or school account)</span></span> | <span data-ttu-id="99342-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99342-114">Calendars.Read</span></span>    |
|<span data-ttu-id="99342-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99342-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99342-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99342-116">Calendars.Read</span></span>    |
|<span data-ttu-id="99342-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99342-117">Application</span></span> | <span data-ttu-id="99342-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="99342-118">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="99342-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99342-119">HTTP request</span></span>
<span data-ttu-id="99342-120"><!-- { "blockType": "ignored" } --> [Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99342-120">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="99342-121">[Календарь](../resources/calendar.md) пользователя в группе по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="99342-121">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="99342-122">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="99342-122">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99342-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99342-123">Optional query parameters</span></span>
<span data-ttu-id="99342-124">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="99342-124">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="99342-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99342-125">Request headers</span></span>
| <span data-ttu-id="99342-126">Имя</span><span class="sxs-lookup"><span data-stu-id="99342-126">Name</span></span>       | <span data-ttu-id="99342-127">Тип</span><span class="sxs-lookup"><span data-stu-id="99342-127">Type</span></span> | <span data-ttu-id="99342-128">Описание</span><span class="sxs-lookup"><span data-stu-id="99342-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99342-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99342-129">Authorization</span></span>  | <span data-ttu-id="99342-130">строка</span><span class="sxs-lookup"><span data-stu-id="99342-130">string</span></span>  | <span data-ttu-id="99342-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99342-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99342-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99342-133">Request body</span></span>
<span data-ttu-id="99342-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99342-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99342-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="99342-135">Response</span></span>

<span data-ttu-id="99342-136">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99342-136">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99342-137">Пример</span><span class="sxs-lookup"><span data-stu-id="99342-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99342-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="99342-138">Request</span></span>
<span data-ttu-id="99342-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99342-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="99342-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="99342-140">Response</span></span>
<span data-ttu-id="99342-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99342-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
