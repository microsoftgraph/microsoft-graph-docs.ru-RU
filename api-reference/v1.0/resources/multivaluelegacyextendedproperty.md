# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="7b2ac-101">Тип ресурса multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7b2ac-101">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="7b2ac-102">Расширенное свойство, содержащее коллекцию значений.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-102">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="7b2ac-103">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="7b2ac-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="7b2ac-104">Методы</span><span class="sxs-lookup"><span data-stu-id="7b2ac-104">Methods</span></span>

| <span data-ttu-id="7b2ac-105">Метод</span><span class="sxs-lookup"><span data-stu-id="7b2ac-105">Method</span></span>           | <span data-ttu-id="7b2ac-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7b2ac-106">Return Type</span></span>    |<span data-ttu-id="7b2ac-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7b2ac-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b2ac-108">Запись блога</span><span class="sxs-lookup"><span data-stu-id="7b2ac-108">Post</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | <span data-ttu-id="7b2ac-p101">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md). Обратите внимание, что ресурсы [post](../resources/post.md) групп не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="7b2ac-111">Создание объекта **multiValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-111">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="7b2ac-112">|||UNTRANSLATED_CONTENT_START|||Get|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="7b2ac-112">Get</span></span>](../api/multivaluelegacyextendedproperty_get.md) |<span data-ttu-id="7b2ac-113">Экземпляр поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы), расширенный объектом [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="7b2ac-113">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="7b2ac-114">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-114">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b2ac-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b2ac-115">Properties</span></span>
| <span data-ttu-id="7b2ac-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b2ac-116">Property</span></span>     | <span data-ttu-id="7b2ac-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7b2ac-117">Type</span></span>   |<span data-ttu-id="7b2ac-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7b2ac-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b2ac-119">id</span><span class="sxs-lookup"><span data-stu-id="7b2ac-119">id</span></span>|<span data-ttu-id="7b2ac-120">строка</span><span class="sxs-lookup"><span data-stu-id="7b2ac-120">string</span></span>|<span data-ttu-id="7b2ac-p102">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="7b2ac-123">value</span><span class="sxs-lookup"><span data-stu-id="7b2ac-123">value</span></span>|<span data-ttu-id="7b2ac-124">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b2ac-124">string collection</span></span>|<span data-ttu-id="7b2ac-125">Коллекция значений свойств.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-125">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b2ac-126">Связи</span><span class="sxs-lookup"><span data-stu-id="7b2ac-126">Relationships</span></span>
<span data-ttu-id="7b2ac-127">Нет</span><span class="sxs-lookup"><span data-stu-id="7b2ac-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b2ac-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b2ac-128">JSON representation</span></span>

<span data-ttu-id="7b2ac-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b2ac-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->