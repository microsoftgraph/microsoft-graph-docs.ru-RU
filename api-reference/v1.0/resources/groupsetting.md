---
title: Тип ресурса groupSetting
description: Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42e6c0dc0f0ffd48da84023c5e4ff0d97cb446f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570829"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="6c241-103">Тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="6c241-103">groupSetting resource type</span></span>

<span data-ttu-id="6c241-104">Параметры группы, такие как заблокированные списки слов для отображаемых имен группы или, могут ли гостевые пользователи быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="6c241-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="6c241-105">Параметры группы могут быть созданы на основе доступных [граупсеттингтемплатес](groupsettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="6c241-105">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="6c241-106">Эти параметры определяют поведение групп на уровне клиента или в определенной группе.</span><span class="sxs-lookup"><span data-stu-id="6c241-106">These settings govern group behaviors at a tenant-wide level or to a specific group.</span></span> <span data-ttu-id="6c241-107">Если один и тот же параметр определен как на уровне клиента, так и в определенной группе, то настройка уровня группы переопределяет параметр на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="6c241-107">When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.</span></span>  <span data-ttu-id="6c241-108">Например, параметр на уровне клиента может разрешить гостям, которые будут приглашены существующими участниками группы, но параметр индивидуальной группы может переопределять и запрещать участникам группы приглашать гостей.</span><span class="sxs-lookup"><span data-stu-id="6c241-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="6c241-109">Параметры группы управляют поведением только групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="6c241-109">Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="6c241-110">Методы</span><span class="sxs-lookup"><span data-stu-id="6c241-110">Methods</span></span>

| <span data-ttu-id="6c241-111">Метод</span><span class="sxs-lookup"><span data-stu-id="6c241-111">Method</span></span> | <span data-ttu-id="6c241-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c241-112">Return Type</span></span> | <span data-ttu-id="6c241-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6c241-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6c241-114">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="6c241-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="6c241-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="6c241-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="6c241-116">Создание объекта Setting на основе объекта groupSettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="6c241-116">Create a setting object based on a groupSettingTemplate.</span></span> <span data-ttu-id="6c241-117">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="6c241-117">The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="6c241-118">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="6c241-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="6c241-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="6c241-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="6c241-120">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="6c241-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="6c241-121">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="6c241-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="6c241-122">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="6c241-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="6c241-123">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="6c241-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="6c241-124">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="6c241-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="6c241-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="6c241-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="6c241-126">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="6c241-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="6c241-127">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="6c241-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="6c241-128">Нет</span><span class="sxs-lookup"><span data-stu-id="6c241-128">None</span></span> | <span data-ttu-id="6c241-129">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="6c241-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6c241-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c241-130">Properties</span></span>

| <span data-ttu-id="6c241-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c241-131">Property</span></span> | <span data-ttu-id="6c241-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6c241-132">Type</span></span> | <span data-ttu-id="6c241-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6c241-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6c241-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6c241-134">displayName</span></span>|<span data-ttu-id="6c241-135">String</span><span class="sxs-lookup"><span data-stu-id="6c241-135">String</span></span>| <span data-ttu-id="6c241-136">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="6c241-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="6c241-137">id</span><span class="sxs-lookup"><span data-stu-id="6c241-137">id</span></span>|<span data-ttu-id="6c241-138">String</span><span class="sxs-lookup"><span data-stu-id="6c241-138">String</span></span>| <span data-ttu-id="6c241-139">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="6c241-139">Unique identifier for these settings.</span></span> <span data-ttu-id="6c241-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c241-140">Read-only.</span></span> |
|<span data-ttu-id="6c241-141">templateId</span><span class="sxs-lookup"><span data-stu-id="6c241-141">templateId</span></span>|<span data-ttu-id="6c241-142">String</span><span class="sxs-lookup"><span data-stu-id="6c241-142">String</span></span>| <span data-ttu-id="6c241-143">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="6c241-143">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="6c241-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c241-144">Read-only.</span></span> |
|<span data-ttu-id="6c241-145">values</span><span class="sxs-lookup"><span data-stu-id="6c241-145">values</span></span>|<span data-ttu-id="6c241-146">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6c241-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="6c241-147">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="6c241-147">Collection of name value pairs.</span></span> <span data-ttu-id="6c241-148">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="6c241-148">Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c241-149">Связи</span><span class="sxs-lookup"><span data-stu-id="6c241-149">Relationships</span></span>

<span data-ttu-id="6c241-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6c241-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c241-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c241-151">JSON representation</span></span>

<span data-ttu-id="6c241-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c241-152">Here is a JSON representation of the resource.</span></span>

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
