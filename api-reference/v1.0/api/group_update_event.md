# <a name="update-event"></a><span data-ttu-id="709db-101">Обновление события</span><span class="sxs-lookup"><span data-stu-id="709db-101">Update event</span></span>
<span data-ttu-id="709db-102">Обновление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="709db-102">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="709db-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="709db-103">Permissions</span></span>
<span data-ttu-id="709db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="709db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="709db-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="709db-106">Permission type</span></span>      | <span data-ttu-id="709db-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="709db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="709db-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="709db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="709db-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709db-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="709db-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="709db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="709db-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709db-111">Not supported.</span></span>    |
|<span data-ttu-id="709db-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="709db-112">Application</span></span> | <span data-ttu-id="709db-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="709db-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="709db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="709db-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="709db-115">Request headers</span></span>
| <span data-ttu-id="709db-116">Имя</span><span class="sxs-lookup"><span data-stu-id="709db-116">Name</span></span>       | <span data-ttu-id="709db-117">Тип</span><span class="sxs-lookup"><span data-stu-id="709db-117">Type</span></span> | <span data-ttu-id="709db-118">Описание</span><span class="sxs-lookup"><span data-stu-id="709db-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="709db-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="709db-119">Authorization</span></span>  | <span data-ttu-id="709db-120">string</span><span class="sxs-lookup"><span data-stu-id="709db-120">string</span></span>  | <span data-ttu-id="709db-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="709db-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="709db-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="709db-123">Request body</span></span>
<span data-ttu-id="709db-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="709db-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="709db-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="709db-127">Response</span></span>
<span data-ttu-id="709db-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="709db-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="709db-129">Пример</span><span class="sxs-lookup"><span data-stu-id="709db-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="709db-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="709db-130">Request</span></span>
<span data-ttu-id="709db-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="709db-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

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

#### <a name="response"></a><span data-ttu-id="709db-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="709db-132">Response</span></span>
<span data-ttu-id="709db-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="709db-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->