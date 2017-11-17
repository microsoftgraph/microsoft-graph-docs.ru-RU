# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="74761-101">Тип ресурса alternativeSecurityId</span><span class="sxs-lookup"><span data-stu-id="74761-101">alternativeSecurityId resource type</span></span>

<span data-ttu-id="74761-p101">Содержит альтернативный ИД безопасности, связанный с устройством. Свойство **alternativeSecurityIds** объекта [Device](device.md) представляет собой коллекцию объектов **alternativeSecurityId**.</span><span class="sxs-lookup"><span data-stu-id="74761-p101">Contains an alternative security ID associated with a device. The **alternativeSecurityIds** property of the [Device](device.md) entity is a collection of **alternativeSecurityId**.</span></span>

## <a name="properties"></a><span data-ttu-id="74761-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="74761-104">Properties</span></span>
| <span data-ttu-id="74761-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="74761-105">Property</span></span>     | <span data-ttu-id="74761-106">Тип</span><span class="sxs-lookup"><span data-stu-id="74761-106">Type</span></span>   |<span data-ttu-id="74761-107">Описание</span><span class="sxs-lookup"><span data-stu-id="74761-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74761-108">identityProvider</span><span class="sxs-lookup"><span data-stu-id="74761-108">identityProvider</span></span>|<span data-ttu-id="74761-109">String</span><span class="sxs-lookup"><span data-stu-id="74761-109">String</span></span>|            |
|<span data-ttu-id="74761-110">key</span><span class="sxs-lookup"><span data-stu-id="74761-110">key</span></span>|<span data-ttu-id="74761-111">Двоичный</span><span class="sxs-lookup"><span data-stu-id="74761-111">Binary</span></span>|            |
|<span data-ttu-id="74761-112">type</span><span class="sxs-lookup"><span data-stu-id="74761-112">type</span></span>|<span data-ttu-id="74761-113">Int32</span><span class="sxs-lookup"><span data-stu-id="74761-113">Int32</span></span>|            |

## <a name="json-representation"></a><span data-ttu-id="74761-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74761-114">JSON representation</span></span>

<span data-ttu-id="74761-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74761-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
