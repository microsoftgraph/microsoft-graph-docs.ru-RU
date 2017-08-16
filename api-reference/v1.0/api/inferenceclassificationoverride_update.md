# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="d16f1-101">Обновление объекта inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="d16f1-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="d16f1-102">Изменение поля **classifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="d16f1-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="d16f1-103">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md).</span><span class="sxs-lookup"><span data-stu-id="d16f1-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="d16f1-104">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification_post_overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="d16f1-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="d16f1-105">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride_delete.md) существующее переопределение и [создав](inferenceclassification_post_overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="d16f1-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d16f1-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d16f1-106">Prerequisites</span></span>
<span data-ttu-id="d16f1-107">Для применения этого API требуется следующая **область**: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="d16f1-107">The following **scopes** are required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="d16f1-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d16f1-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d16f1-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d16f1-109">Request headers</span></span>
| <span data-ttu-id="d16f1-110">Имя</span><span class="sxs-lookup"><span data-stu-id="d16f1-110">Name</span></span>       | <span data-ttu-id="d16f1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d16f1-111">Type</span></span> | <span data-ttu-id="d16f1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d16f1-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d16f1-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="d16f1-113">Authorization</span></span>  | <span data-ttu-id="d16f1-114">string</span><span class="sxs-lookup"><span data-stu-id="d16f1-114">string</span></span>  | <span data-ttu-id="d16f1-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d16f1-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d16f1-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d16f1-117">Content-Type</span></span> | <span data-ttu-id="d16f1-118">string</span><span class="sxs-lookup"><span data-stu-id="d16f1-118">string</span></span>  | <span data-ttu-id="d16f1-p102">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d16f1-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d16f1-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d16f1-121">Request body</span></span>
<span data-ttu-id="d16f1-p103">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="d16f1-p103">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="d16f1-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d16f1-124">Property</span></span>     | <span data-ttu-id="d16f1-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d16f1-125">Type</span></span>   |<span data-ttu-id="d16f1-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d16f1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d16f1-127">classifyAs</span><span class="sxs-lookup"><span data-stu-id="d16f1-127">classifyAs</span></span>|<span data-ttu-id="d16f1-128">string</span><span class="sxs-lookup"><span data-stu-id="d16f1-128">string</span></span>| <span data-ttu-id="d16f1-p104">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="d16f1-p104">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="d16f1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d16f1-131">Response</span></span>

<span data-ttu-id="d16f1-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d16f1-132">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d16f1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d16f1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d16f1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d16f1-134">Request</span></span>
<span data-ttu-id="d16f1-135">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="d16f1-135">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="d16f1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d16f1-136">Response</span></span>
<span data-ttu-id="d16f1-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d16f1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->