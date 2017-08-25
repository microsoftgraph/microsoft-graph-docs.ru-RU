# <a name="message-reply"></a><span data-ttu-id="7b791-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="7b791-101">message: reply</span></span>

<span data-ttu-id="7b791-p101">Ответ отправителю сообщения. После этого сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="7b791-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b791-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b791-104">Permissions</span></span>
<span data-ttu-id="7b791-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b791-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7b791-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b791-107">Permission type</span></span>      | <span data-ttu-id="7b791-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b791-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="7b791-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b791-109">Delegated (work or school account)</span></span> | <span data-ttu-id="7b791-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7b791-110">Mail.Send</span></span>    | 
|<span data-ttu-id="7b791-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b791-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b791-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7b791-112">Mail.Send</span></span>    | 
|<span data-ttu-id="7b791-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b791-113">Application</span></span> | <span data-ttu-id="7b791-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7b791-114">Mail.Send</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7b791-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b791-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="7b791-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b791-116">Request headers</span></span>
| <span data-ttu-id="7b791-117">Имя</span><span class="sxs-lookup"><span data-stu-id="7b791-117">Name</span></span>       | <span data-ttu-id="7b791-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7b791-118">Type</span></span> | <span data-ttu-id="7b791-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7b791-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7b791-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b791-120">Authorization</span></span>  | <span data-ttu-id="7b791-121">string</span><span class="sxs-lookup"><span data-stu-id="7b791-121">string</span></span>  | <span data-ttu-id="7b791-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b791-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7b791-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b791-124">Content-Type</span></span> | <span data-ttu-id="7b791-125">string</span><span class="sxs-lookup"><span data-stu-id="7b791-125">string</span></span>  | <span data-ttu-id="7b791-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7b791-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b791-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b791-128">Request body</span></span>
<span data-ttu-id="7b791-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="7b791-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7b791-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="7b791-130">Parameter</span></span>    | <span data-ttu-id="7b791-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7b791-131">Type</span></span>   |<span data-ttu-id="7b791-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7b791-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b791-133">comment</span><span class="sxs-lookup"><span data-stu-id="7b791-133">comment</span></span>|<span data-ttu-id="7b791-134">String</span><span class="sxs-lookup"><span data-stu-id="7b791-134">String</span></span>|<span data-ttu-id="7b791-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="7b791-p105">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="7b791-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b791-137">Response</span></span>

<span data-ttu-id="7b791-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7b791-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b791-140">Пример</span><span class="sxs-lookup"><span data-stu-id="7b791-140">Example</span></span>
<span data-ttu-id="7b791-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="7b791-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7b791-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b791-142">Request</span></span>
<span data-ttu-id="7b791-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b791-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="7b791-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b791-144">Response</span></span>
##### <a name="response"></a><span data-ttu-id="7b791-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b791-145">Response</span></span>
<span data-ttu-id="7b791-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b791-146">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
