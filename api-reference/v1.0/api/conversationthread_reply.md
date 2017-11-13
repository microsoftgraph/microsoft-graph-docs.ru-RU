# <a name="conversationthread-reply"></a><span data-ttu-id="68751-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="68751-101">conversationThread: reply</span></span>

<span data-ttu-id="68751-p101">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="68751-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="68751-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68751-104">Permissions</span></span>
<span data-ttu-id="68751-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68751-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68751-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68751-107">Permission type</span></span>      | <span data-ttu-id="68751-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68751-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68751-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68751-109">Delegated (work or school account)</span></span> | <span data-ttu-id="68751-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68751-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="68751-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68751-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68751-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68751-112">Not supported.</span></span>    |
|<span data-ttu-id="68751-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68751-113">Application</span></span> | <span data-ttu-id="68751-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68751-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68751-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68751-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="68751-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68751-116">Request headers</span></span>
| <span data-ttu-id="68751-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68751-117">Header</span></span>       | <span data-ttu-id="68751-118">Значение</span><span class="sxs-lookup"><span data-stu-id="68751-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68751-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68751-119">Authorization</span></span>  | <span data-ttu-id="68751-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68751-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68751-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68751-122">Content-Type</span></span>  | <span data-ttu-id="68751-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68751-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68751-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68751-125">Request body</span></span>
<span data-ttu-id="68751-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="68751-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="68751-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="68751-127">Parameter</span></span>    | <span data-ttu-id="68751-128">Тип</span><span class="sxs-lookup"><span data-stu-id="68751-128">Type</span></span>   |<span data-ttu-id="68751-129">Описание</span><span class="sxs-lookup"><span data-stu-id="68751-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68751-130">post</span><span class="sxs-lookup"><span data-stu-id="68751-130">post</span></span>|[<span data-ttu-id="68751-131">post</span><span class="sxs-lookup"><span data-stu-id="68751-131">post</span></span>](../resources/post.md)|<span data-ttu-id="68751-132">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="68751-132">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="68751-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="68751-133">Response</span></span>

<span data-ttu-id="68751-p105">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="68751-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68751-136">Пример</span><span class="sxs-lookup"><span data-stu-id="68751-136">Example</span></span>
<span data-ttu-id="68751-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="68751-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="68751-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="68751-138">Request</span></span>
<span data-ttu-id="68751-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68751-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="68751-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="68751-140">Response</span></span>
<span data-ttu-id="68751-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="68751-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
