# <a name="phone-resource-type"></a><span data-ttu-id="6f22c-101">Тип ресурса phone</span><span class="sxs-lookup"><span data-stu-id="6f22c-101">phone resource type</span></span>

<span data-ttu-id="6f22c-102">Представляет номер телефона.</span><span class="sxs-lookup"><span data-stu-id="6f22c-102">Represents a phone number identified in an item.</span></span>


## <a name="properties"></a><span data-ttu-id="6f22c-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f22c-103">Properties</span></span>
| <span data-ttu-id="6f22c-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f22c-104">Property</span></span>     | <span data-ttu-id="6f22c-105">Тип</span><span class="sxs-lookup"><span data-stu-id="6f22c-105">Type</span></span>   |<span data-ttu-id="6f22c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="6f22c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f22c-107">number</span><span class="sxs-lookup"><span data-stu-id="6f22c-107">number</span></span>|<span data-ttu-id="6f22c-108">string</span><span class="sxs-lookup"><span data-stu-id="6f22c-108">string</span></span>|<span data-ttu-id="6f22c-109">Номер телефона.</span><span class="sxs-lookup"><span data-stu-id="6f22c-109">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="6f22c-110">type</span><span class="sxs-lookup"><span data-stu-id="6f22c-110">type</span></span>|<span data-ttu-id="6f22c-111">String</span><span class="sxs-lookup"><span data-stu-id="6f22c-111">String</span></span>|<span data-ttu-id="6f22c-p101">Тип номера телефона. Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="6f22c-p101">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f22c-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6f22c-114">JSON representation</span></span>

<span data-ttu-id="6f22c-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f22c-115">Here is a JSON representation of the resource.</span></span>

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