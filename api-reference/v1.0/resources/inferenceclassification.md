# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="fd0e5-101">Тип ресурса inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="fd0e5-101">inferenceClassification resource type</span></span>

<span data-ttu-id="fd0e5-102">Классификация сообщений пользователя, позволяющая сосредоточиться на самых важных сообщениях.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-102">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="fd0e5-103">Дополнительные сведения см. в статье [Управление сортировкой почты](manage_focused_inbox.md).</span><span class="sxs-lookup"><span data-stu-id="fd0e5-103">For more information, see [Manage Focused Inbox](manage_focused_inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fd0e5-104">Методы</span><span class="sxs-lookup"><span data-stu-id="fd0e5-104">Methods</span></span>

| <span data-ttu-id="fd0e5-105">Метод</span><span class="sxs-lookup"><span data-stu-id="fd0e5-105">Method</span></span>           | <span data-ttu-id="fd0e5-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fd0e5-106">Return Type</span></span>    |<span data-ttu-id="fd0e5-107">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0e5-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd0e5-108">Создание объекта inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fd0e5-108">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification_post_overrides.md) |[<span data-ttu-id="fd0e5-109">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fd0e5-109">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="fd0e5-p101">Создание переопределения для отправителя, определенного адресом SMTP. Последующие сообщения с этого SMTP-адреса всегда будут классифицироваться так, как указано в переопределении.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="fd0e5-112">Список переопределений</span><span class="sxs-lookup"><span data-stu-id="fd0e5-112">List overrides</span></span>](../api/inferenceclassification_list_overrides.md) |<span data-ttu-id="fd0e5-113">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fd0e5-113">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fd0e5-114">Получение переопределений, настроенных пользователем для классификации сообщений от определенных отправителей.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-114">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd0e5-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd0e5-115">Properties</span></span>
| <span data-ttu-id="fd0e5-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd0e5-116">Property</span></span>     | <span data-ttu-id="fd0e5-117">Тип</span><span class="sxs-lookup"><span data-stu-id="fd0e5-117">Type</span></span>   |<span data-ttu-id="fd0e5-118">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0e5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd0e5-119">id</span><span class="sxs-lookup"><span data-stu-id="fd0e5-119">id</span></span>|<span data-ttu-id="fd0e5-120">строка</span><span class="sxs-lookup"><span data-stu-id="fd0e5-120">string</span></span>| <span data-ttu-id="fd0e5-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd0e5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="fd0e5-122">Relationships</span></span>
| <span data-ttu-id="fd0e5-123">Связь</span><span class="sxs-lookup"><span data-stu-id="fd0e5-123">Relationship</span></span> | <span data-ttu-id="fd0e5-124">Тип</span><span class="sxs-lookup"><span data-stu-id="fd0e5-124">Type</span></span>   |<span data-ttu-id="fd0e5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="fd0e5-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd0e5-126">overrides</span><span class="sxs-lookup"><span data-stu-id="fd0e5-126">overrides</span></span>|<span data-ttu-id="fd0e5-127">Коллекция объектов [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="fd0e5-127">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="fd0e5-p102">Набор переопределений пользователя, классифицирующих сообщения от определенных отправителей указанными способами: `focused` или `other`. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd0e5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd0e5-131">JSON representation</span></span>

<span data-ttu-id="fd0e5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd0e5-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->