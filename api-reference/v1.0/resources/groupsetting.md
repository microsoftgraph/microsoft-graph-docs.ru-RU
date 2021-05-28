---
title: тип ресурса groupSetting
description: Параметры группы контролируют поведение, например заблокированные списки слов для имен отображения групп или разрешено ли гостевых пользователей быть владельцами групп.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1e18f78f0b0d7c9e8cb9c054afd5645ae45e1c48
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680880"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="74256-103">тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="74256-103">groupSetting resource type</span></span>

<span data-ttu-id="74256-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74256-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74256-105">Параметры группы контролируют поведение, например заблокированные списки слов для имен отображения групп или разрешено ли гостевых пользователей быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="74256-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="74256-106">Параметры группы можно создать на основе доступных [группSettingTemplates](groupsettingtemplate.md)и изменить их по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="74256-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="74256-107">Эти параметры регулируют групповое поведение на уровне клиента или определенной группе.</span><span class="sxs-lookup"><span data-stu-id="74256-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="74256-108">Если один и тот же параметр определяется как для клиента, так и для определенной группы, параметр группового уровня переопределяет параметр на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="74256-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="74256-109">Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но отдельные параметры группы могут переопределять и не разрешая приглашать гостей членами группы.</span><span class="sxs-lookup"><span data-stu-id="74256-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="74256-110">Параметры группы регулируют только поведение Microsoft 365 групп.</span><span class="sxs-lookup"><span data-stu-id="74256-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="74256-111">Методы</span><span class="sxs-lookup"><span data-stu-id="74256-111">Methods</span></span>

| <span data-ttu-id="74256-112">Метод</span><span class="sxs-lookup"><span data-stu-id="74256-112">Method</span></span> | <span data-ttu-id="74256-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74256-113">Return Type</span></span> | <span data-ttu-id="74256-114">Описание</span><span class="sxs-lookup"><span data-stu-id="74256-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="74256-115">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="74256-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="74256-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="74256-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="74256-117">Создание объекта настройки на основе groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="74256-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="74256-118">Запрос POST должен предоставить параметрValues для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="74256-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="74256-119">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="74256-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="74256-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="74256-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="74256-121">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="74256-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="74256-122">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="74256-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="74256-123">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="74256-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="74256-124">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="74256-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="74256-125">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="74256-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="74256-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="74256-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="74256-127">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="74256-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="74256-128">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="74256-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="74256-129">Нет</span><span class="sxs-lookup"><span data-stu-id="74256-129">None</span></span> | <span data-ttu-id="74256-130">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="74256-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74256-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="74256-131">Properties</span></span>

| <span data-ttu-id="74256-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="74256-132">Property</span></span> | <span data-ttu-id="74256-133">Тип</span><span class="sxs-lookup"><span data-stu-id="74256-133">Type</span></span> | <span data-ttu-id="74256-134">Описание</span><span class="sxs-lookup"><span data-stu-id="74256-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="74256-135">displayName</span><span class="sxs-lookup"><span data-stu-id="74256-135">displayName</span></span>|<span data-ttu-id="74256-136">String</span><span class="sxs-lookup"><span data-stu-id="74256-136">String</span></span>| <span data-ttu-id="74256-137">Отображение имени этой группы параметров, которое происходит из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="74256-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="74256-138">id</span><span class="sxs-lookup"><span data-stu-id="74256-138">id</span></span>|<span data-ttu-id="74256-139">String</span><span class="sxs-lookup"><span data-stu-id="74256-139">String</span></span>| <span data-ttu-id="74256-140">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="74256-140">Unique identifier for these settings.</span></span> <span data-ttu-id="74256-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74256-141">Read-only.</span></span> |
|<span data-ttu-id="74256-142">templateId</span><span class="sxs-lookup"><span data-stu-id="74256-142">templateId</span></span>|<span data-ttu-id="74256-143">String</span><span class="sxs-lookup"><span data-stu-id="74256-143">String</span></span>| <span data-ttu-id="74256-144">Уникальный идентификатор для шаблона, используемого для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="74256-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="74256-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74256-145">Read-only.</span></span> |
|<span data-ttu-id="74256-146">values</span><span class="sxs-lookup"><span data-stu-id="74256-146">values</span></span>|<span data-ttu-id="74256-147">[settingValue](settingvalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="74256-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="74256-148">Коллекция пар значений имен.</span><span class="sxs-lookup"><span data-stu-id="74256-148">Collection of name value pairs.</span></span> <span data-ttu-id="74256-149">Необходимо содержать и задать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="74256-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="74256-150">Связи</span><span class="sxs-lookup"><span data-stu-id="74256-150">Relationships</span></span>

<span data-ttu-id="74256-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74256-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74256-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74256-152">JSON representation</span></span>

<span data-ttu-id="74256-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74256-153">Here is a JSON representation of the resource.</span></span>

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

