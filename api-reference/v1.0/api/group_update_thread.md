# <a name="update-conversation-thread"></a><span data-ttu-id="b4445-101">Обновление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="b4445-101">Update conversation thread</span></span>
<span data-ttu-id="b4445-102">Обновление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="b4445-102">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4445-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4445-103">Permissions</span></span>
<span data-ttu-id="b4445-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4445-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4445-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4445-106">Permission type</span></span>      | <span data-ttu-id="b4445-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4445-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4445-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4445-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b4445-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4445-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4445-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4445-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4445-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4445-111">Not supported.</span></span>    |
|<span data-ttu-id="b4445-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4445-112">Application</span></span> | <span data-ttu-id="b4445-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4445-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4445-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4445-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4445-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4445-115">Request headers</span></span>
| <span data-ttu-id="b4445-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b4445-116">Name</span></span>       | <span data-ttu-id="b4445-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b4445-117">Type</span></span> | <span data-ttu-id="b4445-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b4445-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4445-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4445-119">Authorization</span></span>  | <span data-ttu-id="b4445-120">строка</span><span class="sxs-lookup"><span data-stu-id="b4445-120">string</span></span>  | <span data-ttu-id="b4445-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4445-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4445-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4445-123">Request body</span></span>
<span data-ttu-id="b4445-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b4445-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="b4445-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4445-127">Response</span></span>
<span data-ttu-id="b4445-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4445-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4445-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b4445-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b4445-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4445-130">Request</span></span>
<span data-ttu-id="b4445-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4445-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="b4445-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4445-132">Response</span></span>
<span data-ttu-id="b4445-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4445-133">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->