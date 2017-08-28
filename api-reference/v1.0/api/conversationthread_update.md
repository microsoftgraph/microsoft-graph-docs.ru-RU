# <a name="update-conversationthread"></a><span data-ttu-id="0fdb7-101">Обновление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="0fdb7-101">Update conversationthread</span></span>

<span data-ttu-id="0fdb7-102">Блокировка и разблокировка, позволяющие разрешить или предотвратить дальнейшую публикацию записей в цепочке.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fdb7-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fdb7-103">Permissions</span></span>
<span data-ttu-id="0fdb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fdb7-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fdb7-106">Permission type</span></span>      | <span data-ttu-id="0fdb7-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fdb7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fdb7-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fdb7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0fdb7-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fdb7-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0fdb7-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fdb7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fdb7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-111">Not supported.</span></span>    |
|<span data-ttu-id="0fdb7-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fdb7-112">Application</span></span> | <span data-ttu-id="0fdb7-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fdb7-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fdb7-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fdb7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0fdb7-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fdb7-115">Request headers</span></span>
| <span data-ttu-id="0fdb7-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fdb7-116">Header</span></span>       | <span data-ttu-id="0fdb7-117">Значение</span><span class="sxs-lookup"><span data-stu-id="0fdb7-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fdb7-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fdb7-118">Authorization</span></span>  | <span data-ttu-id="0fdb7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0fdb7-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fdb7-121">Content-Type</span></span>  | <span data-ttu-id="0fdb7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fdb7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fdb7-124">Request body</span></span>
<span data-ttu-id="0fdb7-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0fdb7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fdb7-128">Property</span></span>     | <span data-ttu-id="0fdb7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0fdb7-129">Type</span></span>   |<span data-ttu-id="0fdb7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0fdb7-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fdb7-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="0fdb7-131">isLocked</span></span>|<span data-ttu-id="0fdb7-132">Логическое</span><span class="sxs-lookup"><span data-stu-id="0fdb7-132">Boolean</span></span>|<span data-ttu-id="0fdb7-p105">Указывает, заблокирована ли цепочка. Чтобы запретить добавление сообщений, задайте значение `true`.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="0fdb7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fdb7-135">Response</span></span>

<span data-ttu-id="0fdb7-136">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0fdb7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="0fdb7-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fdb7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fdb7-138">Request</span></span>
<span data-ttu-id="0fdb7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="0fdb7-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="0fdb7-140">Response</span></span>
<span data-ttu-id="0fdb7-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0fdb7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
