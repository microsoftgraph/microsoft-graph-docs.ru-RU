# <a name="itembody-resource-type"></a><span data-ttu-id="4ef9b-101">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="4ef9b-101">itemBody resource type</span></span>

<span data-ttu-id="4ef9b-102">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="4ef9b-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="4ef9b-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ef9b-103">Properties</span></span>
| <span data-ttu-id="4ef9b-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef9b-104">Property</span></span>     | <span data-ttu-id="4ef9b-105">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef9b-105">Type</span></span>   |<span data-ttu-id="4ef9b-106">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef9b-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ef9b-107">content</span><span class="sxs-lookup"><span data-stu-id="4ef9b-107">content</span></span>|<span data-ttu-id="4ef9b-108">String</span><span class="sxs-lookup"><span data-stu-id="4ef9b-108">String</span></span>|<span data-ttu-id="4ef9b-109">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="4ef9b-109">The content of the item.</span></span>|
|<span data-ttu-id="4ef9b-110">contentType</span><span class="sxs-lookup"><span data-stu-id="4ef9b-110">contentType</span></span>|<span data-ttu-id="4ef9b-111">String</span><span class="sxs-lookup"><span data-stu-id="4ef9b-111">String</span></span>|<span data-ttu-id="4ef9b-p101">Тип контента. Возможные значения: `Text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="4ef9b-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ef9b-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ef9b-114">JSON representation</span></span>

<span data-ttu-id="4ef9b-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef9b-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
