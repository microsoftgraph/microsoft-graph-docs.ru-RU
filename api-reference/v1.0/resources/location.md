# <a name="location-resource-type"></a><span data-ttu-id="670a0-101">Тип ресурса Location</span><span class="sxs-lookup"><span data-stu-id="670a0-101">Location resource type</span></span>

<span data-ttu-id="670a0-102">Представляет сведения о месте проведения события.</span><span class="sxs-lookup"><span data-stu-id="670a0-102">Represents location information of an event.</span></span>


## <a name="properties"></a><span data-ttu-id="670a0-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="670a0-103">Properties</span></span>
| <span data-ttu-id="670a0-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="670a0-104">Property</span></span>  | <span data-ttu-id="670a0-105">Тип</span><span class="sxs-lookup"><span data-stu-id="670a0-105">Type</span></span>   | <span data-ttu-id="670a0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="670a0-106">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="670a0-107">address</span><span class="sxs-lookup"><span data-stu-id="670a0-107">address</span></span> | [<span data-ttu-id="670a0-108">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="670a0-108">physicalAddress</span></span>](physicalAddress.md) |<span data-ttu-id="670a0-109">Почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="670a0-109">The street address of the location.</span></span> |
| <span data-ttu-id="670a0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="670a0-110">displayName</span></span>  | <span data-ttu-id="670a0-111">String</span><span class="sxs-lookup"><span data-stu-id="670a0-111">String</span></span> | <span data-ttu-id="670a0-112">Имя, связанное с расположением.</span><span class="sxs-lookup"><span data-stu-id="670a0-112">The name associated with the location.</span></span>                       |
| <span data-ttu-id="670a0-113">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="670a0-113">locationEmailAddress</span></span> | <span data-ttu-id="670a0-114">String</span><span class="sxs-lookup"><span data-stu-id="670a0-114">String</span></span> | <span data-ttu-id="670a0-115">Необязательный адрес электронной почты для расположения.</span><span class="sxs-lookup"><span data-stu-id="670a0-115">Optional email address of the location.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="670a0-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="670a0-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a><span data-ttu-id="670a0-117">Заметки</span><span class="sxs-lookup"><span data-stu-id="670a0-117">Remarks</span></span>

<span data-ttu-id="670a0-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="670a0-118">For more information about the facets on a [driveItem](driveitem.md), see driveItem.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->