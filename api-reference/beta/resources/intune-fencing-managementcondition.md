---
title: Тип ресурса managementCondition
description: События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
localization_priority: Normal
ms.openlocfilehash: a836aeaa660de8f02c4e441e9eb390e1513c917c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834113"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="60ed5-103">Тип ресурса managementCondition</span><span class="sxs-lookup"><span data-stu-id="60ed5-103">managementCondition resource type</span></span>

> <span data-ttu-id="60ed5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="60ed5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60ed5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ed5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60ed5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="60ed5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60ed5-107">События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.</span><span class="sxs-lookup"><span data-stu-id="60ed5-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="60ed5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="60ed5-108">Methods</span></span>
|<span data-ttu-id="60ed5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="60ed5-109">Method</span></span>|<span data-ttu-id="60ed5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60ed5-110">Return Type</span></span>|<span data-ttu-id="60ed5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60ed5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60ed5-112">Список managementConditions</span><span class="sxs-lookup"><span data-stu-id="60ed5-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="60ed5-113">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="60ed5-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="60ed5-114">Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="60ed5-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="60ed5-115">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="60ed5-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="60ed5-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="60ed5-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="60ed5-117">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="60ed5-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="60ed5-118">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="60ed5-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="60ed5-119">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="60ed5-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="60ed5-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="60ed5-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="60ed5-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="60ed5-121">Properties</span></span>
|<span data-ttu-id="60ed5-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="60ed5-122">Property</span></span>|<span data-ttu-id="60ed5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="60ed5-123">Type</span></span>|<span data-ttu-id="60ed5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="60ed5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ed5-125">id</span><span class="sxs-lookup"><span data-stu-id="60ed5-125">id</span></span>|<span data-ttu-id="60ed5-126">Строка</span><span class="sxs-lookup"><span data-stu-id="60ed5-126">String</span></span>|<span data-ttu-id="60ed5-127">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="60ed5-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="60ed5-128">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="60ed5-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="60ed5-129">уникального имени</span><span class="sxs-lookup"><span data-stu-id="60ed5-129">uniqueName</span></span>|<span data-ttu-id="60ed5-130">Строка</span><span class="sxs-lookup"><span data-stu-id="60ed5-130">String</span></span>|<span data-ttu-id="60ed5-131">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="60ed5-131">Unique name for the management condition.</span></span> <span data-ttu-id="60ed5-132">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="60ed5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="60ed5-133">displayName</span></span>|<span data-ttu-id="60ed5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="60ed5-134">String</span></span>|<span data-ttu-id="60ed5-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="60ed5-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="60ed5-136">описание</span><span class="sxs-lookup"><span data-stu-id="60ed5-136">description</span></span>|<span data-ttu-id="60ed5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="60ed5-137">String</span></span>|<span data-ttu-id="60ed5-138">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="60ed5-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="60ed5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60ed5-139">createdDateTime</span></span>|<span data-ttu-id="60ed5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60ed5-140">DateTimeOffset</span></span>|<span data-ttu-id="60ed5-141">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-141">The time the management condition was created.</span></span> <span data-ttu-id="60ed5-142">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="60ed5-142">Generated service side.</span></span>|
|<span data-ttu-id="60ed5-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60ed5-143">modifiedDateTime</span></span>|<span data-ttu-id="60ed5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60ed5-144">DateTimeOffset</span></span>|<span data-ttu-id="60ed5-145">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-145">The time the management condition was last modified.</span></span> <span data-ttu-id="60ed5-146">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="60ed5-146">Updated service side.</span></span>|
|<span data-ttu-id="60ed5-147">eTag</span><span class="sxs-lookup"><span data-stu-id="60ed5-147">eTag</span></span>|<span data-ttu-id="60ed5-148">String</span><span class="sxs-lookup"><span data-stu-id="60ed5-148">String</span></span>|<span data-ttu-id="60ed5-149">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-149">ETag of the management condition.</span></span> <span data-ttu-id="60ed5-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="60ed5-150">Updated service side.</span></span>|
|<span data-ttu-id="60ed5-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="60ed5-151">applicablePlatforms</span></span>|<span data-ttu-id="60ed5-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="60ed5-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="60ed5-153">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60ed5-154">Связи</span><span class="sxs-lookup"><span data-stu-id="60ed5-154">Relationships</span></span>
|<span data-ttu-id="60ed5-155">Связь</span><span class="sxs-lookup"><span data-stu-id="60ed5-155">Relationship</span></span>|<span data-ttu-id="60ed5-156">Тип</span><span class="sxs-lookup"><span data-stu-id="60ed5-156">Type</span></span>|<span data-ttu-id="60ed5-157">Описание</span><span class="sxs-lookup"><span data-stu-id="60ed5-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ed5-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="60ed5-158">managementConditionStatements</span></span>|<span data-ttu-id="60ed5-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="60ed5-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="60ed5-160">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="60ed5-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60ed5-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60ed5-161">JSON Representation</span></span>
<span data-ttu-id="60ed5-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60ed5-162">Here is a JSON representation of the resource.</span></span>
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





