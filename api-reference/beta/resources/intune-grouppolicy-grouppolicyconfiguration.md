---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 544b743ab690521fee48e3609e2c62582131d6ef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994246"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="9b230-103">Тип ресурса Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="9b230-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b230-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b230-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b230-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b230-106">Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="9b230-106">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="9b230-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9b230-107">Methods</span></span>
|<span data-ttu-id="9b230-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9b230-108">Method</span></span>|<span data-ttu-id="9b230-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b230-109">Return Type</span></span>|<span data-ttu-id="9b230-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b230-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b230-111">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="9b230-111">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="9b230-112">Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9b230-112">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="9b230-113">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b230-113">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="9b230-114">Получение Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-114">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="9b230-115">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-115">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="9b230-116">Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b230-116">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9b230-117">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-117">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="9b230-118">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-118">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="9b230-119">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b230-119">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9b230-120">Удаление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-120">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="9b230-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9b230-121">None</span></span>|<span data-ttu-id="9b230-122">Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9b230-122">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="9b230-123">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-123">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="9b230-124">Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9b230-124">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="9b230-125">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9b230-125">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="9b230-126">Действие assign</span><span class="sxs-lookup"><span data-stu-id="9b230-126">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="9b230-127">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b230-127">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9b230-128">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9b230-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9b230-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b230-129">Properties</span></span>
|<span data-ttu-id="9b230-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b230-130">Property</span></span>|<span data-ttu-id="9b230-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b230-131">Type</span></span>|<span data-ttu-id="9b230-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b230-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b230-133">createdDateTime</span></span>|<span data-ttu-id="9b230-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b230-134">DateTimeOffset</span></span>|<span data-ttu-id="9b230-135">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9b230-135">The date and time the object was created.</span></span>|
|<span data-ttu-id="9b230-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9b230-136">displayName</span></span>|<span data-ttu-id="9b230-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9b230-137">String</span></span>|<span data-ttu-id="9b230-138">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="9b230-138">User provided name for the resource object.</span></span>|
|<span data-ttu-id="9b230-139">description</span><span class="sxs-lookup"><span data-stu-id="9b230-139">description</span></span>|<span data-ttu-id="9b230-140">String</span><span class="sxs-lookup"><span data-stu-id="9b230-140">String</span></span>|<span data-ttu-id="9b230-141">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="9b230-141">User provided description for the resource object.</span></span>|
|<span data-ttu-id="9b230-142">id</span><span class="sxs-lookup"><span data-stu-id="9b230-142">id</span></span>|<span data-ttu-id="9b230-143">String</span><span class="sxs-lookup"><span data-stu-id="9b230-143">String</span></span>|<span data-ttu-id="9b230-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9b230-144">Key of the entity.</span></span>|
|<span data-ttu-id="9b230-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b230-145">lastModifiedDateTime</span></span>|<span data-ttu-id="9b230-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b230-146">DateTimeOffset</span></span>|<span data-ttu-id="9b230-147">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9b230-147">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b230-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="9b230-148">Relationships</span></span>
|<span data-ttu-id="9b230-149">Отношение</span><span class="sxs-lookup"><span data-stu-id="9b230-149">Relationship</span></span>|<span data-ttu-id="9b230-150">Тип</span><span class="sxs-lookup"><span data-stu-id="9b230-150">Type</span></span>|<span data-ttu-id="9b230-151">Описание</span><span class="sxs-lookup"><span data-stu-id="9b230-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b230-152">Дефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="9b230-152">definitionValues</span></span>|<span data-ttu-id="9b230-153">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9b230-153">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="9b230-154">Список включенных или отключенных значений определений групповой политики для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9b230-154">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="9b230-155">assignments</span><span class="sxs-lookup"><span data-stu-id="9b230-155">assignments</span></span>|<span data-ttu-id="9b230-156">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9b230-156">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="9b230-157">Список назначений групп для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="9b230-157">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b230-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b230-158">JSON Representation</span></span>
<span data-ttu-id="9b230-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b230-159">Here is a JSON representation of the resource.</span></span>
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





