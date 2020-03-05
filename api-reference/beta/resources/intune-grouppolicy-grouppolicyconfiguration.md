---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5624f86622b49d8739de85a2c58067dd7263aace
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528117"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="737c1-103">Тип ресурса Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-103">groupPolicyConfiguration resource type</span></span>

<span data-ttu-id="737c1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="737c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="737c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="737c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="737c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="737c1-107">Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="737c1-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="737c1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="737c1-108">Methods</span></span>
|<span data-ttu-id="737c1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="737c1-109">Method</span></span>|<span data-ttu-id="737c1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="737c1-110">Return Type</span></span>|<span data-ttu-id="737c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="737c1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="737c1-112">Список Граупполициконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="737c1-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="737c1-113">Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="737c1-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="737c1-114">Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="737c1-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="737c1-115">Получение Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="737c1-116">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="737c1-117">Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="737c1-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="737c1-118">Создание Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="737c1-119">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="737c1-120">Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="737c1-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="737c1-121">Удаление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="737c1-122">Нет</span><span class="sxs-lookup"><span data-stu-id="737c1-122">None</span></span>|<span data-ttu-id="737c1-123">Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="737c1-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="737c1-124">Обновление Граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="737c1-125">граупполициконфигуратион</span><span class="sxs-lookup"><span data-stu-id="737c1-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="737c1-126">Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="737c1-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="737c1-127">Действие assign</span><span class="sxs-lookup"><span data-stu-id="737c1-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="737c1-128">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="737c1-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="737c1-129">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="737c1-129">Not yet documented</span></span>|
|[<span data-ttu-id="737c1-130">действие Упдатедефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="737c1-130">updateDefinitionValues action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|<span data-ttu-id="737c1-131">Нет</span><span class="sxs-lookup"><span data-stu-id="737c1-131">None</span></span>|<span data-ttu-id="737c1-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="737c1-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="737c1-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="737c1-133">Properties</span></span>
|<span data-ttu-id="737c1-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="737c1-134">Property</span></span>|<span data-ttu-id="737c1-135">Тип</span><span class="sxs-lookup"><span data-stu-id="737c1-135">Type</span></span>|<span data-ttu-id="737c1-136">Описание</span><span class="sxs-lookup"><span data-stu-id="737c1-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="737c1-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="737c1-137">createdDateTime</span></span>|<span data-ttu-id="737c1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="737c1-138">DateTimeOffset</span></span>|<span data-ttu-id="737c1-139">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="737c1-139">The date and time the object was created.</span></span>|
|<span data-ttu-id="737c1-140">displayName</span><span class="sxs-lookup"><span data-stu-id="737c1-140">displayName</span></span>|<span data-ttu-id="737c1-141">Строка</span><span class="sxs-lookup"><span data-stu-id="737c1-141">String</span></span>|<span data-ttu-id="737c1-142">Предоставленное пользователем имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="737c1-142">User provided name for the resource object.</span></span>|
|<span data-ttu-id="737c1-143">description</span><span class="sxs-lookup"><span data-stu-id="737c1-143">description</span></span>|<span data-ttu-id="737c1-144">String</span><span class="sxs-lookup"><span data-stu-id="737c1-144">String</span></span>|<span data-ttu-id="737c1-145">Предоставленное пользователем описание объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="737c1-145">User provided description for the resource object.</span></span>|
|<span data-ttu-id="737c1-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="737c1-146">roleScopeTagIds</span></span>|<span data-ttu-id="737c1-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="737c1-147">String collection</span></span>|<span data-ttu-id="737c1-148">Список тегов области для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="737c1-148">The list of scope tags for the configuration.</span></span>|
|<span data-ttu-id="737c1-149">id</span><span class="sxs-lookup"><span data-stu-id="737c1-149">id</span></span>|<span data-ttu-id="737c1-150">String</span><span class="sxs-lookup"><span data-stu-id="737c1-150">String</span></span>|<span data-ttu-id="737c1-151">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="737c1-151">Key of the entity.</span></span>|
|<span data-ttu-id="737c1-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="737c1-152">lastModifiedDateTime</span></span>|<span data-ttu-id="737c1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="737c1-153">DateTimeOffset</span></span>|<span data-ttu-id="737c1-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="737c1-154">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="737c1-155">Связи</span><span class="sxs-lookup"><span data-stu-id="737c1-155">Relationships</span></span>
|<span data-ttu-id="737c1-156">Связь</span><span class="sxs-lookup"><span data-stu-id="737c1-156">Relationship</span></span>|<span data-ttu-id="737c1-157">Тип</span><span class="sxs-lookup"><span data-stu-id="737c1-157">Type</span></span>|<span data-ttu-id="737c1-158">Описание</span><span class="sxs-lookup"><span data-stu-id="737c1-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="737c1-159">дефинитионвалуес</span><span class="sxs-lookup"><span data-stu-id="737c1-159">definitionValues</span></span>|<span data-ttu-id="737c1-160">Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)</span><span class="sxs-lookup"><span data-stu-id="737c1-160">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="737c1-161">Список включенных или отключенных значений определений групповой политики для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="737c1-161">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="737c1-162">assignments</span><span class="sxs-lookup"><span data-stu-id="737c1-162">assignments</span></span>|<span data-ttu-id="737c1-163">Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="737c1-163">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="737c1-164">Список назначений групп для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="737c1-164">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="737c1-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="737c1-165">JSON Representation</span></span>
<span data-ttu-id="737c1-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="737c1-166">Here is a JSON representation of the resource.</span></span>
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



