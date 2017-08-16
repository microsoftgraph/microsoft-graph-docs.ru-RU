# <a name="create-event"></a><span data-ttu-id="69a0e-101">Создание объекта Event</span><span class="sxs-lookup"><span data-stu-id="69a0e-101">Create Event</span></span>

<span data-ttu-id="69a0e-102">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="69a0e-102">Use this API to create a new [event](../resources/event.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69a0e-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="69a0e-103">Prerequisites</span></span>
<span data-ttu-id="69a0e-104">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="69a0e-104">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="69a0e-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69a0e-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```
## <a name="request-headers"></a><span data-ttu-id="69a0e-106">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69a0e-106">Request headers</span></span>
| <span data-ttu-id="69a0e-107">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69a0e-107">Header</span></span>       | <span data-ttu-id="69a0e-108">Значение</span><span class="sxs-lookup"><span data-stu-id="69a0e-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69a0e-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69a0e-109">Authorization</span></span>  | <span data-ttu-id="69a0e-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69a0e-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69a0e-112">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69a0e-112">Request body</span></span>
<span data-ttu-id="69a0e-113">Предоставьте в тексте запроса описание объекта [Event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69a0e-113">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="69a0e-114">Отклик</span><span class="sxs-lookup"><span data-stu-id="69a0e-114">Response</span></span>

<span data-ttu-id="69a0e-115">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Event](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69a0e-115">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69a0e-116">Пример</span><span class="sxs-lookup"><span data-stu-id="69a0e-116">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69a0e-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="69a0e-117">Request</span></span>
<span data-ttu-id="69a0e-118">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69a0e-118">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/events
Content-type: application/json
Content-length: 285

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
```
<span data-ttu-id="69a0e-119">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69a0e-119">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="69a0e-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="69a0e-120">Response</span></span>
<span data-ttu-id="69a0e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="69a0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
