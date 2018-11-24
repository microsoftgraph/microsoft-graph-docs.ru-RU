# <a name="list-calendars"></a><span data-ttu-id="aa389-101">Список календарей</span><span class="sxs-lookup"><span data-stu-id="aa389-101">List calendars</span></span>

<span data-ttu-id="aa389-102">Получение списка календарей из группы календарей.</span><span class="sxs-lookup"><span data-stu-id="aa389-102">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa389-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa389-103">Permissions</span></span>

<span data-ttu-id="aa389-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="aa389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="aa389-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa389-106">Permission type</span></span>                        | <span data-ttu-id="aa389-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa389-107">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="aa389-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa389-108">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa389-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa389-109">Calendars.Read</span></span>                              |
| <span data-ttu-id="aa389-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa389-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa389-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa389-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="aa389-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa389-112">Application</span></span>                            | <span data-ttu-id="aa389-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="aa389-113">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="aa389-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa389-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="aa389-115">Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa389-115">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="aa389-116">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa389-116">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa389-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa389-117">Optional query parameters</span></span>

<span data-ttu-id="aa389-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa389-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa389-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa389-119">Request headers</span></span>

| <span data-ttu-id="aa389-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aa389-120">Name</span></span>          | <span data-ttu-id="aa389-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aa389-121">Type</span></span>   | <span data-ttu-id="aa389-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aa389-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="aa389-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa389-123">Authorization</span></span> | <span data-ttu-id="aa389-124">string</span><span class="sxs-lookup"><span data-stu-id="aa389-124">string</span></span> | <span data-ttu-id="aa389-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa389-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa389-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa389-127">Request body</span></span>

<span data-ttu-id="aa389-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa389-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa389-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa389-129">Response</span></span>

<span data-ttu-id="aa389-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Calendar](../resources/calendar.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa389-130">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa389-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa389-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aa389-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa389-132">Request</span></span>

<span data-ttu-id="aa389-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa389-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="aa389-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa389-134">Response</span></span>

<span data-ttu-id="aa389-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="aa389-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
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
