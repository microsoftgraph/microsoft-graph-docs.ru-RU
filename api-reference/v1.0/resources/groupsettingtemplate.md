---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров групп представляют системные параметры, доступные для клиента. Параметры группы могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa392d6bf6dcd8ceaf15d97dfe695fbaaeabed4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531358"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="d9885-107">Тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d9885-107">groupSettingTemplate resource type</span></span>

<span data-ttu-id="d9885-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9885-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9885-109">Шаблоны параметров групп представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9885-109">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="d9885-110">[Параметры группы](groupsetting.md) могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются.</span><span class="sxs-lookup"><span data-stu-id="d9885-110">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="d9885-111">Шаблоны параметров групп не могут быть созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="d9885-111">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="d9885-112">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы.</span><span class="sxs-lookup"><span data-stu-id="d9885-112">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="d9885-113">В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="d9885-113">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="d9885-114">Методы</span><span class="sxs-lookup"><span data-stu-id="d9885-114">Methods</span></span>

| <span data-ttu-id="d9885-115">Метод</span><span class="sxs-lookup"><span data-stu-id="d9885-115">Method</span></span> | <span data-ttu-id="d9885-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9885-116">Return Type</span></span> | <span data-ttu-id="d9885-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d9885-117">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9885-118">Получение groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d9885-118">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="d9885-119">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d9885-119">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="d9885-120">Чтение определенных свойств одного из системных объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="d9885-120">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="d9885-121">Список groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d9885-121">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="d9885-122">Коллекция groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="d9885-122">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="d9885-123">Перечисление всех объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="d9885-123">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9885-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9885-124">Properties</span></span>

| <span data-ttu-id="d9885-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9885-125">Property</span></span> | <span data-ttu-id="d9885-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d9885-126">Type</span></span> | <span data-ttu-id="d9885-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d9885-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d9885-128">description</span><span class="sxs-lookup"><span data-stu-id="d9885-128">description</span></span>|<span data-ttu-id="d9885-129">String</span><span class="sxs-lookup"><span data-stu-id="d9885-129">String</span></span>| <span data-ttu-id="d9885-130">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="d9885-130">Description of the template.</span></span> |
|<span data-ttu-id="d9885-131">displayName</span><span class="sxs-lookup"><span data-stu-id="d9885-131">displayName</span></span>|<span data-ttu-id="d9885-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d9885-132">String</span></span>| <span data-ttu-id="d9885-133">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="d9885-133">Display name of the template.</span></span> |
|<span data-ttu-id="d9885-134">id</span><span class="sxs-lookup"><span data-stu-id="d9885-134">id</span></span>|<span data-ttu-id="d9885-135">String</span><span class="sxs-lookup"><span data-stu-id="d9885-135">String</span></span>| <span data-ttu-id="d9885-136">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="d9885-136">Unique identifier for the template.</span></span> <span data-ttu-id="d9885-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9885-137">Read-only.</span></span>|
|<span data-ttu-id="d9885-138">values</span><span class="sxs-lookup"><span data-stu-id="d9885-138">values</span></span>|<span data-ttu-id="d9885-139">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="d9885-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="d9885-140">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="d9885-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9885-141">Связи</span><span class="sxs-lookup"><span data-stu-id="d9885-141">Relationships</span></span>

<span data-ttu-id="d9885-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d9885-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d9885-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d9885-143">JSON representation</span></span>

<span data-ttu-id="d9885-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9885-144">Here is a JSON representation of the resource.</span></span>

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
