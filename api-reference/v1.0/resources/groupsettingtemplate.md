# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="9899f-101">Тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9899f-101">groupSettingTemplate resource type</span></span>

<span data-ttu-id="9899f-p101">Шаблоны параметров группы представляют определенные системой параметры для клиента. Можно на базе доступных объектов **groupSettingTemplate** создавать [параметры группы](groupsetting.md), а также менять предопределенные значения по умолчанию этих параметров. Шаблоны параметров группы невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или отдельной группы. На данный момент доступны только шаблоны, применимые к группам Office 365 и включающие параметры, которые, например, разрешают или запрещают пользователям создавать группы либо приглашать внешних гостей в группу.</span><span class="sxs-lookup"><span data-stu-id="9899f-p101">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="9899f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9899f-107">Methods</span></span>

| <span data-ttu-id="9899f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9899f-108">Method</span></span> | <span data-ttu-id="9899f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9899f-109">Return Type</span></span> | <span data-ttu-id="9899f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9899f-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9899f-111">Получение groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9899f-111">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate_get.md) | [<span data-ttu-id="9899f-112">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9899f-112">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="9899f-113">Считывание конкретных свойств одного из определенных системой объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="9899f-113">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="9899f-114">Перечисление groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9899f-114">List groupSettingTemplate</span></span>](../api/groupsettingtemplate_list.md) | [<span data-ttu-id="9899f-115">Коллекция объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="9899f-115">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="9899f-116">Перечисление всех определенных системой объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="9899f-116">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="9899f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9899f-117">Properties</span></span>

| <span data-ttu-id="9899f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9899f-118">Property</span></span> | <span data-ttu-id="9899f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9899f-119">Type</span></span> | <span data-ttu-id="9899f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9899f-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9899f-121">description</span><span class="sxs-lookup"><span data-stu-id="9899f-121">description</span></span>|<span data-ttu-id="9899f-122">Строка</span><span class="sxs-lookup"><span data-stu-id="9899f-122">String</span></span>| <span data-ttu-id="9899f-123">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="9899f-123">Description of the template.</span></span> |
|<span data-ttu-id="9899f-124">displayName</span><span class="sxs-lookup"><span data-stu-id="9899f-124">displayName</span></span>|<span data-ttu-id="9899f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9899f-125">String</span></span>| <span data-ttu-id="9899f-126">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="9899f-126">Display name of the template.</span></span> |
|<span data-ttu-id="9899f-127">id</span><span class="sxs-lookup"><span data-stu-id="9899f-127">id</span></span>|<span data-ttu-id="9899f-128">Строка</span><span class="sxs-lookup"><span data-stu-id="9899f-128">String</span></span>| <span data-ttu-id="9899f-p102">Уникальный идентификатор шаблона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9899f-p102">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="9899f-131">values</span><span class="sxs-lookup"><span data-stu-id="9899f-131">values</span></span>|<span data-ttu-id="9899f-132">Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="9899f-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="9899f-133">Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.</span><span class="sxs-lookup"><span data-stu-id="9899f-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9899f-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="9899f-134">Relationships</span></span>

<span data-ttu-id="9899f-135">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9899f-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9899f-136">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9899f-136">JSON representation</span></span>

<span data-ttu-id="9899f-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9899f-137">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->