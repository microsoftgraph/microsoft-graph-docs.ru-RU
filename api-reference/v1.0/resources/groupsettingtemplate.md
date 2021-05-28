---
title: тип ресурса groupSettingTemplate
description: Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a7868538c13b1e386e7aa10dcdf3fed9c03b198f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680873"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="84a47-103">тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84a47-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="84a47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84a47-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84a47-105">Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="84a47-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="84a47-106">[Параметры группы](groupsetting.md) могут быть созданы на основе доступных **группSettingTemplates** и значений, измененных по заранее.</span><span class="sxs-lookup"><span data-stu-id="84a47-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="84a47-107">Шаблоны параметров группы не могут быть созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="84a47-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="84a47-108">Эти параметры могут представлять параметры для клиента или представлять определенные параметры группы.</span><span class="sxs-lookup"><span data-stu-id="84a47-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="84a47-109">В настоящее время только доступные шаблоны применяются к Microsoft 365 группам и включают параметры, например, могут ли пользователи создавать группы или приглашать гостей из-за пределов организации в члены группы.</span><span class="sxs-lookup"><span data-stu-id="84a47-109">Currently, the only templates available apply to Microsoft 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="84a47-110">Методы</span><span class="sxs-lookup"><span data-stu-id="84a47-110">Methods</span></span>

| <span data-ttu-id="84a47-111">Метод</span><span class="sxs-lookup"><span data-stu-id="84a47-111">Method</span></span> | <span data-ttu-id="84a47-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84a47-112">Return Type</span></span> | <span data-ttu-id="84a47-113">Описание</span><span class="sxs-lookup"><span data-stu-id="84a47-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="84a47-114">Get groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84a47-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="84a47-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84a47-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="84a47-116">Ознакомьтесь с определенными свойствами одного из системных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="84a47-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="84a47-117">List groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84a47-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="84a47-118">Коллекция groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="84a47-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="84a47-119">Список всех системных объектов groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="84a47-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="84a47-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="84a47-120">Properties</span></span>

| <span data-ttu-id="84a47-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="84a47-121">Property</span></span> | <span data-ttu-id="84a47-122">Тип</span><span class="sxs-lookup"><span data-stu-id="84a47-122">Type</span></span> | <span data-ttu-id="84a47-123">Описание</span><span class="sxs-lookup"><span data-stu-id="84a47-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="84a47-124">description</span><span class="sxs-lookup"><span data-stu-id="84a47-124">description</span></span>|<span data-ttu-id="84a47-125">String</span><span class="sxs-lookup"><span data-stu-id="84a47-125">String</span></span>| <span data-ttu-id="84a47-126">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="84a47-126">Description of the template.</span></span> |
|<span data-ttu-id="84a47-127">displayName</span><span class="sxs-lookup"><span data-stu-id="84a47-127">displayName</span></span>|<span data-ttu-id="84a47-128">String</span><span class="sxs-lookup"><span data-stu-id="84a47-128">String</span></span>| <span data-ttu-id="84a47-129">Отображение имени шаблона.</span><span class="sxs-lookup"><span data-stu-id="84a47-129">Display name of the template.</span></span> |
|<span data-ttu-id="84a47-130">id</span><span class="sxs-lookup"><span data-stu-id="84a47-130">id</span></span>|<span data-ttu-id="84a47-131">String</span><span class="sxs-lookup"><span data-stu-id="84a47-131">String</span></span>| <span data-ttu-id="84a47-132">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="84a47-132">Unique identifier for the template.</span></span> <span data-ttu-id="84a47-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84a47-133">Read-only.</span></span>|
|<span data-ttu-id="84a47-134">values</span><span class="sxs-lookup"><span data-stu-id="84a47-134">values</span></span>|<span data-ttu-id="84a47-135">[settingTemplateValue](settingtemplatevalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="84a47-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="84a47-136">Коллекция параметровTemplateValues, которые перечисляют набор доступных параметров, по умолчанию и типов, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="84a47-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84a47-137">Связи</span><span class="sxs-lookup"><span data-stu-id="84a47-137">Relationships</span></span>

<span data-ttu-id="84a47-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84a47-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="84a47-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="84a47-139">JSON representation</span></span>

<span data-ttu-id="84a47-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84a47-140">Here is a JSON representation of the resource.</span></span>

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

