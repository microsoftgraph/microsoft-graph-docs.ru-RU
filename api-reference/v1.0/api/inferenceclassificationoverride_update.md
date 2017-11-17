# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="97789-101">Обновление объекта inferenceclassificationoverride</span><span class="sxs-lookup"><span data-stu-id="97789-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="97789-102">Изменение поля **classifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="97789-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="97789-103">Вы не можете использовать операцию PATCH, чтобы менять поля в экземпляре [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md).</span><span class="sxs-lookup"><span data-stu-id="97789-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="97789-104">Если для конкретного отправителя существует переопределение и он меняет свое отображаемое имя, вы можете использовать операцию [POST](inferenceclassification_post_overrides.md) для принудительного обновления поля ввода имени в имеющемся переопределении.</span><span class="sxs-lookup"><span data-stu-id="97789-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="97789-105">Если для конкретного отправителя существует переопределение и он меняет свой SMTP-адрес, "обновить" переопределение для этого отправителя можно только [удалив](inferenceclassificationoverride_delete.md) существующее переопределение и [создав](inferenceclassification_post_overrides.md) другое с новым SMTP-адресом.</span><span class="sxs-lookup"><span data-stu-id="97789-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="97789-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97789-106">Permissions</span></span>
<span data-ttu-id="97789-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97789-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97789-109">Permission type</span></span>      | <span data-ttu-id="97789-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97789-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97789-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97789-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97789-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97789-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97789-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97789-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97789-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97789-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="97789-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97789-115">Application</span></span> | <span data-ttu-id="97789-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97789-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="97789-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97789-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97789-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97789-118">Request headers</span></span>
| <span data-ttu-id="97789-119">Имя</span><span class="sxs-lookup"><span data-stu-id="97789-119">Name</span></span>       | <span data-ttu-id="97789-120">Тип</span><span class="sxs-lookup"><span data-stu-id="97789-120">Type</span></span> | <span data-ttu-id="97789-121">Описание</span><span class="sxs-lookup"><span data-stu-id="97789-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97789-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97789-122">Authorization</span></span>  | <span data-ttu-id="97789-123">string</span><span class="sxs-lookup"><span data-stu-id="97789-123">string</span></span>  | <span data-ttu-id="97789-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97789-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97789-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97789-126">Content-Type</span></span> | <span data-ttu-id="97789-127">string</span><span class="sxs-lookup"><span data-stu-id="97789-127">string</span></span>  | <span data-ttu-id="97789-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97789-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97789-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97789-130">Request body</span></span>
<span data-ttu-id="97789-p104">В тексте запроса предоставьте новое значение для поля **classifyAs**. Чтобы производительность была максимальной, не следует включать существующие значения, которые не меняются.</span><span class="sxs-lookup"><span data-stu-id="97789-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="97789-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="97789-133">Property</span></span>     | <span data-ttu-id="97789-134">Тип</span><span class="sxs-lookup"><span data-stu-id="97789-134">Type</span></span>   |<span data-ttu-id="97789-135">Описание</span><span class="sxs-lookup"><span data-stu-id="97789-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97789-136">classifyAs</span><span class="sxs-lookup"><span data-stu-id="97789-136">classifyAs</span></span>|<span data-ttu-id="97789-137">string</span><span class="sxs-lookup"><span data-stu-id="97789-137">string</span></span>| <span data-ttu-id="97789-p105">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя. Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="97789-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="97789-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="97789-140">Response</span></span>

<span data-ttu-id="97789-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97789-141">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97789-142">Пример</span><span class="sxs-lookup"><span data-stu-id="97789-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97789-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="97789-143">Request</span></span>
<span data-ttu-id="97789-144">В следующем примере переопределение для SMTP-адреса randiw@adatum.onmicrosoft.com меняется из `other` на `focused`.</span><span class="sxs-lookup"><span data-stu-id="97789-144">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="97789-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="97789-145">Response</span></span>
<span data-ttu-id="97789-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="97789-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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