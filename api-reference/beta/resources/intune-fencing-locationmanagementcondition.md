---
title: Тип ресурса locationManagementCondition
description: Содержит данные для определения условие управления расположение области интересов, мониторинг.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 541cf74decad641f6dc7751945e1d0ffceee1366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922979"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="02275-103">Тип ресурса locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="02275-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="02275-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02275-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02275-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02275-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02275-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02275-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02275-107">Содержит данные для определения условие управления расположение области интересов, мониторинг.</span><span class="sxs-lookup"><span data-stu-id="02275-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>

<span data-ttu-id="02275-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="02275-109">Методы</span><span class="sxs-lookup"><span data-stu-id="02275-109">Methods</span></span>
|<span data-ttu-id="02275-110">Метод</span><span class="sxs-lookup"><span data-stu-id="02275-110">Method</span></span>|<span data-ttu-id="02275-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="02275-111">Return Type</span></span>|<span data-ttu-id="02275-112">Описание</span><span class="sxs-lookup"><span data-stu-id="02275-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="02275-113">Список locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="02275-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="02275-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="02275-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="02275-115">Свойства списка и связей объектов [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="02275-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="02275-116">Получение locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="02275-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="02275-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="02275-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="02275-118">Чтение свойства и связи объекта [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="02275-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="02275-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="02275-119">Properties</span></span>
|<span data-ttu-id="02275-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="02275-120">Property</span></span>|<span data-ttu-id="02275-121">Тип</span><span class="sxs-lookup"><span data-stu-id="02275-121">Type</span></span>|<span data-ttu-id="02275-122">Описание</span><span class="sxs-lookup"><span data-stu-id="02275-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02275-123">id</span><span class="sxs-lookup"><span data-stu-id="02275-123">id</span></span>|<span data-ttu-id="02275-124">Строка</span><span class="sxs-lookup"><span data-stu-id="02275-124">String</span></span>|<span data-ttu-id="02275-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="02275-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="02275-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="02275-126">System generated value assigned when created.</span></span> <span data-ttu-id="02275-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="02275-128">uniqueName</span></span>|<span data-ttu-id="02275-129">Строка</span><span class="sxs-lookup"><span data-stu-id="02275-129">String</span></span>|<span data-ttu-id="02275-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="02275-130">Unique name for the management condition.</span></span> <span data-ttu-id="02275-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="02275-131">Used in management condition expressions.</span></span> <span data-ttu-id="02275-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-133">displayName</span><span class="sxs-lookup"><span data-stu-id="02275-133">displayName</span></span>|<span data-ttu-id="02275-134">Строка</span><span class="sxs-lookup"><span data-stu-id="02275-134">String</span></span>|<span data-ttu-id="02275-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="02275-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="02275-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-137">описание</span><span class="sxs-lookup"><span data-stu-id="02275-137">description</span></span>|<span data-ttu-id="02275-138">Строка</span><span class="sxs-lookup"><span data-stu-id="02275-138">String</span></span>|<span data-ttu-id="02275-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="02275-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="02275-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02275-141">createdDateTime</span></span>|<span data-ttu-id="02275-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02275-142">DateTimeOffset</span></span>|<span data-ttu-id="02275-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="02275-143">The time the management condition was created.</span></span> <span data-ttu-id="02275-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="02275-144">Generated service side.</span></span> <span data-ttu-id="02275-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02275-146">modifiedDateTime</span></span>|<span data-ttu-id="02275-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02275-147">DateTimeOffset</span></span>|<span data-ttu-id="02275-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="02275-148">The time the management condition was last modified.</span></span> <span data-ttu-id="02275-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="02275-149">Updated service side.</span></span> <span data-ttu-id="02275-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-151">eTag</span><span class="sxs-lookup"><span data-stu-id="02275-151">eTag</span></span>|<span data-ttu-id="02275-152">String</span><span class="sxs-lookup"><span data-stu-id="02275-152">String</span></span>|<span data-ttu-id="02275-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="02275-153">ETag of the management condition.</span></span> <span data-ttu-id="02275-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="02275-154">Updated service side.</span></span> <span data-ttu-id="02275-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="02275-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="02275-156">applicablePlatforms</span></span>|<span data-ttu-id="02275-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="02275-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="02275-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="02275-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="02275-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="02275-160">Связи</span><span class="sxs-lookup"><span data-stu-id="02275-160">Relationships</span></span>
|<span data-ttu-id="02275-161">Связь</span><span class="sxs-lookup"><span data-stu-id="02275-161">Relationship</span></span>|<span data-ttu-id="02275-162">Тип</span><span class="sxs-lookup"><span data-stu-id="02275-162">Type</span></span>|<span data-ttu-id="02275-163">Описание</span><span class="sxs-lookup"><span data-stu-id="02275-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02275-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="02275-164">managementConditionStatements</span></span>|<span data-ttu-id="02275-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="02275-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="02275-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="02275-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="02275-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="02275-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02275-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02275-168">JSON Representation</span></span>
<span data-ttu-id="02275-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02275-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
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





