# <a name="post-forward"></a><span data-ttu-id="5d90c-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="5d90c-101">post: forward</span></span>

<span data-ttu-id="5d90c-p101">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="5d90c-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5d90c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d90c-104">Permissions</span></span>
<span data-ttu-id="5d90c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d90c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5d90c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d90c-107">Permission type</span></span>      | <span data-ttu-id="5d90c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d90c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d90c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d90c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5d90c-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d90c-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5d90c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d90c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d90c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d90c-112">Not supported.</span></span>    |
|<span data-ttu-id="5d90c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d90c-113">Application</span></span> | <span data-ttu-id="5d90c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d90c-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d90c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d90c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="5d90c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d90c-116">Request headers</span></span>
| <span data-ttu-id="5d90c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d90c-117">Header</span></span>       | <span data-ttu-id="5d90c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5d90c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5d90c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d90c-119">Authorization</span></span>  | <span data-ttu-id="5d90c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d90c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5d90c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d90c-122">Request body</span></span>
<span data-ttu-id="5d90c-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5d90c-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d90c-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="5d90c-124">Parameter</span></span>    | <span data-ttu-id="5d90c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5d90c-125">Type</span></span>   |<span data-ttu-id="5d90c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5d90c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d90c-127">comment</span><span class="sxs-lookup"><span data-stu-id="5d90c-127">comment</span></span>|<span data-ttu-id="5d90c-128">String</span><span class="sxs-lookup"><span data-stu-id="5d90c-128">String</span></span>|<span data-ttu-id="5d90c-129">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="5d90c-129">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="5d90c-130">toRecipients</span><span class="sxs-lookup"><span data-stu-id="5d90c-130">toRecipients</span></span>|<span data-ttu-id="5d90c-131">Коллекция объектов [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="5d90c-131">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="5d90c-132">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="5d90c-132">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="5d90c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d90c-133">Response</span></span>

<span data-ttu-id="5d90c-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5d90c-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d90c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="5d90c-136">Example</span></span>
<span data-ttu-id="5d90c-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5d90c-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5d90c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d90c-138">Request</span></span>
<span data-ttu-id="5d90c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d90c-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="5d90c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d90c-140">Response</span></span>
<span data-ttu-id="5d90c-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5d90c-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
