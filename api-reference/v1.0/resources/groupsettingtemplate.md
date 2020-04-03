---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров групп представляют системные параметры, доступные для клиента.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a74999a29c32ac82dc568df593f6df5e8f925f1b
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124926"
---
# <a name="groupsettingtemplate-resource-type"></a><span data-ttu-id="a3146-103">Тип ресурса groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a3146-103">groupSettingTemplate resource type</span></span>

<span data-ttu-id="a3146-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3146-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3146-105">Шаблоны параметров групп представляют системные параметры, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3146-105">Group setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="a3146-106">[Параметры группы](groupsetting.md) могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются.</span><span class="sxs-lookup"><span data-stu-id="a3146-106">[Group settings](groupsetting.md) can be created based on the available **groupSettingTemplates**, and values changed from their preset defaults.</span></span> <span data-ttu-id="a3146-107">Шаблоны параметров групп не могут быть созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="a3146-107">Group setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="a3146-108">Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы.</span><span class="sxs-lookup"><span data-stu-id="a3146-108">These settings can represent tenant-wide settings, or can represent specific group settings.</span></span> <span data-ttu-id="a3146-109">В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.</span><span class="sxs-lookup"><span data-stu-id="a3146-109">Currently, the only templates available apply to Office 365 groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

## <a name="methods"></a><span data-ttu-id="a3146-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a3146-110">Methods</span></span>

| <span data-ttu-id="a3146-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a3146-111">Method</span></span> | <span data-ttu-id="a3146-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3146-112">Return Type</span></span> | <span data-ttu-id="a3146-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a3146-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3146-114">Получение groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a3146-114">Get groupSettingTemplate</span></span>](../api/groupsettingtemplate-get.md) | [<span data-ttu-id="a3146-115">groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a3146-115">groupSettingTemplate</span></span>](groupsettingtemplate.md) | <span data-ttu-id="a3146-116">Чтение определенных свойств одного из системных объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="a3146-116">Read the specific properties of one of the system defined groupSettingTemplate objects.</span></span> |
|[<span data-ttu-id="a3146-117">Список groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a3146-117">List groupSettingTemplate</span></span>](../api/groupsettingtemplate-list.md) | [<span data-ttu-id="a3146-118">Коллекция groupSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="a3146-118">Collection of groupSettingTemplate</span></span>](groupsettingtemplate.md) |<span data-ttu-id="a3146-119">Перечисление всех объектов groupSettingTemplate, определенных системой.</span><span class="sxs-lookup"><span data-stu-id="a3146-119">List all of the system defined groupSettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3146-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3146-120">Properties</span></span>

| <span data-ttu-id="a3146-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3146-121">Property</span></span> | <span data-ttu-id="a3146-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a3146-122">Type</span></span> | <span data-ttu-id="a3146-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a3146-123">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a3146-124">description</span><span class="sxs-lookup"><span data-stu-id="a3146-124">description</span></span>|<span data-ttu-id="a3146-125">String</span><span class="sxs-lookup"><span data-stu-id="a3146-125">String</span></span>| <span data-ttu-id="a3146-126">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="a3146-126">Description of the template.</span></span> |
|<span data-ttu-id="a3146-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a3146-127">displayName</span></span>|<span data-ttu-id="a3146-128">Строка</span><span class="sxs-lookup"><span data-stu-id="a3146-128">String</span></span>| <span data-ttu-id="a3146-129">Отображаемое имя шаблона.</span><span class="sxs-lookup"><span data-stu-id="a3146-129">Display name of the template.</span></span> |
|<span data-ttu-id="a3146-130">id</span><span class="sxs-lookup"><span data-stu-id="a3146-130">id</span></span>|<span data-ttu-id="a3146-131">String</span><span class="sxs-lookup"><span data-stu-id="a3146-131">String</span></span>| <span data-ttu-id="a3146-132">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="a3146-132">Unique identifier for the template.</span></span> <span data-ttu-id="a3146-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3146-133">Read-only.</span></span>|
|<span data-ttu-id="a3146-134">values</span><span class="sxs-lookup"><span data-stu-id="a3146-134">values</span></span>|<span data-ttu-id="a3146-135">Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)</span><span class="sxs-lookup"><span data-stu-id="a3146-135">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="a3146-136">Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="a3146-136">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3146-137">Связи</span><span class="sxs-lookup"><span data-stu-id="a3146-137">Relationships</span></span>

<span data-ttu-id="a3146-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a3146-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3146-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3146-139">JSON representation</span></span>

<span data-ttu-id="a3146-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3146-140">Here is a JSON representation of the resource.</span></span>

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
