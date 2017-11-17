# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="af0c9-101">Тип ресурса settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="af0c9-101">settingTemplateValue resource type</span></span>

<span data-ttu-id="af0c9-102">Представляет определение отдельного параметра шаблона, включая значение по умолчанию для этого параметра, если экземпляр этого параметра не создан.</span><span class="sxs-lookup"><span data-stu-id="af0c9-102">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="af0c9-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="af0c9-103">Properties</span></span>

| <span data-ttu-id="af0c9-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="af0c9-104">Property</span></span> | <span data-ttu-id="af0c9-105">Тип</span><span class="sxs-lookup"><span data-stu-id="af0c9-105">Type</span></span> | <span data-ttu-id="af0c9-106">Описание</span><span class="sxs-lookup"><span data-stu-id="af0c9-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="af0c9-107">defaultValue</span><span class="sxs-lookup"><span data-stu-id="af0c9-107">DefaultValue</span></span>|<span data-ttu-id="af0c9-108">String</span><span class="sxs-lookup"><span data-stu-id="af0c9-108">String</span></span>| <span data-ttu-id="af0c9-109">Значение по умолчанию для параметра.</span><span class="sxs-lookup"><span data-stu-id="af0c9-109">Default value for the setting.</span></span> |
|<span data-ttu-id="af0c9-110">description</span><span class="sxs-lookup"><span data-stu-id="af0c9-110">description</span></span>|<span data-ttu-id="af0c9-111">String</span><span class="sxs-lookup"><span data-stu-id="af0c9-111">String</span></span>| <span data-ttu-id="af0c9-112">Описание параметра.</span><span class="sxs-lookup"><span data-stu-id="af0c9-112">Description of the component.</span></span> |
|<span data-ttu-id="af0c9-113">name</span><span class="sxs-lookup"><span data-stu-id="af0c9-113">name</span></span>|<span data-ttu-id="af0c9-114">String</span><span class="sxs-lookup"><span data-stu-id="af0c9-114">String</span></span>| <span data-ttu-id="af0c9-115">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="af0c9-115">Name of the setting.</span></span> |
|<span data-ttu-id="af0c9-116">type</span><span class="sxs-lookup"><span data-stu-id="af0c9-116">type</span></span>|<span data-ttu-id="af0c9-117">String</span><span class="sxs-lookup"><span data-stu-id="af0c9-117">String</span></span>| <span data-ttu-id="af0c9-118">Тип параметра.</span><span class="sxs-lookup"><span data-stu-id="af0c9-118">Key of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="af0c9-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="af0c9-119">JSON representation</span></span>

<span data-ttu-id="af0c9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af0c9-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->