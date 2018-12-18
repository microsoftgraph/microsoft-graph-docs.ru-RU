---
title: Тип ресурса groupSetting
description: Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, а также разрешение или запрещение пользователям-гостям быть владельцами групп.
author: dkershaw10
ms.openlocfilehash: c4e3f92b96aa1be5088cace4adeef3ae33d968b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301150"
---
# <a name="groupsetting-resource-type"></a><span data-ttu-id="98570-103">Тип ресурса groupSetting</span><span class="sxs-lookup"><span data-stu-id="98570-103">groupSetting resource type</span></span>

<span data-ttu-id="98570-104">Параметры группы контролируют такое поведение, как обработка списков заблокированных слов для отображаемых имен группы, а также разрешение или запрещение пользователям-гостям быть владельцами групп.</span><span class="sxs-lookup"><span data-stu-id="98570-104">Group settings control behaviors such as blocked word lists for group display names or whether guest users are allowed to be group owners.</span></span>

<span data-ttu-id="98570-p101">Можно на базе доступных объектов [groupSettingTemplate](groupsettingtemplate.md) создавать параметры группы, а также менять предопределенные значения по умолчанию этих параметров. Они контролируют поведение групп на уровне клиента или отдельной группы. Если один и тот же параметр определен на двух уровнях — и клиента, и отдельной группы, параметр для группы переопределяет параметр для клиента.  Например, если получать приглашения от существующих членов групп разрешает пользователям параметр на уровне клиента, но запрещает параметр для отдельной группы, гости не смогут делать этого. Параметры группы контролируют только поведение групп Office 365.</span><span class="sxs-lookup"><span data-stu-id="98570-p101">Group settings can be created based on the available [groupSettingTemplates](groupsettingtemplate.md), and changed from their preset defaults. These settings govern group behaviors at a tenant-wide level or to a specific group. When the same setting is defined at both the tenant-wide and to a specific group, the group-level setting overrides the tenant-wide setting.  For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but an individual group setting can override and not allow guests to be invited by members of the group. Group settings only govern Office 365 groups behavior.</span></span>

## <a name="methods"></a><span data-ttu-id="98570-110">Методы</span><span class="sxs-lookup"><span data-stu-id="98570-110">Methods</span></span>

| <span data-ttu-id="98570-111">Метод</span><span class="sxs-lookup"><span data-stu-id="98570-111">Method</span></span> | <span data-ttu-id="98570-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98570-112">Return Type</span></span> | <span data-ttu-id="98570-113">Описание</span><span class="sxs-lookup"><span data-stu-id="98570-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="98570-114">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="98570-114">Create setting</span></span>](../api/groupsetting-post-groupsettings.md) | [<span data-ttu-id="98570-115">groupSetting</span><span class="sxs-lookup"><span data-stu-id="98570-115">groupSetting</span></span>](groupsetting.md) |<span data-ttu-id="98570-p102">Создание параметра объекта на базе groupSettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="98570-p102">Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template.</span></span> |
|[<span data-ttu-id="98570-118">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="98570-118">Get setting</span></span>](../api/groupsetting-get.md) | [<span data-ttu-id="98570-119">groupSetting</span><span class="sxs-lookup"><span data-stu-id="98570-119">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="98570-120">Считывание свойств определенного объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="98570-120">Read properties of a specific setting object.</span></span> |
|[<span data-ttu-id="98570-121">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="98570-121">List settings</span></span>](../api/groupsetting-list.md) | <span data-ttu-id="98570-122">Коллекция объектов [groupSetting](groupsetting.md)</span><span class="sxs-lookup"><span data-stu-id="98570-122">[groupSetting](groupsetting.md) collection</span></span> | <span data-ttu-id="98570-123">Перечисление свойств всех объектов параметра.</span><span class="sxs-lookup"><span data-stu-id="98570-123">List properties of all setting objects.</span></span> |
|[<span data-ttu-id="98570-124">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="98570-124">Update setting</span></span>](../api/groupsetting-update.md) | [<span data-ttu-id="98570-125">groupSetting</span><span class="sxs-lookup"><span data-stu-id="98570-125">groupSetting</span></span>](groupsetting.md) | <span data-ttu-id="98570-126">Обновление объекта groupsetting.</span><span class="sxs-lookup"><span data-stu-id="98570-126">Update groupsetting object.</span></span> |
|[<span data-ttu-id="98570-127">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="98570-127">Delete setting</span></span>](../api/groupsetting-delete.md) | <span data-ttu-id="98570-128">Нет</span><span class="sxs-lookup"><span data-stu-id="98570-128">None</span></span> | <span data-ttu-id="98570-129">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="98570-129">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="98570-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="98570-130">Properties</span></span>

| <span data-ttu-id="98570-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="98570-131">Property</span></span> | <span data-ttu-id="98570-132">Тип</span><span class="sxs-lookup"><span data-stu-id="98570-132">Type</span></span> | <span data-ttu-id="98570-133">Описание</span><span class="sxs-lookup"><span data-stu-id="98570-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="98570-134">displayName</span><span class="sxs-lookup"><span data-stu-id="98570-134">displayName</span></span>|<span data-ttu-id="98570-135">String</span><span class="sxs-lookup"><span data-stu-id="98570-135">String</span></span>| <span data-ttu-id="98570-136">Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="98570-136">Display name of this group of settings, which comes from the associated template.</span></span> |
|<span data-ttu-id="98570-137">id</span><span class="sxs-lookup"><span data-stu-id="98570-137">id</span></span>|<span data-ttu-id="98570-138">String</span><span class="sxs-lookup"><span data-stu-id="98570-138">String</span></span>| <span data-ttu-id="98570-p103">Уникальный идентификатор этих параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98570-p103">Unique identifier for these settings. Read-only.</span></span> |
|<span data-ttu-id="98570-141">templateId</span><span class="sxs-lookup"><span data-stu-id="98570-141">templateId</span></span>|<span data-ttu-id="98570-142">String</span><span class="sxs-lookup"><span data-stu-id="98570-142">String</span></span>| <span data-ttu-id="98570-p104">Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98570-p104">Unique identifier for the template used to create this group of settings. Read-only.</span></span> |
|<span data-ttu-id="98570-145">values</span><span class="sxs-lookup"><span data-stu-id="98570-145">values</span></span>|<span data-ttu-id="98570-146">Коллекция объектов [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="98570-146">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="98570-p105">Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="98570-p105">Collection of name value pairs. Must contain and set all the settings defined in the template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98570-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="98570-149">Relationships</span></span>

<span data-ttu-id="98570-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98570-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98570-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98570-151">JSON representation</span></span>

<span data-ttu-id="98570-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98570-152">Here is a JSON representation of the resource.</span></span>

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