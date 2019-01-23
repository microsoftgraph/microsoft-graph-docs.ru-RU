---
title: Тип ресурса managementCondition
description: События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405858"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="d8bdc-103">Тип ресурса managementCondition</span><span class="sxs-lookup"><span data-stu-id="d8bdc-103">managementCondition resource type</span></span>

> <span data-ttu-id="d8bdc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8bdc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8bdc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8bdc-107">События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="d8bdc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d8bdc-108">Methods</span></span>
|<span data-ttu-id="d8bdc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d8bdc-109">Method</span></span>|<span data-ttu-id="d8bdc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8bdc-110">Return Type</span></span>|<span data-ttu-id="d8bdc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8bdc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8bdc-112">Список managementConditions</span><span class="sxs-lookup"><span data-stu-id="d8bdc-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="d8bdc-113">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d8bdc-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="d8bdc-114">Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bdc-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="d8bdc-115">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="d8bdc-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="d8bdc-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="d8bdc-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="d8bdc-117">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="d8bdc-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="d8bdc-118">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="d8bdc-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="d8bdc-119">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d8bdc-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="d8bdc-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d8bdc-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d8bdc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8bdc-121">Properties</span></span>
|<span data-ttu-id="d8bdc-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8bdc-122">Property</span></span>|<span data-ttu-id="d8bdc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d8bdc-123">Type</span></span>|<span data-ttu-id="d8bdc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8bdc-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bdc-125">id</span><span class="sxs-lookup"><span data-stu-id="d8bdc-125">id</span></span>|<span data-ttu-id="d8bdc-126">String</span><span class="sxs-lookup"><span data-stu-id="d8bdc-126">String</span></span>|<span data-ttu-id="d8bdc-127">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="d8bdc-128">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d8bdc-129">уникального имени</span><span class="sxs-lookup"><span data-stu-id="d8bdc-129">uniqueName</span></span>|<span data-ttu-id="d8bdc-130">String</span><span class="sxs-lookup"><span data-stu-id="d8bdc-130">String</span></span>|<span data-ttu-id="d8bdc-131">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-131">Unique name for the management condition.</span></span> <span data-ttu-id="d8bdc-132">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="d8bdc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d8bdc-133">displayName</span></span>|<span data-ttu-id="d8bdc-134">String</span><span class="sxs-lookup"><span data-stu-id="d8bdc-134">String</span></span>|<span data-ttu-id="d8bdc-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="d8bdc-136">description</span><span class="sxs-lookup"><span data-stu-id="d8bdc-136">description</span></span>|<span data-ttu-id="d8bdc-137">String</span><span class="sxs-lookup"><span data-stu-id="d8bdc-137">String</span></span>|<span data-ttu-id="d8bdc-138">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="d8bdc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8bdc-139">createdDateTime</span></span>|<span data-ttu-id="d8bdc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8bdc-140">DateTimeOffset</span></span>|<span data-ttu-id="d8bdc-141">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-141">The time the management condition was created.</span></span> <span data-ttu-id="d8bdc-142">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-142">Generated service side.</span></span>|
|<span data-ttu-id="d8bdc-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8bdc-143">modifiedDateTime</span></span>|<span data-ttu-id="d8bdc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8bdc-144">DateTimeOffset</span></span>|<span data-ttu-id="d8bdc-145">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-145">The time the management condition was last modified.</span></span> <span data-ttu-id="d8bdc-146">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-146">Updated service side.</span></span>|
|<span data-ttu-id="d8bdc-147">eTag</span><span class="sxs-lookup"><span data-stu-id="d8bdc-147">eTag</span></span>|<span data-ttu-id="d8bdc-148">String</span><span class="sxs-lookup"><span data-stu-id="d8bdc-148">String</span></span>|<span data-ttu-id="d8bdc-149">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-149">ETag of the management condition.</span></span> <span data-ttu-id="d8bdc-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-150">Updated service side.</span></span>|
|<span data-ttu-id="d8bdc-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d8bdc-151">applicablePlatforms</span></span>|<span data-ttu-id="d8bdc-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d8bdc-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d8bdc-153">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8bdc-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="d8bdc-154">Relationships</span></span>
|<span data-ttu-id="d8bdc-155">Связь</span><span class="sxs-lookup"><span data-stu-id="d8bdc-155">Relationship</span></span>|<span data-ttu-id="d8bdc-156">Тип</span><span class="sxs-lookup"><span data-stu-id="d8bdc-156">Type</span></span>|<span data-ttu-id="d8bdc-157">Описание</span><span class="sxs-lookup"><span data-stu-id="d8bdc-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bdc-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="d8bdc-158">managementConditionStatements</span></span>|<span data-ttu-id="d8bdc-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="d8bdc-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="d8bdc-160">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8bdc-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8bdc-161">JSON Representation</span></span>
<span data-ttu-id="d8bdc-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8bdc-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




