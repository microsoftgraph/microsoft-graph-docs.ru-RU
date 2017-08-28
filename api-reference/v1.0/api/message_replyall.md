# <a name="message-replyall"></a><span data-ttu-id="8456c-101">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="8456c-101">message: replyAll</span></span>

<span data-ttu-id="8456c-p101">Ответ всем получателям сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="8456c-p101">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8456c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8456c-104">Permissions</span></span>
<span data-ttu-id="8456c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8456c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8456c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8456c-107">Permission type</span></span>      | <span data-ttu-id="8456c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8456c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8456c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8456c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="8456c-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8456c-110">Mail.Send</span></span>    |
|<span data-ttu-id="8456c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8456c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8456c-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8456c-112">Mail.Send</span></span>    |
|<span data-ttu-id="8456c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8456c-113">Application</span></span> | <span data-ttu-id="8456c-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="8456c-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="8456c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8456c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="8456c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8456c-116">Request headers</span></span>
| <span data-ttu-id="8456c-117">Имя</span><span class="sxs-lookup"><span data-stu-id="8456c-117">Name</span></span>       | <span data-ttu-id="8456c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8456c-118">Type</span></span> | <span data-ttu-id="8456c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8456c-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8456c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8456c-120">Authorization</span></span>  | <span data-ttu-id="8456c-121">string</span><span class="sxs-lookup"><span data-stu-id="8456c-121">string</span></span>  | <span data-ttu-id="8456c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8456c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8456c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8456c-124">Content-Type</span></span> | <span data-ttu-id="8456c-125">string</span><span class="sxs-lookup"><span data-stu-id="8456c-125">string</span></span>  | <span data-ttu-id="8456c-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8456c-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8456c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8456c-128">Request body</span></span>
<span data-ttu-id="8456c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8456c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8456c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="8456c-130">Parameter</span></span>    | <span data-ttu-id="8456c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8456c-131">Type</span></span>   |<span data-ttu-id="8456c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8456c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8456c-133">comment</span><span class="sxs-lookup"><span data-stu-id="8456c-133">comment</span></span>|<span data-ttu-id="8456c-134">String</span><span class="sxs-lookup"><span data-stu-id="8456c-134">String</span></span>|<span data-ttu-id="8456c-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="8456c-p105">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="8456c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8456c-137">Response</span></span>

<span data-ttu-id="8456c-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8456c-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8456c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="8456c-140">Example</span></span>
<span data-ttu-id="8456c-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8456c-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8456c-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8456c-142">Request</span></span>
<span data-ttu-id="8456c-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8456c-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="8456c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8456c-144">Response</span></span>
<span data-ttu-id="8456c-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8456c-145">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
