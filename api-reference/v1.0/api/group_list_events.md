# <a name="list-events"></a><span data-ttu-id="6857b-101">Список событий</span><span class="sxs-lookup"><span data-stu-id="6857b-101">List events</span></span>

<span data-ttu-id="6857b-102">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="6857b-102">Retrieve a list of [event](../resources/event.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6857b-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6857b-103">Permissions</span></span>
<span data-ttu-id="6857b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6857b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6857b-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6857b-106">Permission type</span></span>      | <span data-ttu-id="6857b-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6857b-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6857b-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6857b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6857b-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6857b-109">Group.Read.All, Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="6857b-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6857b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6857b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6857b-111">Not supported.</span></span>    | 
|<span data-ttu-id="6857b-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6857b-112">Application</span></span> | <span data-ttu-id="6857b-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6857b-113">Group.Read.All, Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6857b-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6857b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6857b-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6857b-115">Optional query parameters</span></span>
<span data-ttu-id="6857b-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6857b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6857b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6857b-117">Request headers</span></span>
| <span data-ttu-id="6857b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6857b-118">Header</span></span>       | <span data-ttu-id="6857b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="6857b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6857b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6857b-120">Authorization</span></span>  | <span data-ttu-id="6857b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6857b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6857b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6857b-123">Request body</span></span>
<span data-ttu-id="6857b-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6857b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6857b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="6857b-125">Response</span></span>

<span data-ttu-id="6857b-126">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6857b-126">If successful, this method returns a `200 OK` response code and a collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6857b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6857b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6857b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6857b-128">Request</span></span>
<span data-ttu-id="6857b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6857b-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/events
```
##### <a name="response"></a><span data-ttu-id="6857b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6857b-130">Response</span></span>
<span data-ttu-id="6857b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6857b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
