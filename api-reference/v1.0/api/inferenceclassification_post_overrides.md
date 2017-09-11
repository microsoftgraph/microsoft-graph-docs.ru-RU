# <a name="create-inferenceclassificationoverride"></a><span data-ttu-id="1b9e7-101">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="1b9e7-101">Create inferenceClassificationOverride</span></span>

<span data-ttu-id="1b9e7-p101">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>

<span data-ttu-id="1b9e7-104">**Примечание**</span><span class="sxs-lookup"><span data-stu-id="1b9e7-104">**Note**</span></span>

- <span data-ttu-id="1b9e7-105">Если переопределение с таким же SMTP-адресом уже существует, его поля **classifyAs** и **name** будут обновлены с использованием предоставленных значений.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-105">If an override already exists with the same STMP address, then the **classifyAs** and **name** fields of that override are updated with the provided values.</span></span>
- <span data-ttu-id="1b9e7-106">Максимальное количество переопределений, поддерживаемых для почтового ящика, — 1000. Они основываются на уникальных SMTP-адресах отправителей.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-106">The maximum number of overrides supported for a mailbox is 1000, based on unique sender SMTP addresses.</span></span>
- <span data-ttu-id="1b9e7-107">Операция POST поддерживает создание только одного переопределения в один момент времени.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-107">The POST operation supports creating only one override at a time.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b9e7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b9e7-108">Permissions</span></span>
<span data-ttu-id="1b9e7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1b9e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1b9e7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b9e7-111">Permission type</span></span>      | <span data-ttu-id="1b9e7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b9e7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b9e7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b9e7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1b9e7-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b9e7-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1b9e7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b9e7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b9e7-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b9e7-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1b9e7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b9e7-117">Application</span></span> | <span data-ttu-id="1b9e7-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b9e7-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b9e7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b9e7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/inferenceClassification/overrides
POST /users/{id}/inferenceClassification/overrides
```
## <a name="request-headers"></a><span data-ttu-id="1b9e7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b9e7-120">Request headers</span></span>
| <span data-ttu-id="1b9e7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1b9e7-121">Name</span></span>       | <span data-ttu-id="1b9e7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1b9e7-122">Type</span></span> | <span data-ttu-id="1b9e7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1b9e7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b9e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b9e7-124">Authorization</span></span>  | <span data-ttu-id="1b9e7-125">string</span><span class="sxs-lookup"><span data-stu-id="1b9e7-125">string</span></span>  | <span data-ttu-id="1b9e7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b9e7-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b9e7-128">Content-Type</span></span> | <span data-ttu-id="1b9e7-129">string</span><span class="sxs-lookup"><span data-stu-id="1b9e7-129">string</span></span>  | <span data-ttu-id="1b9e7-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b9e7-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b9e7-132">Request body</span></span>
<span data-ttu-id="1b9e7-133">В тексте запроса предоставьте описание объекта [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-133">In the request body, supply a JSON representation of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b9e7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b9e7-134">Response</span></span>

<span data-ttu-id="1b9e7-135">В случае успешного выполнения этот метод возвращает код отклика `201, Created` и объект [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-135">If successful, this method returns `201, Created` response code and an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b9e7-136">Пример</span><span class="sxs-lookup"><span data-stu-id="1b9e7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b9e7-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b9e7-137">Request</span></span>
<span data-ttu-id="1b9e7-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassificationoverride_from_inferenceclassification"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  }
}
```

##### <a name="response"></a><span data-ttu-id="1b9e7-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b9e7-139">Response</span></span>
<span data-ttu-id="1b9e7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b9e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Samantha Booth",
    "address": "samanthab@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create inferenceClassificationOverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->