# <a name="create-message"></a><span data-ttu-id="239f0-101">Создание объекта Message</span><span class="sxs-lookup"><span data-stu-id="239f0-101">Create Message</span></span>

<span data-ttu-id="239f0-102">С помощью этого API можно создать экземпляр Message в mailfolder.</span><span class="sxs-lookup"><span data-stu-id="239f0-102">Use this API to create a new Message in a mailfolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="239f0-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="239f0-103">Permissions</span></span>
<span data-ttu-id="239f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="239f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="239f0-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="239f0-106">Permission type</span></span>      | <span data-ttu-id="239f0-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="239f0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="239f0-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="239f0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="239f0-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="239f0-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="239f0-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="239f0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="239f0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="239f0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="239f0-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="239f0-112">Application</span></span> | <span data-ttu-id="239f0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="239f0-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="239f0-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="239f0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/messages
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages
```
## <a name="request-headers"></a><span data-ttu-id="239f0-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="239f0-115">Request headers</span></span>
| <span data-ttu-id="239f0-116">Заголовок</span><span class="sxs-lookup"><span data-stu-id="239f0-116">Header</span></span>       | <span data-ttu-id="239f0-117">Значение</span><span class="sxs-lookup"><span data-stu-id="239f0-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="239f0-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="239f0-118">Authorization</span></span>  | <span data-ttu-id="239f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="239f0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="239f0-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="239f0-121">Content-Type</span></span>  | <span data-ttu-id="239f0-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="239f0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="239f0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="239f0-124">Request body</span></span>
<span data-ttu-id="239f0-125">Предоставьте в тексте запроса описание объекта [Message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="239f0-125">In the request body, supply a JSON representation of [Message](../resources/message.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="239f0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="239f0-126">Response</span></span>

<span data-ttu-id="239f0-127">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="239f0-127">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239f0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="239f0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="239f0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="239f0-129">Request</span></span>
<span data-ttu-id="239f0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="239f0-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_message_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/messages
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```
<span data-ttu-id="239f0-131">Предоставьте в тексте запроса описание объекта [message](../resources/message.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="239f0-131">In the request body, supply a JSON representation of [message](../resources/message.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="239f0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="239f0-132">Response</span></span>
<span data-ttu-id="239f0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="239f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
