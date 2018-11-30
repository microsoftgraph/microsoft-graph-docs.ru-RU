---
title: Тип ресурса directorySetting
description: Параметры каталога можно основанного на доступные directorySettingTemplates и изменено с предварительно значения по умолчанию. Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности. Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.  Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы. В настоящее время системных параметров являются только влияет на поведение группы Office.
ms.openlocfilehash: 4a807d22bfd5d6651b4064542d33fe285b637a3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078451"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="1f025-107">Тип ресурса directorySetting</span><span class="sxs-lookup"><span data-stu-id="1f025-107">directorySetting resource type</span></span>

> <span data-ttu-id="1f025-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f025-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f025-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f025-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f025-110">Параметры каталога можно основанного на доступные [directorySettingTemplates](directorysettingtemplate.md)и изменено с предварительно значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1f025-110">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="1f025-111">Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности.</span><span class="sxs-lookup"><span data-stu-id="1f025-111">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="1f025-112">Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1f025-112">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="1f025-113">Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы.</span><span class="sxs-lookup"><span data-stu-id="1f025-113">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="1f025-114">В настоящее время системных параметров являются только влияет на поведение группы Office.</span><span class="sxs-lookup"><span data-stu-id="1f025-114">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="1f025-115">**Примечание**: версия /beta типа ресурса directorySetting применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="1f025-115">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="1f025-116">Версия /v1.0 переименовано в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="1f025-116">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="1f025-117">Методы</span><span class="sxs-lookup"><span data-stu-id="1f025-117">Methods</span></span>

| <span data-ttu-id="1f025-118">Метод</span><span class="sxs-lookup"><span data-stu-id="1f025-118">Method</span></span>           | <span data-ttu-id="1f025-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f025-119">Return Type</span></span>    |<span data-ttu-id="1f025-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f025-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f025-121">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="1f025-121">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="1f025-122">directorySetting</span><span class="sxs-lookup"><span data-stu-id="1f025-122">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="1f025-123">Создайте объект параметр на основании directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="1f025-123">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="1f025-124">Запрос POST необходимо задать settingValues для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="1f025-124">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="1f025-125">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="1f025-125">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="1f025-126">directorySetting</span><span class="sxs-lookup"><span data-stu-id="1f025-126">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="1f025-127">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="1f025-127">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="1f025-128">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="1f025-128">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="1f025-129">[directorySetting](directorysetting.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1f025-129">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="1f025-130">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="1f025-130">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="1f025-131">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="1f025-131">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="1f025-132">directorySetting</span><span class="sxs-lookup"><span data-stu-id="1f025-132">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="1f025-133">Обновление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="1f025-133">Update a setting object.</span></span> <span data-ttu-id="1f025-134">Можно изменить только settingValues в обновление.</span><span class="sxs-lookup"><span data-stu-id="1f025-134">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="1f025-135">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="1f025-135">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="1f025-136">Нет</span><span class="sxs-lookup"><span data-stu-id="1f025-136">None</span></span> |<span data-ttu-id="1f025-137">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="1f025-137">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f025-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f025-138">Properties</span></span>
| <span data-ttu-id="1f025-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f025-139">Property</span></span>     | <span data-ttu-id="1f025-140">Тип</span><span class="sxs-lookup"><span data-stu-id="1f025-140">Type</span></span>   |<span data-ttu-id="1f025-141">Описание</span><span class="sxs-lookup"><span data-stu-id="1f025-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f025-142">displayName</span><span class="sxs-lookup"><span data-stu-id="1f025-142">displayName</span></span>|<span data-ttu-id="1f025-143">строка</span><span class="sxs-lookup"><span data-stu-id="1f025-143">string</span></span>|<span data-ttu-id="1f025-144">Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="1f025-144">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="1f025-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f025-145">Read-only.</span></span>|
|<span data-ttu-id="1f025-146">id</span><span class="sxs-lookup"><span data-stu-id="1f025-146">id</span></span>|<span data-ttu-id="1f025-147">строка</span><span class="sxs-lookup"><span data-stu-id="1f025-147">string</span></span>| <span data-ttu-id="1f025-p108">Уникальный идентификатор этих параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f025-p108">Unique identifier for these settings. Read-only.</span></span>|
|<span data-ttu-id="1f025-150">templateId</span><span class="sxs-lookup"><span data-stu-id="1f025-150">templateId</span></span>|<span data-ttu-id="1f025-151">string</span><span class="sxs-lookup"><span data-stu-id="1f025-151">string</span></span>| <span data-ttu-id="1f025-p109">Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f025-p109">Unique identifier for the template used to create this group of settings. Read-only.</span></span>|
|<span data-ttu-id="1f025-154">values</span><span class="sxs-lookup"><span data-stu-id="1f025-154">values</span></span>|<span data-ttu-id="1f025-155">Коллекция объектов [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1f025-155">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="1f025-p110">Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="1f025-p110">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f025-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f025-158">Relationships</span></span>
<span data-ttu-id="1f025-159">Нет</span><span class="sxs-lookup"><span data-stu-id="1f025-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1f025-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f025-160">JSON representation</span></span>

<span data-ttu-id="1f025-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f025-161">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->