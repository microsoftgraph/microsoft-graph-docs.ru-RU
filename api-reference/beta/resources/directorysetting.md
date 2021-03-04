---
title: тип ресурса directorySetting
description: Параметры каталога можно создать на основе доступных directorySettingTemplates и изменить их по умолчанию.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440453"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="03c56-103">тип ресурса directorySetting</span><span class="sxs-lookup"><span data-stu-id="03c56-103">directorySetting resource type</span></span>

<span data-ttu-id="03c56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03c56-105">Параметры каталога могут быть созданы на основе доступных [directorySettingTemplates](directorysettingtemplate.md)и изменены по заранее.</span><span class="sxs-lookup"><span data-stu-id="03c56-105">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="03c56-106">Эти параметры могут управлять поведением сущности или функций как на уровне клиента, так и на определенном уровне объекта.</span><span class="sxs-lookup"><span data-stu-id="03c56-106">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="03c56-107">Если один и тот же параметр определяется как на уровне клиента, так и на уровне определенного объекта, определенный параметр уровня сущности может отказаться от параметра для всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="03c56-107">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="03c56-108">Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но определенный параметр группы может отказаться и не разрешит приглашать гостей членами группы.</span><span class="sxs-lookup"><span data-stu-id="03c56-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="03c56-109">В настоящее время параметры, определенные системой, регулируют только поведение групп Office.</span><span class="sxs-lookup"><span data-stu-id="03c56-109">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="03c56-110">**Примечание.** Бета-версия типа ресурса directorySetting применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="03c56-110">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="03c56-111">Версия /v1.0 переименована в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="03c56-111">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="03c56-112">Методы</span><span class="sxs-lookup"><span data-stu-id="03c56-112">Methods</span></span>

| <span data-ttu-id="03c56-113">Метод</span><span class="sxs-lookup"><span data-stu-id="03c56-113">Method</span></span>           | <span data-ttu-id="03c56-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03c56-114">Return Type</span></span>    |<span data-ttu-id="03c56-115">Описание</span><span class="sxs-lookup"><span data-stu-id="03c56-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="03c56-116">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="03c56-116">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="03c56-117">directorySetting</span><span class="sxs-lookup"><span data-stu-id="03c56-117">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="03c56-118">Создание объекта настройки на основе directorySettingTemplate.</span><span class="sxs-lookup"><span data-stu-id="03c56-118">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="03c56-119">Запрос POST должен предоставить параметрValues для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="03c56-119">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="03c56-120">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="03c56-120">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="03c56-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="03c56-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="03c56-122">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="03c56-122">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="03c56-123">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="03c56-123">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="03c56-124">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="03c56-124">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="03c56-125">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="03c56-125">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="03c56-126">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="03c56-126">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="03c56-127">directorySetting</span><span class="sxs-lookup"><span data-stu-id="03c56-127">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="03c56-128">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="03c56-128">Update a setting object.</span></span> <span data-ttu-id="03c56-129">В обновлении можно изменить только параметрValues.</span><span class="sxs-lookup"><span data-stu-id="03c56-129">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="03c56-130">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="03c56-130">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="03c56-131">Нет</span><span class="sxs-lookup"><span data-stu-id="03c56-131">None</span></span> |<span data-ttu-id="03c56-132">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="03c56-132">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="03c56-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="03c56-133">Properties</span></span>
| <span data-ttu-id="03c56-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="03c56-134">Property</span></span>     | <span data-ttu-id="03c56-135">Тип</span><span class="sxs-lookup"><span data-stu-id="03c56-135">Type</span></span>   |<span data-ttu-id="03c56-136">Описание</span><span class="sxs-lookup"><span data-stu-id="03c56-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03c56-137">displayName</span><span class="sxs-lookup"><span data-stu-id="03c56-137">displayName</span></span>|<span data-ttu-id="03c56-138">string</span><span class="sxs-lookup"><span data-stu-id="03c56-138">string</span></span>|<span data-ttu-id="03c56-139">Отображение имени этой группы параметров, которое происходит из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="03c56-139">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="03c56-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03c56-140">Read-only.</span></span>|
|<span data-ttu-id="03c56-141">id</span><span class="sxs-lookup"><span data-stu-id="03c56-141">id</span></span>|<span data-ttu-id="03c56-142">string</span><span class="sxs-lookup"><span data-stu-id="03c56-142">string</span></span>| <span data-ttu-id="03c56-143">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="03c56-143">Unique identifier for these settings.</span></span> <span data-ttu-id="03c56-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03c56-144">Read-only.</span></span>|
|<span data-ttu-id="03c56-145">templateId</span><span class="sxs-lookup"><span data-stu-id="03c56-145">templateId</span></span>|<span data-ttu-id="03c56-146">string</span><span class="sxs-lookup"><span data-stu-id="03c56-146">string</span></span>| <span data-ttu-id="03c56-147">Уникальный идентификатор для шаблона, используемого для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="03c56-147">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="03c56-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03c56-148">Read-only.</span></span>|
|<span data-ttu-id="03c56-149">values</span><span class="sxs-lookup"><span data-stu-id="03c56-149">values</span></span>|<span data-ttu-id="03c56-150">[settingValue](settingvalue.md) collection</span><span class="sxs-lookup"><span data-stu-id="03c56-150">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="03c56-151">Коллекция пар значений имен.</span><span class="sxs-lookup"><span data-stu-id="03c56-151">Collection of name value pairs.</span></span> <span data-ttu-id="03c56-152">Необходимо содержать и задать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="03c56-152">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03c56-153">Связи</span><span class="sxs-lookup"><span data-stu-id="03c56-153">Relationships</span></span>
<span data-ttu-id="03c56-154">Нет</span><span class="sxs-lookup"><span data-stu-id="03c56-154">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="03c56-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03c56-155">JSON representation</span></span>

<span data-ttu-id="03c56-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03c56-156">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


