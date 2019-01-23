---
title: Тип ресурса groupPolicyConfiguration
description: Сущности конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431755"
---
# <a name="grouppolicyconfiguration-resource-type"></a><span data-ttu-id="e9f89-103">Тип ресурса groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-103">groupPolicyConfiguration resource type</span></span>

> <span data-ttu-id="e9f89-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9f89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9f89-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9f89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9f89-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9f89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9f89-107">Сущности конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.</span><span class="sxs-lookup"><span data-stu-id="e9f89-107">The group policy configuration entity contains the configured values for one or more group policy definitions.</span></span>

## <a name="methods"></a><span data-ttu-id="e9f89-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e9f89-108">Methods</span></span>
|<span data-ttu-id="e9f89-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e9f89-109">Method</span></span>|<span data-ttu-id="e9f89-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9f89-110">Return Type</span></span>|<span data-ttu-id="e9f89-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f89-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9f89-112">Список groupPolicyConfigurations</span><span class="sxs-lookup"><span data-stu-id="e9f89-112">List groupPolicyConfigurations</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|<span data-ttu-id="e9f89-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e9f89-113">[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) collection</span></span>|<span data-ttu-id="e9f89-114">Свойства списка и связей объектов [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f89-114">List properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e9f89-115">Получение groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-115">Get groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[<span data-ttu-id="e9f89-116">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-116">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e9f89-117">Чтение свойства и связи объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f89-117">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e9f89-118">Создание groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-118">Create groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[<span data-ttu-id="e9f89-119">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-119">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e9f89-120">Создание нового объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f89-120">Create a new [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e9f89-121">Удаление groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-121">Delete groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|<span data-ttu-id="e9f89-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e9f89-122">None</span></span>|<span data-ttu-id="e9f89-123">Удаляет [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e9f89-123">Deletes a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).</span></span>|
|[<span data-ttu-id="e9f89-124">Обновление groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-124">Update groupPolicyConfiguration</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[<span data-ttu-id="e9f89-125">groupPolicyConfiguration</span><span class="sxs-lookup"><span data-stu-id="e9f89-125">groupPolicyConfiguration</span></span>](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|<span data-ttu-id="e9f89-126">Обновление свойства объекта [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e9f89-126">Update the properties of a [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>|
|[<span data-ttu-id="e9f89-127">Действие assign</span><span class="sxs-lookup"><span data-stu-id="e9f89-127">assign action</span></span>](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|<span data-ttu-id="e9f89-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e9f89-128">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e9f89-129">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e9f89-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e9f89-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9f89-130">Properties</span></span>
|<span data-ttu-id="e9f89-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9f89-131">Property</span></span>|<span data-ttu-id="e9f89-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e9f89-132">Type</span></span>|<span data-ttu-id="e9f89-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f89-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f89-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f89-134">createdDateTime</span></span>|<span data-ttu-id="e9f89-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f89-135">DateTimeOffset</span></span>|<span data-ttu-id="e9f89-136">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e9f89-136">The date and time the object was created.</span></span>|
|<span data-ttu-id="e9f89-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e9f89-137">displayName</span></span>|<span data-ttu-id="e9f89-138">String</span><span class="sxs-lookup"><span data-stu-id="e9f89-138">String</span></span>|<span data-ttu-id="e9f89-139">Имя объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="e9f89-139">User provided name for the resource object.</span></span>|
|<span data-ttu-id="e9f89-140">description</span><span class="sxs-lookup"><span data-stu-id="e9f89-140">description</span></span>|<span data-ttu-id="e9f89-141">String</span><span class="sxs-lookup"><span data-stu-id="e9f89-141">String</span></span>|<span data-ttu-id="e9f89-142">Описание для объекта ресурса, предоставляемые пользователями.</span><span class="sxs-lookup"><span data-stu-id="e9f89-142">User provided description for the resource object.</span></span>|
|<span data-ttu-id="e9f89-143">id</span><span class="sxs-lookup"><span data-stu-id="e9f89-143">id</span></span>|<span data-ttu-id="e9f89-144">String</span><span class="sxs-lookup"><span data-stu-id="e9f89-144">String</span></span>|<span data-ttu-id="e9f89-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9f89-145">Key of the entity.</span></span>|
|<span data-ttu-id="e9f89-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f89-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e9f89-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f89-147">DateTimeOffset</span></span>|<span data-ttu-id="e9f89-148">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e9f89-148">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9f89-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9f89-149">Relationships</span></span>
|<span data-ttu-id="e9f89-150">Связь</span><span class="sxs-lookup"><span data-stu-id="e9f89-150">Relationship</span></span>|<span data-ttu-id="e9f89-151">Тип</span><span class="sxs-lookup"><span data-stu-id="e9f89-151">Type</span></span>|<span data-ttu-id="e9f89-152">Описание</span><span class="sxs-lookup"><span data-stu-id="e9f89-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f89-153">definitionValues</span><span class="sxs-lookup"><span data-stu-id="e9f89-153">definitionValues</span></span>|<span data-ttu-id="e9f89-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e9f89-154">[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) collection</span></span>|<span data-ttu-id="e9f89-155">Список включен или отключен групповой политики определения значений для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e9f89-155">The list of enabled or disabled group policy definition values for the configuration.</span></span>|
|<span data-ttu-id="e9f89-156">assignments</span><span class="sxs-lookup"><span data-stu-id="e9f89-156">assignments</span></span>|<span data-ttu-id="e9f89-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e9f89-157">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e9f89-158">Список назначений группы для конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e9f89-158">The list of group assignments for the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9f89-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9f89-159">JSON Representation</span></span>
<span data-ttu-id="e9f89-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9f89-160">Here is a JSON representation of the resource.</span></span>
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




