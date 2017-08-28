# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="ec1cf-101">Тип ресурса singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ec1cf-101">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="ec1cf-102">Расширенное свойство, содержащее одно значение.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-102">An extended property that contains a single value.</span></span> 

<span data-ttu-id="ec1cf-103">Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="ec1cf-103">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="ec1cf-104">Методы</span><span class="sxs-lookup"><span data-stu-id="ec1cf-104">Methods</span></span>

| <span data-ttu-id="ec1cf-105">Метод</span><span class="sxs-lookup"><span data-stu-id="ec1cf-105">Method</span></span>           | <span data-ttu-id="ec1cf-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec1cf-106">Return Type</span></span>    |<span data-ttu-id="ec1cf-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ec1cf-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec1cf-108">Создание</span><span class="sxs-lookup"><span data-stu-id="ec1cf-108">Post</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | <span data-ttu-id="ec1cf-109">Экземпляр поддерживаемого ресурса: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) или [contactFolder](../resources/contactfolder.md), но не [post](../resources/post.md) группы.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-109">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="ec1cf-110">Создание объекта **singleValueLegacyExtendedProperty** в новом или существующем экземпляре поддерживаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-110">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="ec1cf-111">Получение</span><span class="sxs-lookup"><span data-stu-id="ec1cf-111">GET</span></span>](../api/singlevaluelegacyextendedproperty_get.md) |<span data-ttu-id="ec1cf-112">Один или несколько экземпляров поддерживаемого ресурса ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) или [post](../resources/post.md) группы) либо один такой экземпляр, расширенный объектом [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="ec1cf-112">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="ec1cf-113">Получение экземпляра ресурса с расширенным свойством с помощью параметра `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-113">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec1cf-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec1cf-114">Properties</span></span>
| <span data-ttu-id="ec1cf-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec1cf-115">Property</span></span>     | <span data-ttu-id="ec1cf-116">Тип</span><span class="sxs-lookup"><span data-stu-id="ec1cf-116">Type</span></span>   |<span data-ttu-id="ec1cf-117">Описание</span><span class="sxs-lookup"><span data-stu-id="ec1cf-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec1cf-118">id</span><span class="sxs-lookup"><span data-stu-id="ec1cf-118">id</span></span>|<span data-ttu-id="ec1cf-119">string</span><span class="sxs-lookup"><span data-stu-id="ec1cf-119">string</span></span>|<span data-ttu-id="ec1cf-p101">Идентификатор свойства. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="ec1cf-122">значение</span><span class="sxs-lookup"><span data-stu-id="ec1cf-122">value</span></span>|<span data-ttu-id="ec1cf-123">string</span><span class="sxs-lookup"><span data-stu-id="ec1cf-123">string</span></span>|<span data-ttu-id="ec1cf-124">Значение свойства.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-124">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec1cf-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ec1cf-125">Relationships</span></span>
<span data-ttu-id="ec1cf-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ec1cf-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ec1cf-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec1cf-127">JSON representation</span></span>

<span data-ttu-id="ec1cf-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec1cf-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singlevaluelegacyextendedproperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->