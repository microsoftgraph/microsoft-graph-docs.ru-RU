# <a name="list-calendars"></a><span data-ttu-id="7829c-101">Список календарей</span><span class="sxs-lookup"><span data-stu-id="7829c-101">List calendars</span></span>

<span data-ttu-id="7829c-102">Получение всех календарей пользователя (свойство навигации `/calendars`), календарей из группы календарей по умолчанию или из указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="7829c-102">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="7829c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7829c-103">Permissions</span></span>
<span data-ttu-id="7829c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7829c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7829c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7829c-106">Permission type</span></span>      | <span data-ttu-id="7829c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7829c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7829c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7829c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7829c-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7829c-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7829c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7829c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7829c-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7829c-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="7829c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7829c-112">Application</span></span> | <span data-ttu-id="7829c-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7829c-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7829c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7829c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7829c-115">Все календари пользователя.</span><span class="sxs-lookup"><span data-stu-id="7829c-115">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="7829c-116">Календари пользователя в объекте [calendarGroup](../resources/calendarGroup.md) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7829c-116">The user's calendars in the default [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="7829c-117">Календари пользователя в указанном объекте [calendarGroup](../resources/calendarGroup.md).</span><span class="sxs-lookup"><span data-stu-id="7829c-117">The user's calendars in a specific [calendarGroup](../resources/calendarGroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7829c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7829c-118">Optional query parameters</span></span>
<span data-ttu-id="7829c-119">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7829c-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7829c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7829c-120">Request headers</span></span>
| <span data-ttu-id="7829c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7829c-121">Header</span></span>       | <span data-ttu-id="7829c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7829c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7829c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7829c-123">Authorization</span></span>  | <span data-ttu-id="7829c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7829c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7829c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7829c-126">Content-Type</span></span>   | <span data-ttu-id="7829c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7829c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7829c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7829c-128">Request body</span></span>
<span data-ttu-id="7829c-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7829c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7829c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7829c-130">Response</span></span>

<span data-ttu-id="7829c-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7829c-131">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7829c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7829c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7829c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7829c-133">Request</span></span>
<span data-ttu-id="7829c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7829c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="7829c-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7829c-135">Response</span></span>
<span data-ttu-id="7829c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7829c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
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
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->