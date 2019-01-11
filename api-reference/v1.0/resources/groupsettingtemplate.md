---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров группы представляют определенные системой параметры для клиента. Можно на базе доступных объектов groupSettingTemplate создавать **параметры группы**, а также менять предопределенные значения по умолчанию этих параметров. Шаблоны параметров группы невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или отдельной группы. На данный момент доступны только шаблоны, применимые к группам Office 365 и включающие параметры, которые, например, разрешают или запрещают пользователям создавать группы либо приглашать внешних гостей в группу.
localization_priority: Normal
ms.openlocfilehash: c2e6b465226b8c1c69438fab37d874735e89ac52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859348"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="b271f-107">Тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b271f-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="b271f-p102">Шаблоны параметров группы представляют определенные системой параметры для клиента. Можно на базе доступных объектов **groupSettingTemplate** создавать [параметры группы](groupsetting.md), а также менять предопределенные значения по умолчанию этих параметров. Шаблоны параметров группы невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или отдельной группы. На данный момент доступны только шаблоны, применимые к группам Office 365 и включающие параметры, которые, например, разрешают или запрещают пользователям создавать группы либо приглашать внешних гостей в группу.</span><span class="sxs-lookup"><span data-stu-id="b271f-p102">Group setting templates represent system-defined settings available to the tenant. [Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults. Group setting templates cannot be created, updated or deleted. These settings can represent tenant-wide settings, or can represent specific group settings. Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="b271f-113">Методы</span><span class="sxs-lookup"><span data-stu-id="b271f-113">Methods</span></span>

| <span data-ttu-id="b271f-114">Метод</span><span class="sxs-lookup"><span data-stu-id="b271f-114">Method</span></span> | <span data-ttu-id="b271f-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b271f-115">Return Type</span></span> | <span data-ttu-id="b271f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b271f-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b271f-117">Получение groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b271f-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="b271f-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b271f-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="b271f-119">Считывание конкретных свойств одного из определенных системой объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="b271f-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="b271f-120">Перечисление groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b271f-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="b271f-121">Коллекция объектов groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="b271f-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="b271f-122">Перечисление всех определенных системой объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="b271f-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="b271f-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="b271f-123">Properties</span></span>

| <span data-ttu-id="b271f-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="b271f-124">Property</span></span> | <span data-ttu-id="b271f-125">Тип</span><span class="sxs-lookup"><span data-stu-id="b271f-125">Type</span></span> | <span data-ttu-id="b271f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b271f-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b271f-127">описание</span><span class="sxs-lookup"><span data-stu-id="b271f-127">description</span></span>|<span data-ttu-id="b271f-128">String</span><span class="sxs-lookup"><span data-stu-id="b271f-128">String</span></span>| <span data-ttu-id="b271f-129">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="b271f-129">Description of the template.</span></span> |
|<span data-ttu-id="b271f-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b271f-130">displayName</span></span>|<span data-ttu-id="b271f-131">String</span><span class="sxs-lookup"><span data-stu-id="b271f-131">String</span></span>| <span data-ttu-id="b271f-132">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="b271f-132">Display name of the template.</span></span> |
|<span data-ttu-id="b271f-133">id</span><span class="sxs-lookup"><span data-stu-id="b271f-133">id</span></span>|<span data-ttu-id="b271f-134">String</span><span class="sxs-lookup"><span data-stu-id="b271f-134">String</span></span>| <span data-ttu-id="b271f-p103">Уникальный идентификатор шаблона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b271f-p103">Unique identifier for the template. Read-only.</span></span>|
|<span data-ttu-id="b271f-137">values</span><span class="sxs-lookup"><span data-stu-id="b271f-137">values</span></span>|<span data-ttu-id="b271f-138">Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="b271f-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="b271f-139">Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.</span><span class="sxs-lookup"><span data-stu-id="b271f-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b271f-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="b271f-140">Relationships</span></span>

<span data-ttu-id="b271f-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b271f-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b271f-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b271f-142">JSON representation</span></span>

<span data-ttu-id="b271f-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b271f-143">Here is a JSON representation of the resource.</span></span>

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
