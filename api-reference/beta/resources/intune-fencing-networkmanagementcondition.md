---
title: Тип ресурса networkManagementCondition
description: Содержит данные для определения состояния управления сети.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7d91ac60ae52f3317e8148e8bb4adcaf82afac53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806512"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="cc47b-103">Тип ресурса networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc47b-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="cc47b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc47b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc47b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc47b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc47b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc47b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc47b-107">Содержит данные для определения состояния управления сети.</span><span class="sxs-lookup"><span data-stu-id="cc47b-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="cc47b-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cc47b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="cc47b-109">Methods</span></span>
|<span data-ttu-id="cc47b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="cc47b-110">Method</span></span>|<span data-ttu-id="cc47b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc47b-111">Return Type</span></span>|<span data-ttu-id="cc47b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cc47b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc47b-113">Список networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="cc47b-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="cc47b-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cc47b-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="cc47b-115">Свойства списка и связей объектов [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cc47b-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="cc47b-116">Получение networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc47b-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="cc47b-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="cc47b-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="cc47b-118">Чтение свойства и связи объекта [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="cc47b-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc47b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc47b-119">Properties</span></span>
|<span data-ttu-id="cc47b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc47b-120">Property</span></span>|<span data-ttu-id="cc47b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cc47b-121">Type</span></span>|<span data-ttu-id="cc47b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cc47b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc47b-123">id</span><span class="sxs-lookup"><span data-stu-id="cc47b-123">id</span></span>|<span data-ttu-id="cc47b-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cc47b-124">String</span></span>|<span data-ttu-id="cc47b-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="cc47b-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="cc47b-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="cc47b-126">System generated value assigned when created.</span></span> <span data-ttu-id="cc47b-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="cc47b-128">uniqueName</span></span>|<span data-ttu-id="cc47b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="cc47b-129">String</span></span>|<span data-ttu-id="cc47b-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="cc47b-130">Unique name for the management condition.</span></span> <span data-ttu-id="cc47b-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-131">Used in management condition expressions.</span></span> <span data-ttu-id="cc47b-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cc47b-133">displayName</span></span>|<span data-ttu-id="cc47b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cc47b-134">String</span></span>|<span data-ttu-id="cc47b-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="cc47b-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="cc47b-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-137">описание</span><span class="sxs-lookup"><span data-stu-id="cc47b-137">description</span></span>|<span data-ttu-id="cc47b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="cc47b-138">String</span></span>|<span data-ttu-id="cc47b-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="cc47b-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="cc47b-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc47b-141">createdDateTime</span></span>|<span data-ttu-id="cc47b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc47b-142">DateTimeOffset</span></span>|<span data-ttu-id="cc47b-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-143">The time the management condition was created.</span></span> <span data-ttu-id="cc47b-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cc47b-144">Generated service side.</span></span> <span data-ttu-id="cc47b-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc47b-146">modifiedDateTime</span></span>|<span data-ttu-id="cc47b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc47b-147">DateTimeOffset</span></span>|<span data-ttu-id="cc47b-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-148">The time the management condition was last modified.</span></span> <span data-ttu-id="cc47b-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cc47b-149">Updated service side.</span></span> <span data-ttu-id="cc47b-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-151">eTag</span><span class="sxs-lookup"><span data-stu-id="cc47b-151">eTag</span></span>|<span data-ttu-id="cc47b-152">String</span><span class="sxs-lookup"><span data-stu-id="cc47b-152">String</span></span>|<span data-ttu-id="cc47b-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-153">ETag of the management condition.</span></span> <span data-ttu-id="cc47b-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="cc47b-154">Updated service side.</span></span> <span data-ttu-id="cc47b-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="cc47b-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="cc47b-156">applicablePlatforms</span></span>|<span data-ttu-id="cc47b-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cc47b-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="cc47b-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="cc47b-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc47b-160">Связи</span><span class="sxs-lookup"><span data-stu-id="cc47b-160">Relationships</span></span>
|<span data-ttu-id="cc47b-161">Связь</span><span class="sxs-lookup"><span data-stu-id="cc47b-161">Relationship</span></span>|<span data-ttu-id="cc47b-162">Тип</span><span class="sxs-lookup"><span data-stu-id="cc47b-162">Type</span></span>|<span data-ttu-id="cc47b-163">Описание</span><span class="sxs-lookup"><span data-stu-id="cc47b-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc47b-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="cc47b-164">managementConditionStatements</span></span>|<span data-ttu-id="cc47b-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cc47b-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="cc47b-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="cc47b-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="cc47b-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="cc47b-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc47b-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc47b-168">JSON Representation</span></span>
<span data-ttu-id="cc47b-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc47b-169">Here is a JSON representation of the resource.</span></span>
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





