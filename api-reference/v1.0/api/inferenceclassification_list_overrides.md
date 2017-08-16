# <a name="list-overrides"></a><span data-ttu-id="38128-101">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="38128-101">List overrides</span></span>

<span data-ttu-id="38128-102">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="38128-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="38128-p101">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="38128-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38128-105">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38128-105">Prerequisites</span></span>
<span data-ttu-id="38128-106">Для применения этого API требуются указанные **области**: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="38128-106">The following **scopes** are required to execute this API: *Mail.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="38128-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38128-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="38128-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38128-108">Request headers</span></span>
| <span data-ttu-id="38128-109">Имя</span><span class="sxs-lookup"><span data-stu-id="38128-109">Name</span></span>       | <span data-ttu-id="38128-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38128-110">Type</span></span> | <span data-ttu-id="38128-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38128-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="38128-112">Authorization</span><span class="sxs-lookup"><span data-stu-id="38128-112">Authorization</span></span>  | <span data-ttu-id="38128-113">string</span><span class="sxs-lookup"><span data-stu-id="38128-113">string</span></span>  | <span data-ttu-id="38128-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38128-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38128-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38128-116">Request body</span></span>
<span data-ttu-id="38128-117">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38128-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38128-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="38128-118">Response</span></span>

<span data-ttu-id="38128-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика. Если у пользователя нет настроенных переопределений, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="38128-p103">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="38128-121">Пример</span><span class="sxs-lookup"><span data-stu-id="38128-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38128-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="38128-122">Request</span></span>
<span data-ttu-id="38128-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38128-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="38128-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="38128-124">Response</span></span>
<span data-ttu-id="38128-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="38128-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Fanny Downs",
        "address": "fannyd@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->