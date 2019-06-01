---
title: Тип ресурса Директорисеттинг
description: Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес и заменены заданными по умолчанию стилями. Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов. Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы. Параметры, заданные в системе, управляют поведением групп Office.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3eccdb3b19acb286a8b67393f9a7b441b108627c
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657884"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="252d3-107">Тип ресурса Директорисеттинг</span><span class="sxs-lookup"><span data-stu-id="252d3-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="252d3-108">Параметры каталога могут быть созданы на основе доступных [директорисеттингтемплатес](directorysettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="252d3-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="252d3-109">Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов.</span><span class="sxs-lookup"><span data-stu-id="252d3-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="252d3-110">Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="252d3-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="252d3-111">Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы.</span><span class="sxs-lookup"><span data-stu-id="252d3-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="252d3-112">Параметры, заданные в системе, управляют поведением групп Office.</span><span class="sxs-lookup"><span data-stu-id="252d3-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="252d3-113">**Note**: версия/Beta типа ресурса директорисеттинг применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="252d3-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="252d3-114">Версия/v1.0 переименована в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="252d3-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="252d3-115">Методы</span><span class="sxs-lookup"><span data-stu-id="252d3-115">Methods</span></span>

| <span data-ttu-id="252d3-116">Метод</span><span class="sxs-lookup"><span data-stu-id="252d3-116">Method</span></span>           | <span data-ttu-id="252d3-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="252d3-117">Return Type</span></span>    |<span data-ttu-id="252d3-118">Описание</span><span class="sxs-lookup"><span data-stu-id="252d3-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="252d3-119">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="252d3-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="252d3-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="252d3-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="252d3-121">Создание объекта Setting на основе объекта Директорисеттингтемплате.</span><span class="sxs-lookup"><span data-stu-id="252d3-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="252d3-122">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="252d3-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="252d3-123">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="252d3-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="252d3-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="252d3-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="252d3-125">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="252d3-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="252d3-126">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="252d3-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="252d3-127">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="252d3-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="252d3-128">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="252d3-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="252d3-129">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="252d3-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="252d3-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="252d3-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="252d3-131">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="252d3-131">Update a setting object.</span></span> <span data-ttu-id="252d3-132">В обновлении можно изменить только Сеттингвалуес.</span><span class="sxs-lookup"><span data-stu-id="252d3-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="252d3-133">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="252d3-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="252d3-134">Нет</span><span class="sxs-lookup"><span data-stu-id="252d3-134">None</span></span> |<span data-ttu-id="252d3-135">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="252d3-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="252d3-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="252d3-136">Properties</span></span>
| <span data-ttu-id="252d3-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="252d3-137">Property</span></span>     | <span data-ttu-id="252d3-138">Тип</span><span class="sxs-lookup"><span data-stu-id="252d3-138">Type</span></span>   |<span data-ttu-id="252d3-139">Описание</span><span class="sxs-lookup"><span data-stu-id="252d3-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="252d3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="252d3-140">displayName</span></span>|<span data-ttu-id="252d3-141">string</span><span class="sxs-lookup"><span data-stu-id="252d3-141">string</span></span>|<span data-ttu-id="252d3-142">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="252d3-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="252d3-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="252d3-143">Read-only.</span></span>|
|<span data-ttu-id="252d3-144">id</span><span class="sxs-lookup"><span data-stu-id="252d3-144">id</span></span>|<span data-ttu-id="252d3-145">string</span><span class="sxs-lookup"><span data-stu-id="252d3-145">string</span></span>| <span data-ttu-id="252d3-146">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="252d3-146">Unique identifier for these settings.</span></span> <span data-ttu-id="252d3-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="252d3-147">Read-only.</span></span>|
|<span data-ttu-id="252d3-148">templateId</span><span class="sxs-lookup"><span data-stu-id="252d3-148">templateId</span></span>|<span data-ttu-id="252d3-149">string</span><span class="sxs-lookup"><span data-stu-id="252d3-149">string</span></span>| <span data-ttu-id="252d3-150">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="252d3-150">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="252d3-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="252d3-151">Read-only.</span></span>|
|<span data-ttu-id="252d3-152">values</span><span class="sxs-lookup"><span data-stu-id="252d3-152">values</span></span>|<span data-ttu-id="252d3-153">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="252d3-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="252d3-154">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="252d3-154">Collection of name value pairs.</span></span> <span data-ttu-id="252d3-155">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="252d3-155">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="252d3-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="252d3-156">Relationships</span></span>
<span data-ttu-id="252d3-157">Нет</span><span class="sxs-lookup"><span data-stu-id="252d3-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="252d3-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="252d3-158">JSON representation</span></span>

<span data-ttu-id="252d3-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="252d3-159">Here is a JSON representation of the resource.</span></span>

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
