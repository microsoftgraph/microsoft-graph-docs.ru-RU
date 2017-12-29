# <a name="create-event"></a><span data-ttu-id="63b11-101">Создание объекта event</span><span class="sxs-lookup"><span data-stu-id="63b11-101">Create Event</span></span>
<span data-ttu-id="63b11-102">С помощью этого API можно создать [событие](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="63b11-102">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="63b11-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63b11-103">Permissions</span></span>
<span data-ttu-id="63b11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63b11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63b11-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63b11-106">Permission type</span></span>      | <span data-ttu-id="63b11-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63b11-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63b11-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63b11-108">Delegated (work or school account)</span></span> | <span data-ttu-id="63b11-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63b11-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63b11-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63b11-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63b11-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63b11-111">Not supported.</span></span>    |
|<span data-ttu-id="63b11-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63b11-112">Application</span></span> | <span data-ttu-id="63b11-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63b11-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63b11-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63b11-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="63b11-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63b11-115">Request headers</span></span>
| <span data-ttu-id="63b11-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63b11-116">Header</span></span>       | <span data-ttu-id="63b11-117">Значение</span><span class="sxs-lookup"><span data-stu-id="63b11-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63b11-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63b11-118">Authorization</span></span>  | <span data-ttu-id="63b11-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63b11-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63b11-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63b11-121">Request body</span></span>
<span data-ttu-id="63b11-122">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63b11-122">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63b11-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b11-123">Response</span></span>
<span data-ttu-id="63b11-124">В случае успеха этот метод возвращает код ответа `201 Created` и объект [event](../resources/event.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="63b11-124">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63b11-125">Пример</span><span class="sxs-lookup"><span data-stu-id="63b11-125">Example</span></span>
#### <a name="request"></a><span data-ttu-id="63b11-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="63b11-126">Request</span></span>
<span data-ttu-id="63b11-127">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63b11-127">The following is an example of the request.</span></span>
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
<span data-ttu-id="63b11-128">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63b11-128">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="63b11-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b11-129">Response</span></span>
<span data-ttu-id="63b11-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63b11-130">The following is an example of the response.</span></span>
><span data-ttu-id="63b11-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63b11-131">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="63b11-132">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63b11-132">All the properties will be returned from an actual call.</span></span>

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
