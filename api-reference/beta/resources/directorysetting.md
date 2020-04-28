---
title: Тип ресурса Директорисеттинг
description: Параметры каталога могут быть созданы на основе доступных Директорисеттингтемплатес и заменены заданными по умолчанию стилями.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8aa79fb8372b9603c8c0d4845d6107e9f3f3cd76
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181766"
---
# <a name="directorysetting-resource-type"></a><span data-ttu-id="d38b2-103">Тип ресурса Директорисеттинг</span><span class="sxs-lookup"><span data-stu-id="d38b2-103">directorySetting resource type</span></span>

<span data-ttu-id="d38b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d38b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38b2-105">Параметры каталога могут быть созданы на основе доступных [директорисеттингтемплатес](directorysettingtemplate.md)и заменены заданными по умолчанию стилями.</span><span class="sxs-lookup"><span data-stu-id="d38b2-105">Directory settings can be created based on the available [directorySettingTemplates](directorysettingtemplate.md), and changed from their preset defaults.</span></span> <span data-ttu-id="d38b2-106">Эти параметры могут управлять поведением сущностей или компонентов как на уровне клиента, так и на уровне отдельных объектов.</span><span class="sxs-lookup"><span data-stu-id="d38b2-106">These settings can govern entity or feature behaviors, both at a tenant-wide level or at a specific entity level.</span></span> <span data-ttu-id="d38b2-107">Если один и тот же параметр определен как на уровне клиента, так и на уровне отдельных сущностей, то параметры определенного уровня объекта могут отказаться от использования параметра на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="d38b2-107">When the same setting is defined at both the tenant-wide and specific entity level, the specific entity level setting may opt-out from the tenant-wide setting.</span></span>  <span data-ttu-id="d38b2-108">Например, параметр на уровне клиента может разрешить гостям, которые могут быть приглашены существующими участниками групп, но определенные параметры группы могут отказаться от использования приглашений гостей для участников группы.</span><span class="sxs-lookup"><span data-stu-id="d38b2-108">For example, the tenant-wide setting may allow guests to be invited by existing members of groups, but a specific group setting may opt-out and not allow guests to be invited by members of the group.</span></span> <span data-ttu-id="d38b2-109">Параметры, заданные в системе, управляют поведением групп Office.</span><span class="sxs-lookup"><span data-stu-id="d38b2-109">Currently system defined settings are only govern Office groups behavior.</span></span>

> <span data-ttu-id="d38b2-110">**Note**: версия/Beta типа ресурса директорисеттинг применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="d38b2-110">**Note**: The /beta version of the directorySetting resource type only applies to groups.</span></span> <span data-ttu-id="d38b2-111">Версия/v1.0 переименована в groupSetting.</span><span class="sxs-lookup"><span data-stu-id="d38b2-111">The /v1.0 version has been renamed to groupSetting.</span></span>

## <a name="methods"></a><span data-ttu-id="d38b2-112">Методы</span><span class="sxs-lookup"><span data-stu-id="d38b2-112">Methods</span></span>

