# <a name="settingvalue-resource-type"></a><span data-ttu-id="0ecdf-101">Тип ресурса settingValue</span><span class="sxs-lookup"><span data-stu-id="0ecdf-101">settingValue resource type</span></span>

<span data-ttu-id="0ecdf-102">Параметр, представленный парой "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="0ecdf-102">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="0ecdf-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ecdf-103">Properties</span></span>

| <span data-ttu-id="0ecdf-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ecdf-104">Property</span></span> | <span data-ttu-id="0ecdf-105">Тип</span><span class="sxs-lookup"><span data-stu-id="0ecdf-105">Type</span></span> | <span data-ttu-id="0ecdf-106">Описание</span><span class="sxs-lookup"><span data-stu-id="0ecdf-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0ecdf-107">name</span><span class="sxs-lookup"><span data-stu-id="0ecdf-107">name</span></span>|<span data-ttu-id="0ecdf-108">String</span><span class="sxs-lookup"><span data-stu-id="0ecdf-108">String</span></span>| <span data-ttu-id="0ecdf-109">Имя параметра, определенное [groupSettingTemplate](groupsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="0ecdf-109">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="0ecdf-110">value</span><span class="sxs-lookup"><span data-stu-id="0ecdf-110">value</span></span>|<span data-ttu-id="0ecdf-111">String</span><span class="sxs-lookup"><span data-stu-id="0ecdf-111">String</span></span>| <span data-ttu-id="0ecdf-112">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="0ecdf-112">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="0ecdf-113">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ecdf-113">JSON representation</span></span>

<span data-ttu-id="0ecdf-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ecdf-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->