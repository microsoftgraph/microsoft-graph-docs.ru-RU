# <a name="get-conversation-thread"></a><span data-ttu-id="3936f-101">Получение цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="3936f-101">Get conversation thread</span></span>
<span data-ttu-id="3936f-102">Получение объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="3936f-102">Get a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3936f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3936f-103">Permissions</span></span>
<span data-ttu-id="3936f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3936f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3936f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3936f-106">Permission type</span></span>      | <span data-ttu-id="3936f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3936f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3936f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3936f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3936f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3936f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3936f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3936f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3936f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3936f-111">Not supported.</span></span>    |
|<span data-ttu-id="3936f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3936f-112">Application</span></span> | <span data-ttu-id="3936f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3936f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3936f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3936f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3936f-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3936f-115">Optional query parameters</span></span>
<span data-ttu-id="3936f-116">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3936f-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3936f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3936f-117">Request headers</span></span>
| <span data-ttu-id="3936f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3936f-118">Header</span></span>       | <span data-ttu-id="3936f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3936f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3936f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3936f-120">Authorization</span></span>  | <span data-ttu-id="3936f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3936f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3936f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3936f-123">Request body</span></span>
<span data-ttu-id="3936f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3936f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3936f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="3936f-125">Response</span></span>
<span data-ttu-id="3936f-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [thread](../resources/conversationthread.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3936f-126">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3936f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3936f-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3936f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3936f-128">Request</span></span>
<span data-ttu-id="3936f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3936f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_thread"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="3936f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3936f-130">Response</span></span>
<span data-ttu-id="3936f-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3936f-131">The following is an example of the response.</span></span>
><span data-ttu-id="3936f-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3936f-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3936f-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3936f-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 655

{
    "id": "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==",
    "topic": "New Training Plans",
    "hasAttachments": false,
    "lastDeliveredDateTime": "2017-07-31T18:59:05Z",
    "uniqueSenders": [
        "HR Taskforce"
    ],
    "preview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "isLocked": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
