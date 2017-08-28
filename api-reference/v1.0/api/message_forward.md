# <a name="message-forward"></a><span data-ttu-id="69bb8-101">message: forward</span><span class="sxs-lookup"><span data-stu-id="69bb8-101">message: forward</span></span>

<span data-ttu-id="69bb8-p101">Пересылка сообщения. Сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="69bb8-p101">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="69bb8-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69bb8-104">Permissions</span></span>
<span data-ttu-id="69bb8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="69bb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="69bb8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69bb8-107">Permission type</span></span>      | <span data-ttu-id="69bb8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69bb8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69bb8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69bb8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="69bb8-110">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="69bb8-110">Mail.Send</span></span>    |
|<span data-ttu-id="69bb8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69bb8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69bb8-112">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="69bb8-112">Mail.Send</span></span>    |
|<span data-ttu-id="69bb8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69bb8-113">Application</span></span> | <span data-ttu-id="69bb8-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="69bb8-114">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="69bb8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69bb8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="69bb8-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69bb8-116">Request headers</span></span>
| <span data-ttu-id="69bb8-117">Имя</span><span class="sxs-lookup"><span data-stu-id="69bb8-117">Name</span></span>       | <span data-ttu-id="69bb8-118">Тип</span><span class="sxs-lookup"><span data-stu-id="69bb8-118">Type</span></span> | <span data-ttu-id="69bb8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="69bb8-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69bb8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="69bb8-120">Authorization</span></span>  | <span data-ttu-id="69bb8-121">string</span><span class="sxs-lookup"><span data-stu-id="69bb8-121">string</span></span>  | <span data-ttu-id="69bb8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69bb8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69bb8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69bb8-124">Content-Type</span></span> | <span data-ttu-id="69bb8-125">string</span><span class="sxs-lookup"><span data-stu-id="69bb8-125">string</span></span>  | <span data-ttu-id="69bb8-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69bb8-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69bb8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69bb8-128">Request body</span></span>
<span data-ttu-id="69bb8-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="69bb8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69bb8-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="69bb8-130">Parameter</span></span>    | <span data-ttu-id="69bb8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="69bb8-131">Type</span></span>   |<span data-ttu-id="69bb8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="69bb8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69bb8-133">comment</span><span class="sxs-lookup"><span data-stu-id="69bb8-133">comment</span></span>|<span data-ttu-id="69bb8-134">String</span><span class="sxs-lookup"><span data-stu-id="69bb8-134">String</span></span>|<span data-ttu-id="69bb8-p105">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="69bb8-p105">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="69bb8-137">toRecipients</span><span class="sxs-lookup"><span data-stu-id="69bb8-137">toRecipients</span></span>|<span data-ttu-id="69bb8-138">Коллекция объектов [Recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="69bb8-138">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="69bb8-139">Список получателей.</span><span class="sxs-lookup"><span data-stu-id="69bb8-139">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="69bb8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="69bb8-140">Response</span></span>

<span data-ttu-id="69bb8-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="69bb8-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69bb8-143">Пример</span><span class="sxs-lookup"><span data-stu-id="69bb8-143">Example</span></span>
<span data-ttu-id="69bb8-144">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="69bb8-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="69bb8-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="69bb8-145">Request</span></span>
<span data-ttu-id="69bb8-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69bb8-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="69bb8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="69bb8-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="69bb8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="69bb8-148">Response</span></span>
<span data-ttu-id="69bb8-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69bb8-149">Here is an example of the response.</span></span>
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
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
