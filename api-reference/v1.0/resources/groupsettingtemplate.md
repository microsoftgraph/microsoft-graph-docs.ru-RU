---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров групп представляют системные параметры, доступные для клиента. Параметры группы могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d0624be1511b542da08e76ed5f9c51e60fe58a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029283"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="193d7-107">Тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="193d7-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="193d7-108">Шаблоны параметров групп представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="193d7-108">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="193d7-109">[Параметры группы](groupsetting.md) могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются.</span><span class="sxs-lookup"><span data-stu-id="193d7-109">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="193d7-110">Шаблоны параметров групп не могут быть созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="193d7-110">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="193d7-111">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы.</span><span class="sxs-lookup"><span data-stu-id="193d7-111">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="193d7-112">В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="193d7-112">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="193d7-113">Методы</span><span class="sxs-lookup"><span data-stu-id="193d7-113">Methods</span></span>

| <span data-ttu-id="193d7-114">Метод</span><span class="sxs-lookup"><span data-stu-id="193d7-114">Method</span></span> | <span data-ttu-id="193d7-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="193d7-115">Return Type</span></span> | <span data-ttu-id="193d7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="193d7-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="193d7-117">Получение groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="193d7-117">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="193d7-118">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="193d7-118">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="193d7-119">Чтение определенных свойств одного из системных объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="193d7-119">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="193d7-120">Список groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="193d7-120">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="193d7-121">Коллекция groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="193d7-121">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="193d7-122">Перечисление всех объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="193d7-122">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="193d7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="193d7-123">Properties</span></span>

| <span data-ttu-id="193d7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="193d7-124">Property</span></span> | <span data-ttu-id="193d7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="193d7-125">Type</span></span> | <span data-ttu-id="193d7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="193d7-126">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="193d7-127">description</span><span class="sxs-lookup"><span data-stu-id="193d7-127">description</span></span>|<span data-ttu-id="193d7-128">String</span><span class="sxs-lookup"><span data-stu-id="193d7-128">String</span></span>| <span data-ttu-id="193d7-129">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="193d7-129">Description of the template.</span></span> |
|<span data-ttu-id="193d7-130">displayName</span><span class="sxs-lookup"><span data-stu-id="193d7-130">displayName</span></span>|<span data-ttu-id="193d7-131">Строка</span><span class="sxs-lookup"><span data-stu-id="193d7-131">String</span></span>| <span data-ttu-id="193d7-132">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="193d7-132">Display name of the template.</span></span> |
|<span data-ttu-id="193d7-133">id</span><span class="sxs-lookup"><span data-stu-id="193d7-133">id</span></span>|<span data-ttu-id="193d7-134">String</span><span class="sxs-lookup"><span data-stu-id="193d7-134">String</span></span>| <span data-ttu-id="193d7-135">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="193d7-135">Unique identifier for the template.</span></span> <span data-ttu-id="193d7-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="193d7-136">Read-only.</span></span>|
|<span data-ttu-id="193d7-137">values</span><span class="sxs-lookup"><span data-stu-id="193d7-137">values</span></span>|<span data-ttu-id="193d7-138">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="193d7-138">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="193d7-139">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="193d7-139">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="193d7-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="193d7-140">Relationships</span></span>

<span data-ttu-id="193d7-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="193d7-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="193d7-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="193d7-142">JSON representation</span></span>

<span data-ttu-id="193d7-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="193d7-143">Here is a JSON representation of the resource.</span></span>

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
