---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d910bf8bdef34c60ca6bb66e1ce87ca9cf1d51ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941179"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="e4086-103">Тип ресурса Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="e4086-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4086-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4086-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4086-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4086-106">Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e4086-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="e4086-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e4086-107">Methods</span></span>
|<span data-ttu-id="e4086-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e4086-108">Method</span></span>|<span data-ttu-id="e4086-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4086-109">Return Type</span></span>|<span data-ttu-id="e4086-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4086-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4086-111">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="e4086-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="e4086-112">Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4086-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="e4086-113">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4086-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e4086-114">Получение Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="e4086-115">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e4086-116">Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4086-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e4086-117">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="e4086-118">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e4086-119">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4086-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e4086-120">Удаление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="e4086-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e4086-121">None</span></span>|<span data-ttu-id="e4086-122">Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e4086-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="e4086-123">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="e4086-124">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e4086-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e4086-125">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e4086-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e4086-126">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e4086-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="e4086-127">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e4086-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e4086-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e4086-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e4086-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4086-129">Properties</span></span>
|<span data-ttu-id="e4086-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4086-130">Property</span></span>|<span data-ttu-id="e4086-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4086-131">Type</span></span>|<span data-ttu-id="e4086-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4086-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4086-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4086-133">createdDateTime</span></span>|<span data-ttu-id="e4086-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4086-134">DateTimeOffset</span></span>|<span data-ttu-id="e4086-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e4086-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="e4086-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e4086-136">displayName</span></span>|<span data-ttu-id="e4086-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e4086-137">String</span></span>|<span data-ttu-id="e4086-138">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4086-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="e4086-139">description</span><span class="sxs-lookup"><span data-stu-id="e4086-139">description</span></span>|<span data-ttu-id="e4086-140">String</span><span class="sxs-lookup"><span data-stu-id="e4086-140">String</span></span>|<span data-ttu-id="e4086-141">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="e4086-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="e4086-142">id</span><span class="sxs-lookup"><span data-stu-id="e4086-142">id</span></span>|<span data-ttu-id="e4086-143">String</span><span class="sxs-lookup"><span data-stu-id="e4086-143">String</span></span>|<span data-ttu-id="e4086-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4086-144">Key of the entity.</span></span>|
|<span data-ttu-id="e4086-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4086-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e4086-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4086-146">DateTimeOffset</span></span>|<span data-ttu-id="e4086-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e4086-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4086-148">Связи</span><span class="sxs-lookup"><span data-stu-id="e4086-148">Relationships</span></span>
|<span data-ttu-id="e4086-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="e4086-149">Relationship</span></span>|<span data-ttu-id="e4086-150">Тип</span><span class="sxs-lookup"><span data-stu-id="e4086-150">Type</span></span>|<span data-ttu-id="e4086-151">Описание</span><span class="sxs-lookup"><span data-stu-id="e4086-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4086-152">Дефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="e4086-152">definitionValues</span></span>|<span data-ttu-id="e4086-153">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e4086-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="e4086-154">Список включенных или отключенных значений определений групповой политики для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e4086-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="e4086-155">assignments</span><span class="sxs-lookup"><span data-stu-id="e4086-155">assignments</span></span>|<span data-ttu-id="e4086-156">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e4086-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e4086-157">Список назначений групп для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e4086-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4086-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4086-158">JSON Representation</span></span>
<span data-ttu-id="e4086-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4086-159">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




