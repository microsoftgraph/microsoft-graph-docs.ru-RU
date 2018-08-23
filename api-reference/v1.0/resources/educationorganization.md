# <a name="educationorganization-resource-type"></a><span data-ttu-id="ef47a-101">Тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="ef47a-101">educationOrganization resource type</span></span>

<span data-ttu-id="ef47a-102">Абстрактный объект, используемый для моделирования общности различных типов организаций в рамках образовательного сектора.</span><span class="sxs-lookup"><span data-stu-id="ef47a-102">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="ef47a-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef47a-103">Properties</span></span>
| <span data-ttu-id="ef47a-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef47a-104">Property</span></span>     | <span data-ttu-id="ef47a-105">Тип</span><span class="sxs-lookup"><span data-stu-id="ef47a-105">Type</span></span>   |<span data-ttu-id="ef47a-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ef47a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef47a-107">description</span><span class="sxs-lookup"><span data-stu-id="ef47a-107">description</span></span>|<span data-ttu-id="ef47a-108">Строка</span><span class="sxs-lookup"><span data-stu-id="ef47a-108">String</span></span>| <span data-ttu-id="ef47a-109">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="ef47a-109">Organization description.</span></span>|
|<span data-ttu-id="ef47a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ef47a-110">displayName</span></span>|<span data-ttu-id="ef47a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ef47a-111">String</span></span>| <span data-ttu-id="ef47a-112">Отображаемое имя организации.</span><span class="sxs-lookup"><span data-stu-id="ef47a-112">Organization display name.</span></span>|
|<span data-ttu-id="ef47a-113">externalSource</span><span class="sxs-lookup"><span data-stu-id="ef47a-113">externalSource</span></span>|<span data-ttu-id="ef47a-114">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="ef47a-114">educationExternalSource</span></span>| <span data-ttu-id="ef47a-115">Источник создания данной организации.</span><span class="sxs-lookup"><span data-stu-id="ef47a-115">Source where this organization was created from.</span></span> <span data-ttu-id="ef47a-116">Возможные значения: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ef47a-116">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef47a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ef47a-117">Relationships</span></span>
<span data-ttu-id="ef47a-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ef47a-118">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ef47a-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ef47a-119">JSON representation</span></span>

<span data-ttu-id="ef47a-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef47a-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->