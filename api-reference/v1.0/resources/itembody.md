# <a name="itembody-resource-type"></a><span data-ttu-id="5dd57-101">Тип ресурса itemBody</span><span class="sxs-lookup"><span data-stu-id="5dd57-101">itemBody resource type</span></span>

<span data-ttu-id="5dd57-102">Представляет свойства основного текста элемента, например сообщения, события или записи группы.</span><span class="sxs-lookup"><span data-stu-id="5dd57-102">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="5dd57-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dd57-103">Properties</span></span>
| <span data-ttu-id="5dd57-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dd57-104">Property</span></span>     | <span data-ttu-id="5dd57-105">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd57-105">Type</span></span>   |<span data-ttu-id="5dd57-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd57-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dd57-107">content</span><span class="sxs-lookup"><span data-stu-id="5dd57-107">content</span></span>|<span data-ttu-id="5dd57-108">Строка</span><span class="sxs-lookup"><span data-stu-id="5dd57-108">String</span></span>|<span data-ttu-id="5dd57-109">Содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="5dd57-109">The content of the item.</span></span>|
|<span data-ttu-id="5dd57-110">contentType</span><span class="sxs-lookup"><span data-stu-id="5dd57-110">contentType</span></span>|<span data-ttu-id="5dd57-111">bodyType</span><span class="sxs-lookup"><span data-stu-id="5dd57-111">BodyType</span></span>|<span data-ttu-id="5dd57-p101">Тип содержимого. Возможные значения: `Text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="5dd57-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dd57-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dd57-114">JSON representation</span></span>

<span data-ttu-id="5dd57-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dd57-115">Here is a JSON representation of the resource</span></span>

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
