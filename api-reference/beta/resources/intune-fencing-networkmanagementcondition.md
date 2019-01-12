---
title: Тип ресурса networkManagementCondition
description: Содержит данные для определения состояния управления сети.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 00ccc045892290ff03e68a109ccc01c4d5dbf8a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927046"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="0da90-103">Тип ресурса networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0da90-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="0da90-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0da90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0da90-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0da90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0da90-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0da90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0da90-107">Содержит данные для определения состояния управления сети.</span><span class="sxs-lookup"><span data-stu-id="0da90-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="0da90-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0da90-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0da90-109">Methods</span></span>
|<span data-ttu-id="0da90-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0da90-110">Method</span></span>|<span data-ttu-id="0da90-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0da90-111">Return Type</span></span>|<span data-ttu-id="0da90-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0da90-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0da90-113">Список networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="0da90-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="0da90-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0da90-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="0da90-115">Свойства списка и связей объектов [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0da90-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0da90-116">Получение networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0da90-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="0da90-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="0da90-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="0da90-118">Чтение свойства и связи объекта [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0da90-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0da90-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0da90-119">Properties</span></span>
|<span data-ttu-id="0da90-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="0da90-120">Property</span></span>|<span data-ttu-id="0da90-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0da90-121">Type</span></span>|<span data-ttu-id="0da90-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0da90-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da90-123">id</span><span class="sxs-lookup"><span data-stu-id="0da90-123">id</span></span>|<span data-ttu-id="0da90-124">String</span><span class="sxs-lookup"><span data-stu-id="0da90-124">String</span></span>|<span data-ttu-id="0da90-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="0da90-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="0da90-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="0da90-126">System generated value assigned when created.</span></span> <span data-ttu-id="0da90-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="0da90-128">uniqueName</span></span>|<span data-ttu-id="0da90-129">String</span><span class="sxs-lookup"><span data-stu-id="0da90-129">String</span></span>|<span data-ttu-id="0da90-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="0da90-130">Unique name for the management condition.</span></span> <span data-ttu-id="0da90-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-131">Used in management condition expressions.</span></span> <span data-ttu-id="0da90-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0da90-133">displayName</span></span>|<span data-ttu-id="0da90-134">String</span><span class="sxs-lookup"><span data-stu-id="0da90-134">String</span></span>|<span data-ttu-id="0da90-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="0da90-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="0da90-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-137">описание</span><span class="sxs-lookup"><span data-stu-id="0da90-137">description</span></span>|<span data-ttu-id="0da90-138">String</span><span class="sxs-lookup"><span data-stu-id="0da90-138">String</span></span>|<span data-ttu-id="0da90-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="0da90-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="0da90-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0da90-141">createdDateTime</span></span>|<span data-ttu-id="0da90-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0da90-142">DateTimeOffset</span></span>|<span data-ttu-id="0da90-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-143">The time the management condition was created.</span></span> <span data-ttu-id="0da90-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0da90-144">Generated service side.</span></span> <span data-ttu-id="0da90-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0da90-146">modifiedDateTime</span></span>|<span data-ttu-id="0da90-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0da90-147">DateTimeOffset</span></span>|<span data-ttu-id="0da90-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-148">The time the management condition was last modified.</span></span> <span data-ttu-id="0da90-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0da90-149">Updated service side.</span></span> <span data-ttu-id="0da90-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-151">eTag</span><span class="sxs-lookup"><span data-stu-id="0da90-151">eTag</span></span>|<span data-ttu-id="0da90-152">String</span><span class="sxs-lookup"><span data-stu-id="0da90-152">String</span></span>|<span data-ttu-id="0da90-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-153">ETag of the management condition.</span></span> <span data-ttu-id="0da90-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0da90-154">Updated service side.</span></span> <span data-ttu-id="0da90-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0da90-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0da90-156">applicablePlatforms</span></span>|<span data-ttu-id="0da90-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0da90-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0da90-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0da90-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0da90-160">Связи</span><span class="sxs-lookup"><span data-stu-id="0da90-160">Relationships</span></span>
|<span data-ttu-id="0da90-161">Связь</span><span class="sxs-lookup"><span data-stu-id="0da90-161">Relationship</span></span>|<span data-ttu-id="0da90-162">Тип</span><span class="sxs-lookup"><span data-stu-id="0da90-162">Type</span></span>|<span data-ttu-id="0da90-163">Описание</span><span class="sxs-lookup"><span data-stu-id="0da90-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da90-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0da90-164">managementConditionStatements</span></span>|<span data-ttu-id="0da90-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0da90-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0da90-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="0da90-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0da90-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0da90-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0da90-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0da90-168">JSON Representation</span></span>
<span data-ttu-id="0da90-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0da90-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