| <span data-ttu-id="d38b2-113">Метод</span><span class="sxs-lookup"><span data-stu-id="d38b2-113">Method</span></span>           | <span data-ttu-id="d38b2-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d38b2-114">Return Type</span></span>    |<span data-ttu-id="d38b2-115">Описание</span><span class="sxs-lookup"><span data-stu-id="d38b2-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d38b2-116">Создание параметра</span><span class="sxs-lookup"><span data-stu-id="d38b2-116">Create setting</span></span>](../api/directorysetting-post-settings.md) | [<span data-ttu-id="d38b2-117">directorySetting</span><span class="sxs-lookup"><span data-stu-id="d38b2-117">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="d38b2-118">Создание объекта Setting на основе объекта Директорисеттингтемплате.</span><span class="sxs-lookup"><span data-stu-id="d38b2-118">Create a setting object based on a directorySettingTemplate.</span></span> <span data-ttu-id="d38b2-119">Запрос POST должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="d38b2-119">The POST request must provide settingValues for all the settings defined in the template.</span></span>|
|[<span data-ttu-id="d38b2-120">Получение параметра</span><span class="sxs-lookup"><span data-stu-id="d38b2-120">Get setting</span></span>](../api/directorysetting-get.md) | [<span data-ttu-id="d38b2-121">directorySetting</span><span class="sxs-lookup"><span data-stu-id="d38b2-121">directorySetting</span></span>](directorysetting.md) |<span data-ttu-id="d38b2-122">Считывание свойств определенного объекта setting.</span><span class="sxs-lookup"><span data-stu-id="d38b2-122">Read properties of a specific setting object.</span></span>|
|[<span data-ttu-id="d38b2-123">Перечисление параметров</span><span class="sxs-lookup"><span data-stu-id="d38b2-123">List settings</span></span>](../api/directorysetting-list.md) | <span data-ttu-id="d38b2-124">Коллекция [directorySetting](directorysetting.md)</span><span class="sxs-lookup"><span data-stu-id="d38b2-124">[directorySetting](directorysetting.md) collection</span></span> |<span data-ttu-id="d38b2-125">Перечисление свойств всех объектов setting.</span><span class="sxs-lookup"><span data-stu-id="d38b2-125">List properties of all setting objects.</span></span>|
|[<span data-ttu-id="d38b2-126">Обновление параметра</span><span class="sxs-lookup"><span data-stu-id="d38b2-126">Update setting</span></span>](../api/directorysetting-update.md) | [<span data-ttu-id="d38b2-127">directorySetting</span><span class="sxs-lookup"><span data-stu-id="d38b2-127">directorySetting</span></span>](directorysetting.md)  |<span data-ttu-id="d38b2-128">Обновление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="d38b2-128">Update a setting object.</span></span> <span data-ttu-id="d38b2-129">В обновлении можно изменить только Сеттингвалуес.</span><span class="sxs-lookup"><span data-stu-id="d38b2-129">Only settingValues can be changed in an update.</span></span>|
|[<span data-ttu-id="d38b2-130">Удаление параметра</span><span class="sxs-lookup"><span data-stu-id="d38b2-130">Delete setting</span></span>](../api/directorysetting-delete.md) | <span data-ttu-id="d38b2-131">Нет</span><span class="sxs-lookup"><span data-stu-id="d38b2-131">None</span></span> |<span data-ttu-id="d38b2-132">Удаление объекта setting.</span><span class="sxs-lookup"><span data-stu-id="d38b2-132">Delete a setting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d38b2-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="d38b2-133">Properties</span></span>
| <span data-ttu-id="d38b2-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d38b2-134">Property</span></span>     | <span data-ttu-id="d38b2-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d38b2-135">Type</span></span>   |<span data-ttu-id="d38b2-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d38b2-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d38b2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d38b2-137">displayName</span></span>|<span data-ttu-id="d38b2-138">string</span><span class="sxs-lookup"><span data-stu-id="d38b2-138">string</span></span>|<span data-ttu-id="d38b2-139">Отображаемое имя группы параметров, поступающих из связанного шаблона.</span><span class="sxs-lookup"><span data-stu-id="d38b2-139">Display name of this group of settings, which comes from the associated template.</span></span> <span data-ttu-id="d38b2-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d38b2-140">Read-only.</span></span>|
|<span data-ttu-id="d38b2-141">id</span><span class="sxs-lookup"><span data-stu-id="d38b2-141">id</span></span>|<span data-ttu-id="d38b2-142">string</span><span class="sxs-lookup"><span data-stu-id="d38b2-142">string</span></span>| <span data-ttu-id="d38b2-143">Уникальный идентификатор для этих параметров.</span><span class="sxs-lookup"><span data-stu-id="d38b2-143">Unique identifier for these settings.</span></span> <span data-ttu-id="d38b2-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d38b2-144">Read-only.</span></span>|
|<span data-ttu-id="d38b2-145">templateId</span><span class="sxs-lookup"><span data-stu-id="d38b2-145">templateId</span></span>|<span data-ttu-id="d38b2-146">string</span><span class="sxs-lookup"><span data-stu-id="d38b2-146">string</span></span>| <span data-ttu-id="d38b2-147">Уникальный идентификатор шаблона, который используется для создания этой группы параметров.</span><span class="sxs-lookup"><span data-stu-id="d38b2-147">Unique identifier for the template used to create this group of settings.</span></span> <span data-ttu-id="d38b2-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d38b2-148">Read-only.</span></span>|
|<span data-ttu-id="d38b2-149">values</span><span class="sxs-lookup"><span data-stu-id="d38b2-149">values</span></span>|<span data-ttu-id="d38b2-150">Коллекция [settingValue](settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d38b2-150">[settingValue](settingvalue.md) collection</span></span>| <span data-ttu-id="d38b2-151">Коллекция пар "имя-значение".</span><span class="sxs-lookup"><span data-stu-id="d38b2-151">Collection of name value pairs.</span></span> <span data-ttu-id="d38b2-152">Должен содержать и задавать все параметры, определенные в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="d38b2-152">Must contain and set all the settings defined in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d38b2-153">Связи</span><span class="sxs-lookup"><span data-stu-id="d38b2-153">Relationships</span></span>
<span data-ttu-id="d38b2-154">Нет</span><span class="sxs-lookup"><span data-stu-id="d38b2-154">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d38b2-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d38b2-155">JSON representation</span></span>

<span data-ttu-id="d38b2-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d38b2-156">Here is a JSON representation of the resource.</span></span>

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
