# <a name="alerttrigger-resource-type"></a><span data-ttu-id="5e22e-101">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="5e22e-101">alertTrigger resource type</span></span>

<span data-ttu-id="5e22e-102">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="5e22e-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="5e22e-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e22e-103">Properties</span></span>

| <span data-ttu-id="5e22e-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e22e-104">Property</span></span>   | <span data-ttu-id="5e22e-105">Тип</span><span class="sxs-lookup"><span data-stu-id="5e22e-105">Type</span></span>|<span data-ttu-id="5e22e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5e22e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e22e-107">name</span><span class="sxs-lookup"><span data-stu-id="5e22e-107">name</span></span>|<span data-ttu-id="5e22e-108">String</span><span class="sxs-lookup"><span data-stu-id="5e22e-108">String</span></span>|<span data-ttu-id="5e22e-109">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5e22e-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="5e22e-110">type</span><span class="sxs-lookup"><span data-stu-id="5e22e-110">type</span></span>|<span data-ttu-id="5e22e-111">String</span><span class="sxs-lookup"><span data-stu-id="5e22e-111">String</span></span>|<span data-ttu-id="5e22e-112">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="5e22e-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="5e22e-113">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="5e22e-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="5e22e-114">value</span><span class="sxs-lookup"><span data-stu-id="5e22e-114">value</span></span>|<span data-ttu-id="5e22e-115">String</span><span class="sxs-lookup"><span data-stu-id="5e22e-115">String</span></span>|<span data-ttu-id="5e22e-116">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5e22e-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e22e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e22e-117">JSON representation</span></span>

<span data-ttu-id="5e22e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e22e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="5e22e-119">Пример</span><span class="sxs-lookup"><span data-stu-id="5e22e-119">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->