---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81c6937fca0c51b18d86ccf3b0dbedd58b71971b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783118"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="be81c-103">Тип ресурса Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="be81c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be81c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be81c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be81c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be81c-106">Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="be81c-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="be81c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="be81c-107">Methods</span></span>
|<span data-ttu-id="be81c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="be81c-108">Method</span></span>|<span data-ttu-id="be81c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be81c-109">Return Type</span></span>|<span data-ttu-id="be81c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be81c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be81c-111">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="be81c-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="be81c-112">Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be81c-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="be81c-113">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be81c-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="be81c-114">Получение Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="be81c-115">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="be81c-116">Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be81c-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="be81c-117">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="be81c-118">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="be81c-119">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be81c-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="be81c-120">Удаление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="be81c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="be81c-121">None</span></span>|<span data-ttu-id="be81c-122">Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be81c-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="be81c-123">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="be81c-124">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="be81c-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="be81c-125">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="be81c-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="be81c-126">Действие assign</span><span class="sxs-lookup"><span data-stu-id="be81c-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="be81c-127">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be81c-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="be81c-128">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be81c-128">Not yet documented</span></span>|
|[<span data-ttu-id="be81c-129">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="be81c-129">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="be81c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="be81c-130">None</span></span>|<span data-ttu-id="be81c-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be81c-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="be81c-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="be81c-132">Properties</span></span>
|<span data-ttu-id="be81c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="be81c-133">Property</span></span>|<span data-ttu-id="be81c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="be81c-134">Type</span></span>|<span data-ttu-id="be81c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="be81c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be81c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be81c-136">createdDateTime</span></span>|<span data-ttu-id="be81c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be81c-137">DateTimeOffset</span></span>|<span data-ttu-id="be81c-138">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="be81c-138">The date and time the object was created.</span></span>|
|<span data-ttu-id="be81c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="be81c-139">displayName</span></span>|<span data-ttu-id="be81c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="be81c-140">String</span></span>|<span data-ttu-id="be81c-141">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="be81c-141">User provided name for the resource object.</span></span>|
|<span data-ttu-id="be81c-142">description</span><span class="sxs-lookup"><span data-stu-id="be81c-142">description</span></span>|<span data-ttu-id="be81c-143">String</span><span class="sxs-lookup"><span data-stu-id="be81c-143">String</span></span>|<span data-ttu-id="be81c-144">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="be81c-144">User provided description for the resource object.</span></span>|
|<span data-ttu-id="be81c-145">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be81c-145">roleScopeTagIds</span></span>|<span data-ttu-id="be81c-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="be81c-146">String collection</span></span>|<span data-ttu-id="be81c-147">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="be81c-147">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="be81c-148">id</span><span class="sxs-lookup"><span data-stu-id="be81c-148">id</span></span>|<span data-ttu-id="be81c-149">String</span><span class="sxs-lookup"><span data-stu-id="be81c-149">String</span></span>|<span data-ttu-id="be81c-150">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be81c-150">Key of the entity.</span></span>|
|<span data-ttu-id="be81c-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be81c-151">lastModifiedDateTime</span></span>|<span data-ttu-id="be81c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be81c-152">DateTimeOffset</span></span>|<span data-ttu-id="be81c-153">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be81c-153">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be81c-154">Связи</span><span class="sxs-lookup"><span data-stu-id="be81c-154">Relationships</span></span>
|<span data-ttu-id="be81c-155">Связь</span><span class="sxs-lookup"><span data-stu-id="be81c-155">Relationship</span></span>|<span data-ttu-id="be81c-156">Тип</span><span class="sxs-lookup"><span data-stu-id="be81c-156">Type</span></span>|<span data-ttu-id="be81c-157">Описание</span><span class="sxs-lookup"><span data-stu-id="be81c-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be81c-158">дефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="be81c-158">definitionValues</span></span>|<span data-ttu-id="be81c-159">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="be81c-159">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="be81c-160">Список включенных или отключенных значений определений групповой политики для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="be81c-160">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="be81c-161">assignments</span><span class="sxs-lookup"><span data-stu-id="be81c-161">assignments</span></span>|<span data-ttu-id="be81c-162">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="be81c-162">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="be81c-163">Список назначений групп для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="be81c-163">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be81c-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be81c-164">JSON Representation</span></span>
<span data-ttu-id="be81c-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be81c-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



