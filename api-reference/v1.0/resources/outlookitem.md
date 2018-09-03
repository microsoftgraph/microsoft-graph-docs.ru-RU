# <a name="outlookitem-resource-type"></a><span data-ttu-id="4b115-101">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="4b115-101">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="4b115-102">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b115-102">JSON representation</span></span>

<span data-ttu-id="4b115-103">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="4b115-103">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookItem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="4b115-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b115-104">Properties</span></span>
| <span data-ttu-id="4b115-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b115-105">Property</span></span>     | <span data-ttu-id="4b115-106">Тип</span><span class="sxs-lookup"><span data-stu-id="4b115-106">Type</span></span>   |<span data-ttu-id="4b115-107">Описание</span><span class="sxs-lookup"><span data-stu-id="4b115-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b115-108">categories</span><span class="sxs-lookup"><span data-stu-id="4b115-108">categories</span></span>|<span data-ttu-id="4b115-109">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b115-109">String collection</span></span>|<span data-ttu-id="4b115-110">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="4b115-110">The categories associated with the message.</span></span>|
|<span data-ttu-id="4b115-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="4b115-111">changeKey</span></span>|<span data-ttu-id="4b115-112">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4b115-112">String</span></span>|<span data-ttu-id="4b115-113">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="4b115-113">Optional. Represents the version of the list item.</span></span> <span data-ttu-id="4b115-114">При каждом изменении элемента свойство ChangeKey также меняется.</span><span class="sxs-lookup"><span data-stu-id="4b115-114">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="4b115-115">Это позволяет программе Exchange применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="4b115-115">Identifies the version of the reminder. Every time the reminder is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="4b115-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b115-116">Read-only.</span></span>|
|<span data-ttu-id="4b115-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b115-117">createdDateTime</span></span>|<span data-ttu-id="4b115-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b115-118">DateTimeOffset</span></span>|<span data-ttu-id="4b115-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4b115-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4b115-121">id</span><span class="sxs-lookup"><span data-stu-id="4b115-121">id</span></span>|<span data-ttu-id="4b115-122">строка</span><span class="sxs-lookup"><span data-stu-id="4b115-122">String</span></span>| <span data-ttu-id="4b115-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b115-123">Read-only.</span></span>|
|<span data-ttu-id="4b115-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b115-124">lastModifiedDateTime</span></span>|<span data-ttu-id="4b115-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b115-125">DateTimeOffset</span></span>|<span data-ttu-id="4b115-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4b115-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b115-128">Связи</span><span class="sxs-lookup"><span data-stu-id="4b115-128">Relationships</span></span>
<span data-ttu-id="4b115-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4b115-129">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
