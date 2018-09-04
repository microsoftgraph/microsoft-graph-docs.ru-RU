# <a name="phone-resource-type"></a><span data-ttu-id="6fa71-101">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="6fa71-101">phone resource type</span></span>

<span data-ttu-id="6fa71-102">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="6fa71-102">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="6fa71-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fa71-103">Properties</span></span>
| <span data-ttu-id="6fa71-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fa71-104">Property</span></span>     | <span data-ttu-id="6fa71-105">Тип</span><span class="sxs-lookup"><span data-stu-id="6fa71-105">Type</span></span>   |<span data-ttu-id="6fa71-106">Описание</span><span class="sxs-lookup"><span data-stu-id="6fa71-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fa71-107">number</span><span class="sxs-lookup"><span data-stu-id="6fa71-107">number</span></span>|<span data-ttu-id="6fa71-108">строка</span><span class="sxs-lookup"><span data-stu-id="6fa71-108">string</span></span>|<span data-ttu-id="6fa71-109">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="6fa71-109">The phone number.</span></span>|
|<span data-ttu-id="6fa71-110">type</span><span class="sxs-lookup"><span data-stu-id="6fa71-110">type</span></span>|<span data-ttu-id="6fa71-111">phoneType</span><span class="sxs-lookup"><span data-stu-id="6fa71-111">phoneType values</span></span>|<span data-ttu-id="6fa71-112">Тип номера телефона.</span><span class="sxs-lookup"><span data-stu-id="6fa71-112">The type of phone number.</span></span> <span data-ttu-id="6fa71-113">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="6fa71-113">The possible values are `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`, , or .</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fa71-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fa71-114">JSON representation</span></span>

<span data-ttu-id="6fa71-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fa71-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
