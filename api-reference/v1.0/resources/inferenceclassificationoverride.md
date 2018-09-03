# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="d6198-101">Тип ресурса inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d6198-101">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="d6198-102">Представляет пользовательское переопределение для классификации входящих сообщений от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="d6198-102">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="d6198-103">Методы</span><span class="sxs-lookup"><span data-stu-id="d6198-103">Methods</span></span>

| <span data-ttu-id="d6198-104">Метод</span><span class="sxs-lookup"><span data-stu-id="d6198-104">Method</span></span>           | <span data-ttu-id="d6198-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d6198-105">Return Type</span></span>    |<span data-ttu-id="d6198-106">Описание</span><span class="sxs-lookup"><span data-stu-id="d6198-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6198-107">Обновление</span><span class="sxs-lookup"><span data-stu-id="d6198-107">Update</span></span>](../api/inferenceclassificationoverride_update.md) | [<span data-ttu-id="d6198-108">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d6198-108">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="d6198-109">Изменение поля **ClassifyAs** переопределения указанным образом.</span><span class="sxs-lookup"><span data-stu-id="d6198-109">Change the **classifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="d6198-110">Удаление</span><span class="sxs-lookup"><span data-stu-id="d6198-110">Delete</span></span>](../api/inferenceclassificationoverride_delete.md) | <span data-ttu-id="d6198-111">Нет</span><span class="sxs-lookup"><span data-stu-id="d6198-111">None</span></span> |<span data-ttu-id="d6198-112">Удаление переопределения по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="d6198-112">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6198-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6198-113">Properties</span></span>
| <span data-ttu-id="d6198-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6198-114">Property</span></span>     | <span data-ttu-id="d6198-115">Тип</span><span class="sxs-lookup"><span data-stu-id="d6198-115">Type</span></span>   |<span data-ttu-id="d6198-116">Описание</span><span class="sxs-lookup"><span data-stu-id="d6198-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6198-117">classifyAs</span><span class="sxs-lookup"><span data-stu-id="d6198-117">classifyAs</span></span>|<span data-ttu-id="d6198-118">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="d6198-118">inferenceClassificationType</span></span>| <span data-ttu-id="d6198-119">Указывает, как должны классифицироваться все входящие сообщения от определенного отправителя.</span><span class="sxs-lookup"><span data-stu-id="d6198-119">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: , .</span></span> <span data-ttu-id="d6198-120">Возможные значения: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="d6198-120">The possible values are:</span></span>|
|<span data-ttu-id="d6198-121">id</span><span class="sxs-lookup"><span data-stu-id="d6198-121">id</span></span>|<span data-ttu-id="d6198-122">string (строка)</span><span class="sxs-lookup"><span data-stu-id="d6198-122">string</span></span>| <span data-ttu-id="d6198-p102">Уникальный идентификатор переопределения. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d6198-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="d6198-125">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d6198-125">senderEmailAddress</span></span>|[<span data-ttu-id="d6198-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d6198-126">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="d6198-127">Сведения об электронном адресе отправителя, для которого создано переопределение.</span><span class="sxs-lookup"><span data-stu-id="d6198-127">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6198-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d6198-128">Relationships</span></span>
<span data-ttu-id="d6198-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d6198-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d6198-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6198-130">JSON representation</span></span>

<span data-ttu-id="d6198-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6198-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->