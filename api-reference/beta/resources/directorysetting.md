---
title: Тип ресурса directorySetting
description: Параметры каталога можно основанного на доступные directorySettingTemplates и изменено с предварительно значения по умолчанию. Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности. Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.  Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы. В настоящее время системных параметров являются только влияет на поведение группы Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521371"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="9a6d4-107">Тип ресурса directorySetting</span><span class="sxs-lookup"><span data-stu-id="9a6d4-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a6d4-108">Параметры каталога можно основанного на доступные [directorySettingTemplates](directorysettingtemplate.md)и изменено с предварительно значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="9a6d4-109">Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="9a6d4-110">Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="9a6d4-111">Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="9a6d4-112">В настоящее время системных параметров являются только влияет на поведение группы Office.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="9a6d4-113">**Примечание**: версия /beta типа ресурса directorySetting применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="9a6d4-114">Версия /v1.0 переименовано в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="9a6d4-115">Методы</span><span class="sxs-lookup"><span data-stu-id="9a6d4-115">Methods</span></span>

| <span data-ttu-id="9a6d4-116">Метод</span><span class="sxs-lookup"><span data-stu-id="9a6d4-116">Method</span></span>           | <span data-ttu-id="9a6d4-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9a6d4-117">Return Type</span></span>    |<span data-ttu-id="9a6d4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9a6d4-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a6d4-119">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="9a6d4-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="9a6d4-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9a6d4-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9a6d4-121">Создание объекта setting на основе directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="9a6d4-122">POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="9a6d4-123">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="9a6d4-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="9a6d4-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9a6d4-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9a6d4-125">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="9a6d4-126">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="9a6d4-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="9a6d4-127">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="9a6d4-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="9a6d4-128">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="9a6d4-129">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="9a6d4-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="9a6d4-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9a6d4-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="9a6d4-131">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-131">Update a setting object.</span></span> <span data-ttu-id="9a6d4-132">Можно изменить только settingValues в обновление.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="9a6d4-133">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="9a6d4-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="9a6d4-134">Нет</span><span class="sxs-lookup"><span data-stu-id="9a6d4-134">None</span></span> |<span data-ttu-id="9a6d4-135">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a6d4-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a6d4-136">Properties</span></span>
| <span data-ttu-id="9a6d4-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a6d4-137">Property</span></span>     | <span data-ttu-id="9a6d4-138">Тип</span><span class="sxs-lookup"><span data-stu-id="9a6d4-138">Type</span></span>   |<span data-ttu-id="9a6d4-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9a6d4-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a6d4-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9a6d4-140">displayName</span></span>|<span data-ttu-id="9a6d4-141">строка</span><span class="sxs-lookup"><span data-stu-id="9a6d4-141">string</span></span>|<span data-ttu-id="9a6d4-142">Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="9a6d4-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-143">Read-only.</span></span>|
|<span data-ttu-id="9a6d4-144">id</span><span class="sxs-lookup"><span data-stu-id="9a6d4-144">id</span></span>|<span data-ttu-id="9a6d4-145">string</span><span class="sxs-lookup"><span data-stu-id="9a6d4-145">string</span></span>| <span data-ttu-id="9a6d4-p107">Уникальный идентификатор этих параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-p107">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="9a6d4-148">templateId</span><span class="sxs-lookup"><span data-stu-id="9a6d4-148">templateId</span></span>|<span data-ttu-id="9a6d4-149">string</span><span class="sxs-lookup"><span data-stu-id="9a6d4-149">string</span></span>| <span data-ttu-id="9a6d4-p108">Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-p108">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="9a6d4-152">values</span><span class="sxs-lookup"><span data-stu-id="9a6d4-152">values</span></span>|<span data-ttu-id="9a6d4-153">Коллекция объектов [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9a6d4-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="9a6d4-p109">Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-p109">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a6d4-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="9a6d4-156">Relationships</span></span>
<span data-ttu-id="9a6d4-157">Нет</span><span class="sxs-lookup"><span data-stu-id="9a6d4-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9a6d4-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a6d4-158">JSON representation</span></span>

<span data-ttu-id="9a6d4-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a6d4-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
