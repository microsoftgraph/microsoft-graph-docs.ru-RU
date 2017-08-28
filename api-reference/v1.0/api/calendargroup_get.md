# <a name="get-calendargroup"></a><span data-ttu-id="acbbb-101">Получение объекта calendarGroup</span><span class="sxs-lookup"><span data-stu-id="acbbb-101">Get calendarGroup</span></span>

<span data-ttu-id="acbbb-102">Получение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="acbbb-102">Retrieve the properties and relationships of a calendar group object.</span></span>
## <a name="permissions"></a><span data-ttu-id="acbbb-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acbbb-103">Permissions</span></span>
<span data-ttu-id="acbbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="acbbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="acbbb-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acbbb-106">Permission type</span></span>      | <span data-ttu-id="acbbb-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acbbb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acbbb-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acbbb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="acbbb-109">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="acbbb-109">Calendars.Read</span></span>    |
|<span data-ttu-id="acbbb-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acbbb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acbbb-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="acbbb-111">Calendars.Read</span></span>    |
|<span data-ttu-id="acbbb-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acbbb-112">Application</span></span> | <span data-ttu-id="acbbb-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="acbbb-113">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="acbbb-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acbbb-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="acbbb-115">Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="acbbb-115">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>
```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="acbbb-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="acbbb-116">Optional query parameters</span></span>
<span data-ttu-id="acbbb-117">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="acbbb-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="acbbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acbbb-118">Request headers</span></span>
| <span data-ttu-id="acbbb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="acbbb-119">Name</span></span>       | <span data-ttu-id="acbbb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="acbbb-120">Type</span></span> | <span data-ttu-id="acbbb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="acbbb-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="acbbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acbbb-122">Authorization</span></span>  | <span data-ttu-id="acbbb-123">string</span><span class="sxs-lookup"><span data-stu-id="acbbb-123">string</span></span>  | <span data-ttu-id="acbbb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acbbb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acbbb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acbbb-126">Request body</span></span>
<span data-ttu-id="acbbb-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acbbb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acbbb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="acbbb-128">Response</span></span>

<span data-ttu-id="acbbb-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [calendarGroup](../resources/calendargroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="acbbb-129">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acbbb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="acbbb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acbbb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="acbbb-131">Request</span></span>
<span data-ttu-id="acbbb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acbbb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="acbbb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="acbbb-133">Response</span></span>
<span data-ttu-id="acbbb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="acbbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
