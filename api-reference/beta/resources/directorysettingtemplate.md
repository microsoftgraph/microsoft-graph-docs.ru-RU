---
title: тип ресурса directorySettingTemplate
description: Шаблоны параметров каталогов представляют параметры, определяемые системой, доступные для клиента.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 71984d472aab9f78197134fae0668fd0a90d7716
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440411"
---
# <a name="directorysettingtemplate-resource-type"></a><span data-ttu-id="25872-103">тип ресурса directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="25872-103">directorySettingTemplate resource type</span></span>

<span data-ttu-id="25872-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25872-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25872-105">Шаблоны параметров каталогов представляют параметры, определяемые системой, доступные для клиента.</span><span class="sxs-lookup"><span data-stu-id="25872-105">Directory setting templates represent system-defined settings available to the tenant.</span></span> <span data-ttu-id="25872-106">[Параметры каталога](directorysetting.md) могут быть созданы на основе доступных directorySettingTemplates, а значения изменены по заранее.</span><span class="sxs-lookup"><span data-stu-id="25872-106">[Directory settings](directorysetting.md) can be created based on the available directorySettingTemplates, and values changed from their preset defaults.</span></span> <span data-ttu-id="25872-107">Шаблоны параметров каталога не могут быть созданы, обновлены или удалены.</span><span class="sxs-lookup"><span data-stu-id="25872-107">Directory setting templates cannot be created, updated or deleted.</span></span> <span data-ttu-id="25872-108">Эти параметры могут представлять параметры для клиента или представлять определенные параметры сущности.</span><span class="sxs-lookup"><span data-stu-id="25872-108">These settings can represent tenant-wide settings, or can represent specific entity settings.</span></span>  <span data-ttu-id="25872-109">В настоящее время только доступные шаблоны применяются к группам Office и включают параметры, например, могут ли пользователи создавать группы или приглашать гостей из-за пределов организации, чтобы стать членами группы.</span><span class="sxs-lookup"><span data-stu-id="25872-109">Currently, the only templates available apply to Office groups, and include settings such as whether users can create groups or invite guests from outside the organization to become members of a group.</span></span>

> <span data-ttu-id="25872-110">**Примечание.**/бета-версия типа ресурса directorySettingTemplate применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="25872-110">**Note**: The /beta version of the directorySettingTemplate resource type only applies to groups.</span></span> <span data-ttu-id="25872-111">Версия /v1.0 переименована в groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="25872-111">The /v1.0 version has been renamed to groupSettingTemplate.</span></span>

## <a name="methods"></a><span data-ttu-id="25872-112">Методы</span><span class="sxs-lookup"><span data-stu-id="25872-112">Methods</span></span>

| <span data-ttu-id="25872-113">Метод</span><span class="sxs-lookup"><span data-stu-id="25872-113">Method</span></span>           | <span data-ttu-id="25872-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25872-114">Return Type</span></span>    |<span data-ttu-id="25872-115">Описание</span><span class="sxs-lookup"><span data-stu-id="25872-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25872-116">Get directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="25872-116">Get directorySettingTemplate</span></span>](../api/directorysettingtemplate-get.md) | [<span data-ttu-id="25872-117">directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="25872-117">directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="25872-118">Ознакомьтесь с определенными свойствами одного из системных объектов directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="25872-118">Read the specific properties of one of the system defined directorySettingTemplate objects.</span></span>|
|[<span data-ttu-id="25872-119">Каталог listSettingTemplate</span><span class="sxs-lookup"><span data-stu-id="25872-119">List directorySettingTemplate</span></span>](../api/directorysettingtemplate-list.md) | [<span data-ttu-id="25872-120">Коллекция directorySettingTemplate</span><span class="sxs-lookup"><span data-stu-id="25872-120">Collection of directorySettingTemplate</span></span>](directorysettingtemplate.md) |<span data-ttu-id="25872-121">Список всех системных объектов directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="25872-121">List all of the system defined directorySettingTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="25872-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="25872-122">Properties</span></span>
| <span data-ttu-id="25872-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="25872-123">Property</span></span>     | <span data-ttu-id="25872-124">Тип</span><span class="sxs-lookup"><span data-stu-id="25872-124">Type</span></span>   |<span data-ttu-id="25872-125">Описание</span><span class="sxs-lookup"><span data-stu-id="25872-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25872-126">description</span><span class="sxs-lookup"><span data-stu-id="25872-126">description</span></span>|<span data-ttu-id="25872-127">string</span><span class="sxs-lookup"><span data-stu-id="25872-127">string</span></span>|<span data-ttu-id="25872-128">Описание шаблона.</span><span class="sxs-lookup"><span data-stu-id="25872-128">Description of the template.</span></span> <span data-ttu-id="25872-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25872-129">Read-only.</span></span>|
|<span data-ttu-id="25872-130">displayName</span><span class="sxs-lookup"><span data-stu-id="25872-130">displayName</span></span>|<span data-ttu-id="25872-131">string</span><span class="sxs-lookup"><span data-stu-id="25872-131">string</span></span>|<span data-ttu-id="25872-132">Отображение имени шаблона.</span><span class="sxs-lookup"><span data-stu-id="25872-132">Display name of the template.</span></span> <span data-ttu-id="25872-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25872-133">Read-only.</span></span> |
|<span data-ttu-id="25872-134">id</span><span class="sxs-lookup"><span data-stu-id="25872-134">id</span></span>|<span data-ttu-id="25872-135">string</span><span class="sxs-lookup"><span data-stu-id="25872-135">string</span></span>| <span data-ttu-id="25872-136">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="25872-136">Unique identifier for the template.</span></span> <span data-ttu-id="25872-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25872-137">Read-only.</span></span>|
|<span data-ttu-id="25872-138">values</span><span class="sxs-lookup"><span data-stu-id="25872-138">values</span></span>|<span data-ttu-id="25872-139">[settingTemplateValue](settingtemplatevalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="25872-139">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="25872-140">Коллекция параметровTemplateValues, которые перечисляют набор доступных параметров, по умолчанию и типов, которые составляют этот шаблон.</span><span class="sxs-lookup"><span data-stu-id="25872-140">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span>  <span data-ttu-id="25872-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25872-141">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25872-142">Связи</span><span class="sxs-lookup"><span data-stu-id="25872-142">Relationships</span></span>
<span data-ttu-id="25872-143">Нет</span><span class="sxs-lookup"><span data-stu-id="25872-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="25872-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25872-144">JSON representation</span></span>

<span data-ttu-id="25872-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25872-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


