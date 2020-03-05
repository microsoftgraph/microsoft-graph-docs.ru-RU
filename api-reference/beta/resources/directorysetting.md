---
title: Тип ресурса Директорисеттинг
description: Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес и заменены заданными по умолчанию стилями. Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов. Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.  Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы. Параметры, заданные в системе, управляют поведением групп Office.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d42e46d39e28357d6839111a5e6a865b421cf87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506633"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="9f4a5-107">Тип ресурса Директорисеттинг</span><span class="sxs-lookup"><span data-stu-id="9f4a5-107">directorySetting resource type</span></span>

<span data-ttu-id="9f4a5-108">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f4a5-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f4a5-109">Параметры каталога могут быть созданы на основе доступных [директорисеттингтемплатес](directorysettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-109">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="9f4a5-110">Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-110">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="9f4a5-111">Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-111">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="9f4a5-112">Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-112">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="9f4a5-113">Параметры, заданные в системе, управляют поведением групп Office.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-113">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="9f4a5-114">**Note**: версия/Beta типа ресурса директорисеттинг применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-114">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="9f4a5-115">Версия/v1.0 переименована в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-115">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="9f4a5-116">Методы</span><span class="sxs-lookup"><span data-stu-id="9f4a5-116">Methods</span></span>

| <span data-ttu-id="9f4a5-117">Метод</span><span class="sxs-lookup"><span data-stu-id="9f4a5-117">Method</span></span>           | <span data-ttu-id="9f4a5-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f4a5-118">Return Type</span></span>    |<span data-ttu-id="9f4a5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4a5-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f4a5-120">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="9f4a5-120">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="9f4a5-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9f4a5-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9f4a5-122">Создание объекта Setting на основе объекта Директорисеттингтемплате.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-122">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="9f4a5-123">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-123">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="9f4a5-124">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="9f4a5-124">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="9f4a5-125">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9f4a5-125">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="9f4a5-126">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-126">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="9f4a5-127">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="9f4a5-127">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="9f4a5-128">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="9f4a5-128">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="9f4a5-129">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-129">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="9f4a5-130">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="9f4a5-130">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="9f4a5-131">directorySetting</span><span class="sxs-lookup"><span data-stu-id="9f4a5-131">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="9f4a5-132">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-132">Update a setting object.</span></span> <span data-ttu-id="9f4a5-133">В обновлении можно изменить только Сеттингвалуес.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-133">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="9f4a5-134">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="9f4a5-134">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="9f4a5-135">Нет</span><span class="sxs-lookup"><span data-stu-id="9f4a5-135">None</span></span> |<span data-ttu-id="9f4a5-136">Удаление объекта параметра.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-136">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f4a5-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f4a5-137">Properties</span></span>
| <span data-ttu-id="9f4a5-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f4a5-138">Property</span></span>     | <span data-ttu-id="9f4a5-139">Тип</span><span class="sxs-lookup"><span data-stu-id="9f4a5-139">Type</span></span>   |<span data-ttu-id="9f4a5-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4a5-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f4a5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="9f4a5-141">displayName</span></span>|<span data-ttu-id="9f4a5-142">string</span><span class="sxs-lookup"><span data-stu-id="9f4a5-142">string</span></span>|<span data-ttu-id="9f4a5-143">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-143">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="9f4a5-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-144">Read-only.</span></span>|
|<span data-ttu-id="9f4a5-145">id</span><span class="sxs-lookup"><span data-stu-id="9f4a5-145">id</span></span>|<span data-ttu-id="9f4a5-146">строка</span><span class="sxs-lookup"><span data-stu-id="9f4a5-146">string</span></span>| <span data-ttu-id="9f4a5-147">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-147">Unique identifier for these settings.</span></span> <span data-ttu-id="9f4a5-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-148">Read-only.</span></span>|
|<span data-ttu-id="9f4a5-149">templateId</span><span class="sxs-lookup"><span data-stu-id="9f4a5-149">templateId</span></span>|<span data-ttu-id="9f4a5-150">строка</span><span class="sxs-lookup"><span data-stu-id="9f4a5-150">string</span></span>| <span data-ttu-id="9f4a5-151">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-151">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="9f4a5-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-152">Read-only.</span></span>|
|<span data-ttu-id="9f4a5-153">values</span><span class="sxs-lookup"><span data-stu-id="9f4a5-153">values</span></span>|<span data-ttu-id="9f4a5-154">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9f4a5-154">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="9f4a5-155">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="9f4a5-155">Collection of name value pairs.</span></span> <span data-ttu-id="9f4a5-156">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-156">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f4a5-157">Связи</span><span class="sxs-lookup"><span data-stu-id="9f4a5-157">Relationships</span></span>
<span data-ttu-id="9f4a5-158">Нет</span><span class="sxs-lookup"><span data-stu-id="9f4a5-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9f4a5-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f4a5-159">JSON representation</span></span>

<span data-ttu-id="9f4a5-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f4a5-160">Here is a JSON representation of the resource.</span></span>

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
