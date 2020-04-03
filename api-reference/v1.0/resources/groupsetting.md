---
title: Тип ресурса groupSetting
description: Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 5e8e890e03a3af81a7fcdbdf5c86e203ae702e81
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125010"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="81c19-103">Тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="81c19-103">groupSetting resource type</span></span>

<span data-ttu-id="81c19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81c19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81c19-105">Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="81c19-105">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="81c19-106">Параметры группы могут быть созданы на основе доступных [граупсеттингтемплатес](groupsettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="81c19-106">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="81c19-107">Эти параметры определяют поведение групп на уровне клиента или в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="81c19-107">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="81c19-108">Если один и тот же параметр определен как на уровне клиента, так и в определенной группе, то настройка уровня группы переопределяет параметр на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="81c19-108">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="81c19-109">Например, параметр на уровне клиента может разрешить гостям, которые будут приглашены существующими участниками группы, но параметр индивидуальной группы может переопределять и запрещать участникам группы приглашать гостей.</span><span class="sxs-lookup"><span data-stu-id="81c19-109">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="81c19-110">Параметры группы управляют поведением только групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="81c19-110">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="81c19-111">Методы</span><span class="sxs-lookup"><span data-stu-id="81c19-111">Methods</span></span>

| <span data-ttu-id="81c19-112">Метод</span><span class="sxs-lookup"><span data-stu-id="81c19-112">Method</span></span> | <span data-ttu-id="81c19-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81c19-113">Return Type</span></span> | <span data-ttu-id="81c19-114">Описание</span><span class="sxs-lookup"><span data-stu-id="81c19-114">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="81c19-115">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="81c19-115">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="81c19-116">groupSetting</span><span class="sxs-lookup"><span data-stu-id="81c19-116">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="81c19-117">Создание объекта Setting на основе объекта groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="81c19-117">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="81c19-118">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="81c19-118">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="81c19-119">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="81c19-119">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="81c19-120">groupSetting</span><span class="sxs-lookup"><span data-stu-id="81c19-120">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="81c19-121">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="81c19-121">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="81c19-122">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="81c19-122">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="81c19-123">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="81c19-123">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="81c19-124">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="81c19-124">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="81c19-125">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="81c19-125">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="81c19-126">groupSetting</span><span class="sxs-lookup"><span data-stu-id="81c19-126">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="81c19-127">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="81c19-127">Update groupsetting object.</span></span> |
|[<span data-ttu-id="81c19-128">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="81c19-128">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="81c19-129">Нет</span><span class="sxs-lookup"><span data-stu-id="81c19-129">None</span></span> | <span data-ttu-id="81c19-130">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="81c19-130">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="81c19-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="81c19-131">Properties</span></span>

| <span data-ttu-id="81c19-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="81c19-132">Property</span></span> | <span data-ttu-id="81c19-133">Тип</span><span class="sxs-lookup"><span data-stu-id="81c19-133">Type</span></span> | <span data-ttu-id="81c19-134">Описание</span><span class="sxs-lookup"><span data-stu-id="81c19-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="81c19-135">displayName</span><span class="sxs-lookup"><span data-stu-id="81c19-135">displayName</span></span>|<span data-ttu-id="81c19-136">Строка</span><span class="sxs-lookup"><span data-stu-id="81c19-136">String</span></span>| <span data-ttu-id="81c19-137">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="81c19-137">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="81c19-138">id</span><span class="sxs-lookup"><span data-stu-id="81c19-138">id</span></span>|<span data-ttu-id="81c19-139">String</span><span class="sxs-lookup"><span data-stu-id="81c19-139">String</span></span>| <span data-ttu-id="81c19-140">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="81c19-140">Unique identifier for these settings.</span></span> <span data-ttu-id="81c19-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81c19-141">Read-only.</span></span> |
|<span data-ttu-id="81c19-142">templateId</span><span class="sxs-lookup"><span data-stu-id="81c19-142">templateId</span></span>|<span data-ttu-id="81c19-143">Строка</span><span class="sxs-lookup"><span data-stu-id="81c19-143">String</span></span>| <span data-ttu-id="81c19-144">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="81c19-144">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="81c19-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81c19-145">Read-only.</span></span> |
|<span data-ttu-id="81c19-146">values</span><span class="sxs-lookup"><span data-stu-id="81c19-146">values</span></span>|<span data-ttu-id="81c19-147">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="81c19-147">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="81c19-148">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="81c19-148">Collection of name value pairs.</span></span> <span data-ttu-id="81c19-149">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="81c19-149">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="81c19-150">Связи</span><span class="sxs-lookup"><span data-stu-id="81c19-150">Relationships</span></span>

<span data-ttu-id="81c19-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="81c19-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81c19-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="81c19-152">JSON representation</span></span>

<span data-ttu-id="81c19-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81c19-153">Here is a JSON representation of the resource.</span></span>

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
