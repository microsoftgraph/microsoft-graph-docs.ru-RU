---
title: Тип ресурса groupSetting
description: Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5dc427dc2ea2bf4e47d101ded89fdfa819d678ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062948"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="d4ace-103">Тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="d4ace-103">groupSetting resource type</span></span>

<span data-ttu-id="d4ace-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4ace-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4ace-105">Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="d4ace-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="d4ace-106">Параметры группы могут быть созданы на основе доступных [граупсеттингтемплатес](groupsettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="d4ace-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="d4ace-107">Эти параметры определяют поведение групп на уровне клиента или в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="d4ace-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="d4ace-108">Если один и тот же параметр определен как на уровне клиента, так и в определенной группе, то настройка уровня группы переопределяет параметр на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="d4ace-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="d4ace-109">Например, параметр на уровне клиента может разрешить гостям, которые будут приглашены существующими участниками группы, но параметр индивидуальной группы может переопределять и запрещать участникам группы приглашать гостей.</span><span class="sxs-lookup"><span data-stu-id="d4ace-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="d4ace-110">Параметры группы управляют только поведением групп Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d4ace-110">Group settings only govern Microsoft 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="d4ace-111">Методы</span><span class="sxs-lookup"><span data-stu-id="d4ace-111">Methods</span></span>

| <span data-ttu-id="d4ace-112">Метод</span><span class="sxs-lookup"><span data-stu-id="d4ace-112">Method</span></span> | <span data-ttu-id="d4ace-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4ace-113">Return Type</span></span> | <span data-ttu-id="d4ace-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ace-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4ace-115">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="d4ace-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="d4ace-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d4ace-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="d4ace-117">Создание объекта Setting на основе объекта groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="d4ace-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="d4ace-118">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="d4ace-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="d4ace-119">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="d4ace-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="d4ace-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d4ace-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="d4ace-121">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="d4ace-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="d4ace-122">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="d4ace-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="d4ace-123">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="d4ace-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="d4ace-124">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="d4ace-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="d4ace-125">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="d4ace-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="d4ace-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="d4ace-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="d4ace-127">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="d4ace-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="d4ace-128">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="d4ace-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="d4ace-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d4ace-129">None</span></span> | <span data-ttu-id="d4ace-130">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="d4ace-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4ace-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4ace-131">Properties</span></span>

| <span data-ttu-id="d4ace-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4ace-132">Property</span></span> | <span data-ttu-id="d4ace-133">Тип</span><span class="sxs-lookup"><span data-stu-id="d4ace-133">Type</span></span> | <span data-ttu-id="d4ace-134">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ace-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4ace-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4ace-135">displayName</span></span>|<span data-ttu-id="d4ace-136">String</span><span class="sxs-lookup"><span data-stu-id="d4ace-136">String</span></span>| <span data-ttu-id="d4ace-137">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="d4ace-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="d4ace-138">id</span><span class="sxs-lookup"><span data-stu-id="d4ace-138">id</span></span>|<span data-ttu-id="d4ace-139">String</span><span class="sxs-lookup"><span data-stu-id="d4ace-139">String</span></span>| <span data-ttu-id="d4ace-140">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="d4ace-140">Unique identifier for these settings.</span></span> <span data-ttu-id="d4ace-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4ace-141">Read-only.</span></span> |
|<span data-ttu-id="d4ace-142">templateId</span><span class="sxs-lookup"><span data-stu-id="d4ace-142">templateId</span></span>|<span data-ttu-id="d4ace-143">String</span><span class="sxs-lookup"><span data-stu-id="d4ace-143">String</span></span>| <span data-ttu-id="d4ace-144">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="d4ace-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="d4ace-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4ace-145">Read-only.</span></span> |
|<span data-ttu-id="d4ace-146">values</span><span class="sxs-lookup"><span data-stu-id="d4ace-146">values</span></span>|<span data-ttu-id="d4ace-147">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d4ace-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="d4ace-148">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="d4ace-148">Collection of name value pairs.</span></span> <span data-ttu-id="d4ace-149">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="d4ace-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4ace-150">Связи</span><span class="sxs-lookup"><span data-stu-id="d4ace-150">Relationships</span></span>

<span data-ttu-id="d4ace-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d4ace-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4ace-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4ace-152">JSON representation</span></span>

<span data-ttu-id="d4ace-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4ace-153">Here is a JSON representation of the resource.</span></span>

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

