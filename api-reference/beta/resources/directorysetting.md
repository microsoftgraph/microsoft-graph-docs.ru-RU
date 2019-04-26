---
title: Тип ресурса Директорисеттинг
description: Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес и заменены заданными по умолчанию стилями. Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов. Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы. Параметры, заданные в системе, управляют поведением групп Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3336ec351c44ba0b69df55e1383cca73b6ea1a96
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340744"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="48f82-107">Тип ресурса Директорисеттинг</span><span class="sxs-lookup"><span data-stu-id="48f82-107">directorySetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f82-108">Параметры каталога могут быть созданы на основе доступных [директорисеттингтемплатес](directorysettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="48f82-108">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="48f82-109">Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов.</span><span class="sxs-lookup"><span data-stu-id="48f82-109">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="48f82-110">Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="48f82-110">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="48f82-111">Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы.</span><span class="sxs-lookup"><span data-stu-id="48f82-111">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="48f82-112">Параметры, заданные в системе, управляют поведением групп Office.</span><span class="sxs-lookup"><span data-stu-id="48f82-112">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="48f82-113">**Note**: версия/Beta типа ресурса директорисеттинг применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="48f82-113">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="48f82-114">Версия/v1.0 переименована в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="48f82-114">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="48f82-115">Методы</span><span class="sxs-lookup"><span data-stu-id="48f82-115">Methods</span></span>

| <span data-ttu-id="48f82-116">Метод</span><span class="sxs-lookup"><span data-stu-id="48f82-116">Method</span></span>           | <span data-ttu-id="48f82-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48f82-117">Return Type</span></span>    |<span data-ttu-id="48f82-118">Описание</span><span class="sxs-lookup"><span data-stu-id="48f82-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48f82-119">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="48f82-119">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="48f82-120">directorySetting</span><span class="sxs-lookup"><span data-stu-id="48f82-120">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="48f82-121">Создание объекта Setting на основе объекта Директорисеттингтемплате.</span><span class="sxs-lookup"><span data-stu-id="48f82-121">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="48f82-122">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="48f82-122">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="48f82-123">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="48f82-123">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="48f82-124">directorySetting</span><span class="sxs-lookup"><span data-stu-id="48f82-124">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="48f82-125">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="48f82-125">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="48f82-126">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="48f82-126">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="48f82-127">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="48f82-127">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="48f82-128">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="48f82-128">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="48f82-129">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="48f82-129">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="48f82-130">directorySetting</span><span class="sxs-lookup"><span data-stu-id="48f82-130">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="48f82-131">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="48f82-131">Update a setting object.</span></span> <span data-ttu-id="48f82-132">В обновлении можно изменить только Сеттингвалуес.</span><span class="sxs-lookup"><span data-stu-id="48f82-132">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="48f82-133">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="48f82-133">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="48f82-134">Нет</span><span class="sxs-lookup"><span data-stu-id="48f82-134">None</span></span> |<span data-ttu-id="48f82-135">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="48f82-135">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="48f82-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="48f82-136">Properties</span></span>
| <span data-ttu-id="48f82-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="48f82-137">Property</span></span>     | <span data-ttu-id="48f82-138">Тип</span><span class="sxs-lookup"><span data-stu-id="48f82-138">Type</span></span>   |<span data-ttu-id="48f82-139">Описание</span><span class="sxs-lookup"><span data-stu-id="48f82-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f82-140">displayName</span><span class="sxs-lookup"><span data-stu-id="48f82-140">displayName</span></span>|<span data-ttu-id="48f82-141">string</span><span class="sxs-lookup"><span data-stu-id="48f82-141">string</span></span>|<span data-ttu-id="48f82-142">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="48f82-142">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="48f82-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48f82-143">Read-only.</span></span>|
|<span data-ttu-id="48f82-144">id</span><span class="sxs-lookup"><span data-stu-id="48f82-144">id</span></span>|<span data-ttu-id="48f82-145">строка</span><span class="sxs-lookup"><span data-stu-id="48f82-145">string</span></span>| <span data-ttu-id="48f82-146">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="48f82-146">Unique identifier for these settings.</span></span> <span data-ttu-id="48f82-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48f82-147">Read-only.</span></span>|
|<span data-ttu-id="48f82-148">templateId</span><span class="sxs-lookup"><span data-stu-id="48f82-148">templateId</span></span>|<span data-ttu-id="48f82-149">string</span><span class="sxs-lookup"><span data-stu-id="48f82-149">string</span></span>| <span data-ttu-id="48f82-150">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="48f82-150">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="48f82-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48f82-151">Read-only.</span></span>|
|<span data-ttu-id="48f82-152">values</span><span class="sxs-lookup"><span data-stu-id="48f82-152">values</span></span>|<span data-ttu-id="48f82-153">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="48f82-153">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="48f82-154">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="48f82-154">Collection of name value pairs.</span></span> <span data-ttu-id="48f82-155">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="48f82-155">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f82-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="48f82-156">Relationships</span></span>
<span data-ttu-id="48f82-157">Нет</span><span class="sxs-lookup"><span data-stu-id="48f82-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="48f82-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48f82-158">JSON representation</span></span>

<span data-ttu-id="48f82-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48f82-159">Here is a JSON representation of the resource.</span></span>

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
