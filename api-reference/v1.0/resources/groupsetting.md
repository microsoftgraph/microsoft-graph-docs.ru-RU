# <a name="groupsetting-resource-type"></a><span data-ttu-id="efb92-101">Тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="efb92-101">groupSetting resource type</span></span>

<span data-ttu-id="efb92-102">Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, а также разрешение или запрещение пользователям-гостям быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="efb92-102">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="efb92-p101">Можно на базе доступных объектов [groupSettingTemplate](groupSettingTemplate.md) создавать параметры группы, а также менять предопределенные значения по умолчанию этих параметров. Они контролируют поведение групп на уровне клиента или отдельной группы. Если один и тот же параметр определен на двух уровнях — и клиента, и отдельной группы, параметр для группы переопределяет параметр для клиента.  Например, если получать приглашения от существующих членов групп разрешает пользователям параметр на уровне клиента, но запрещает параметр для отдельной группы, гости не смогут делать этого. Параметры группы контролируют только поведение групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="efb92-p101">Group settings can be created based on the available [groupSettingTemplates](groupSettingTemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="efb92-108">Методы</span><span class="sxs-lookup"><span data-stu-id="efb92-108">Methods</span></span>

| <span data-ttu-id="efb92-109">Метод</span><span class="sxs-lookup"><span data-stu-id="efb92-109">Method</span></span> | <span data-ttu-id="efb92-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efb92-110">Return Type</span></span> | <span data-ttu-id="efb92-111">Описание</span><span class="sxs-lookup"><span data-stu-id="efb92-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="efb92-112">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="efb92-112">Create setting</span></span>](../api/groupsetting_post_groupsettings.md) | [<span data-ttu-id="efb92-113">groupSetting</span><span class="sxs-lookup"><span data-stu-id="efb92-113">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="efb92-p102">Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="efb92-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="efb92-116">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="efb92-116">Get setting</span></span>](../api/groupsetting_get.md) | [<span data-ttu-id="efb92-117">groupSetting</span><span class="sxs-lookup"><span data-stu-id="efb92-117">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="efb92-118">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="efb92-118">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="efb92-119">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="efb92-119">List settings</span></span>](../api/groupsetting_list.md) | <span data-ttu-id="efb92-120">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="efb92-120">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="efb92-121">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="efb92-121">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="efb92-122">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="efb92-122">Update setting</span></span>](../api/groupsetting_update.md) | [<span data-ttu-id="efb92-123">groupSetting</span><span class="sxs-lookup"><span data-stu-id="efb92-123">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="efb92-124">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="efb92-124">Update groupsetting object.</span></span> |
|[<span data-ttu-id="efb92-125">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="efb92-125">Delete setting</span></span>](../api/groupsetting_delete.md) | <span data-ttu-id="efb92-126">Нет</span><span class="sxs-lookup"><span data-stu-id="efb92-126">None</span></span> | <span data-ttu-id="efb92-127">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="efb92-127">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="efb92-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="efb92-128">Properties</span></span>

| <span data-ttu-id="efb92-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="efb92-129">Property</span></span> | <span data-ttu-id="efb92-130">Тип</span><span class="sxs-lookup"><span data-stu-id="efb92-130">Type</span></span> | <span data-ttu-id="efb92-131">Описание</span><span class="sxs-lookup"><span data-stu-id="efb92-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="efb92-132">displayName</span><span class="sxs-lookup"><span data-stu-id="efb92-132">displayName</span></span>|<span data-ttu-id="efb92-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="efb92-133">String</span></span>| <span data-ttu-id="efb92-134">Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="efb92-134">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="efb92-135">id</span><span class="sxs-lookup"><span data-stu-id="efb92-135">id</span></span>|<span data-ttu-id="efb92-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="efb92-136">String</span></span>| <span data-ttu-id="efb92-p103">Уникальный идентификатор этих параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efb92-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="efb92-139">templateId</span><span class="sxs-lookup"><span data-stu-id="efb92-139">templateId</span></span>|<span data-ttu-id="efb92-140">String (строка)</span><span class="sxs-lookup"><span data-stu-id="efb92-140">String</span></span>| <span data-ttu-id="efb92-p104">Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="efb92-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="efb92-143">values</span><span class="sxs-lookup"><span data-stu-id="efb92-143">values</span></span>|<span data-ttu-id="efb92-144">Коллекция объектов [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="efb92-144">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="efb92-p105">Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="efb92-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="efb92-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="efb92-147">Relationships</span></span>

<span data-ttu-id="efb92-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="efb92-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efb92-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="efb92-149">JSON representation</span></span>

<span data-ttu-id="efb92-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efb92-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->