# <a name="persontype-resource-type"></a><span data-ttu-id="f00ff-101">тип ресурса personType</span><span class="sxs-lookup"><span data-stu-id="f00ff-101">personType resource type</span></span>

<span data-ttu-id="f00ff-102">Представляет тип пользователя.</span><span class="sxs-lookup"><span data-stu-id="f00ff-102">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f00ff-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f00ff-103">JSON representation</span></span>

<span data-ttu-id="f00ff-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f00ff-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persontype
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f00ff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f00ff-105">Properties</span></span>
| <span data-ttu-id="f00ff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f00ff-106">Property</span></span>     | <span data-ttu-id="f00ff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f00ff-107">Type</span></span>   |<span data-ttu-id="f00ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f00ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f00ff-109">класс</span><span class="sxs-lookup"><span data-stu-id="f00ff-109">class</span></span>|<span data-ttu-id="f00ff-110">String</span><span class="sxs-lookup"><span data-stu-id="f00ff-110">String</span></span>|<span data-ttu-id="f00ff-111">Тип источника данных, например Person.</span><span class="sxs-lookup"><span data-stu-id="f00ff-111">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="f00ff-112">subclass</span><span class="sxs-lookup"><span data-stu-id="f00ff-112">subclass</span></span>|<span data-ttu-id="f00ff-113">String</span><span class="sxs-lookup"><span data-stu-id="f00ff-113">String</span></span>|<span data-ttu-id="f00ff-114">Дополнительный тип источника данных, например OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="f00ff-114">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persontype resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
