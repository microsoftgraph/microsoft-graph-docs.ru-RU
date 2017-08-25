# <a name="list-overrides"></a><span data-ttu-id="bc8c8-101">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="bc8c8-101">List overrides</span></span>

<span data-ttu-id="bc8c8-102">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-102">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="bc8c8-p101">Каждое переопределение соответствует SMTP-адресу отправителя. Изначально у пользователя нет переопределений.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc8c8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc8c8-105">Permissions</span></span>
<span data-ttu-id="bc8c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc8c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc8c8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc8c8-108">Permission type</span></span>      | <span data-ttu-id="bc8c8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc8c8-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bc8c8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc8c8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc8c8-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bc8c8-111">Mail.Read</span></span>    | 
|<span data-ttu-id="bc8c8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc8c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc8c8-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bc8c8-113">Mail.Read</span></span>    | 
|<span data-ttu-id="bc8c8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc8c8-114">Application</span></span> | <span data-ttu-id="bc8c8-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bc8c8-115">Mail.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bc8c8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc8c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="bc8c8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc8c8-117">Request headers</span></span>
| <span data-ttu-id="bc8c8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bc8c8-118">Name</span></span>       | <span data-ttu-id="bc8c8-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bc8c8-119">Type</span></span> | <span data-ttu-id="bc8c8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc8c8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bc8c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc8c8-121">Authorization</span></span>  | <span data-ttu-id="bc8c8-122">string</span><span class="sxs-lookup"><span data-stu-id="bc8c8-122">string</span></span>  | <span data-ttu-id="bc8c8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc8c8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc8c8-125">Request body</span></span>
<span data-ttu-id="bc8c8-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc8c8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc8c8-127">Response</span></span>

<span data-ttu-id="bc8c8-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика. Если у пользователя нет настроенных переопределений, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="bc8c8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bc8c8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc8c8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc8c8-131">Request</span></span>
<span data-ttu-id="bc8c8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="bc8c8-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc8c8-133">Response</span></span>
<span data-ttu-id="bc8c8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bc8c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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