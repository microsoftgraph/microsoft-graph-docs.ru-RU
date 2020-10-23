---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fb3ea6abdceae5f3af2300810d7d822b2c2c5e39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697429"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="bd720-103">Тип ресурса Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-103">groupPolicyConfiguration resource type</span></span>

<span data-ttu-id="bd720-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd720-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd720-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd720-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd720-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd720-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd720-107">Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="bd720-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="bd720-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bd720-108">Methods</span></span>
|<span data-ttu-id="bd720-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bd720-109">Method</span></span>|<span data-ttu-id="bd720-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd720-110">Return Type</span></span>|<span data-ttu-id="bd720-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd720-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd720-112">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="bd720-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="bd720-113">Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bd720-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="bd720-114">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd720-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bd720-115">Получение Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="bd720-116">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="bd720-117">Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd720-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bd720-118">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="bd720-119">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="bd720-120">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd720-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bd720-121">Удаление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="bd720-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bd720-122">None</span></span>|<span data-ttu-id="bd720-123">Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bd720-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="bd720-124">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="bd720-125">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bd720-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="bd720-126">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bd720-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bd720-127">Действие assign</span><span class="sxs-lookup"><span data-stu-id="bd720-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="bd720-128">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bd720-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bd720-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bd720-129">Not yet documented</span></span>|
|[<span data-ttu-id="bd720-130">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="bd720-130">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="bd720-131">Нет</span><span class="sxs-lookup"><span data-stu-id="bd720-131">None</span></span>|<span data-ttu-id="bd720-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bd720-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bd720-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd720-133">Properties</span></span>
|<span data-ttu-id="bd720-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd720-134">Property</span></span>|<span data-ttu-id="bd720-135">Тип</span><span class="sxs-lookup"><span data-stu-id="bd720-135">Type</span></span>|<span data-ttu-id="bd720-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bd720-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd720-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd720-137">createdDateTime</span></span>|<span data-ttu-id="bd720-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd720-138">DateTimeOffset</span></span>|<span data-ttu-id="bd720-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bd720-139">The date and time the object was created.</span></span>|
|<span data-ttu-id="bd720-140">displayName</span><span class="sxs-lookup"><span data-stu-id="bd720-140">displayName</span></span>|<span data-ttu-id="bd720-141">Строка</span><span class="sxs-lookup"><span data-stu-id="bd720-141">String</span></span>|<span data-ttu-id="bd720-142">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd720-142">User provided name for the resource object.</span></span>|
|<span data-ttu-id="bd720-143">description</span><span class="sxs-lookup"><span data-stu-id="bd720-143">description</span></span>|<span data-ttu-id="bd720-144">Строка</span><span class="sxs-lookup"><span data-stu-id="bd720-144">String</span></span>|<span data-ttu-id="bd720-145">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="bd720-145">User provided description for the resource object.</span></span>|
|<span data-ttu-id="bd720-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bd720-146">roleScopeTagIds</span></span>|<span data-ttu-id="bd720-147">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bd720-147">String collection</span></span>|<span data-ttu-id="bd720-148">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd720-148">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="bd720-149">id</span><span class="sxs-lookup"><span data-stu-id="bd720-149">id</span></span>|<span data-ttu-id="bd720-150">Строка</span><span class="sxs-lookup"><span data-stu-id="bd720-150">String</span></span>|<span data-ttu-id="bd720-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd720-151">Key of the entity.</span></span>|
|<span data-ttu-id="bd720-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd720-152">lastModifiedDateTime</span></span>|<span data-ttu-id="bd720-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd720-153">DateTimeOffset</span></span>|<span data-ttu-id="bd720-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bd720-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd720-155">Связи</span><span class="sxs-lookup"><span data-stu-id="bd720-155">Relationships</span></span>
|<span data-ttu-id="bd720-156">Связь</span><span class="sxs-lookup"><span data-stu-id="bd720-156">Relationship</span></span>|<span data-ttu-id="bd720-157">Тип</span><span class="sxs-lookup"><span data-stu-id="bd720-157">Type</span></span>|<span data-ttu-id="bd720-158">Описание</span><span class="sxs-lookup"><span data-stu-id="bd720-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd720-159">дефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="bd720-159">definitionValues</span></span>|<span data-ttu-id="bd720-160">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bd720-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="bd720-161">Список включенных или отключенных значений определений групповой политики для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd720-161">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="bd720-162">assignments</span><span class="sxs-lookup"><span data-stu-id="bd720-162">assignments</span></span>|<span data-ttu-id="bd720-163">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bd720-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bd720-164">Список назначений групп для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bd720-164">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd720-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd720-165">JSON Representation</span></span>
<span data-ttu-id="bd720-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd720-166">Here is a JSON representation of the resource.</span></span>
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





