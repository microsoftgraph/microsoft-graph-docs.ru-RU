# <a name="delete-event"></a><span data-ttu-id="90cf9-101">Удаление события</span><span class="sxs-lookup"><span data-stu-id="90cf9-101">Delete event</span></span>
<span data-ttu-id="90cf9-102">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="90cf9-102">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90cf9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90cf9-103">Permissions</span></span>
<span data-ttu-id="90cf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="90cf9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90cf9-106">Permission type</span></span>      | <span data-ttu-id="90cf9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90cf9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90cf9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90cf9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="90cf9-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90cf9-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90cf9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90cf9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90cf9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90cf9-111">Not supported.</span></span>    |
|<span data-ttu-id="90cf9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90cf9-112">Application</span></span> | <span data-ttu-id="90cf9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90cf9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90cf9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90cf9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90cf9-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90cf9-115">Request headers</span></span>
| <span data-ttu-id="90cf9-116">Имя</span><span class="sxs-lookup"><span data-stu-id="90cf9-116">Name</span></span>       | <span data-ttu-id="90cf9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="90cf9-117">Type</span></span> | <span data-ttu-id="90cf9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="90cf9-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="90cf9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="90cf9-119">Authorization</span></span>  | <span data-ttu-id="90cf9-120">string</span><span class="sxs-lookup"><span data-stu-id="90cf9-120">string</span></span>  | <span data-ttu-id="90cf9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90cf9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90cf9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90cf9-123">Request body</span></span>
<span data-ttu-id="90cf9-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90cf9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90cf9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="90cf9-125">Response</span></span>
<span data-ttu-id="90cf9-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="90cf9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90cf9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="90cf9-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="90cf9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="90cf9-129">Request</span></span>
<span data-ttu-id="90cf9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90cf9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="90cf9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="90cf9-131">Response</span></span>
<span data-ttu-id="90cf9-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90cf9-132">The following is an example of the response.</span></span> 
><span data-ttu-id="90cf9-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90cf9-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90cf9-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90cf9-134">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->