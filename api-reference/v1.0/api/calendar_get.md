# <a name="get-calendar"></a><span data-ttu-id="47581-101">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="47581-101">Get calendar</span></span>

<span data-ttu-id="47581-102">Получение свойств и связей объекта календаря.</span><span class="sxs-lookup"><span data-stu-id="47581-102">Retrieve the properties and relationships of calendar object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47581-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47581-103">Permissions</span></span>
<span data-ttu-id="47581-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="47581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="47581-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47581-106">Permission type</span></span>      | <span data-ttu-id="47581-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47581-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="47581-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47581-108">Delegated (work or school account)</span></span> | <span data-ttu-id="47581-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47581-109">Calendars.Read</span></span>    | 
|<span data-ttu-id="47581-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47581-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47581-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47581-111">Calendars.Read</span></span>    | 
|<span data-ttu-id="47581-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47581-112">Application</span></span> | <span data-ttu-id="47581-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="47581-113">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47581-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47581-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="47581-115">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="47581-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar
GET /users/{id | userPrincipalName}/calendar
GET /groups/{id}/calendar
```
<span data-ttu-id="47581-116">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="47581-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}
GET /users/{id | userPrincipalName}/calendars/{id}

GET /me/calendarGroup/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}
```
<span data-ttu-id="47581-117">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="47581-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="47581-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47581-118">Optional query parameters</span></span>
<span data-ttu-id="47581-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47581-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="47581-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47581-120">Request headers</span></span>
| <span data-ttu-id="47581-121">Имя</span><span class="sxs-lookup"><span data-stu-id="47581-121">Name</span></span>       | <span data-ttu-id="47581-122">Тип</span><span class="sxs-lookup"><span data-stu-id="47581-122">Type</span></span> | <span data-ttu-id="47581-123">Описание</span><span class="sxs-lookup"><span data-stu-id="47581-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="47581-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="47581-124">Authorization</span></span>  | <span data-ttu-id="47581-125">string</span><span class="sxs-lookup"><span data-stu-id="47581-125">string</span></span>  | <span data-ttu-id="47581-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47581-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47581-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47581-128">Request body</span></span>
<span data-ttu-id="47581-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47581-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47581-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="47581-130">Response</span></span>

<span data-ttu-id="47581-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47581-131">If successful, this method returns a `200 OK` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47581-132">Пример</span><span class="sxs-lookup"><span data-stu-id="47581-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47581-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="47581-133">Request</span></span>
<span data-ttu-id="47581-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47581-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar
```
##### <a name="response"></a><span data-ttu-id="47581-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="47581-135">Response</span></span>
<span data-ttu-id="47581-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="47581-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "name":"Fanny Downs",
        "address":"fannyd@adatum.onmicrosoft.com"
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
