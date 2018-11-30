---
title: Тип ресурса managementCondition
description: События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
ms.openlocfilehash: 3c2bc1d7594e61642b96398bfb55d6aa38f3283d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076843"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="0a4c3-103">Тип ресурса managementCondition</span><span class="sxs-lookup"><span data-stu-id="0a4c3-103">managementCondition resource type</span></span>

> <span data-ttu-id="0a4c3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a4c3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a4c3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a4c3-107">События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="0a4c3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0a4c3-108">Methods</span></span>
|<span data-ttu-id="0a4c3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0a4c3-109">Method</span></span>|<span data-ttu-id="0a4c3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0a4c3-110">Return Type</span></span>|<span data-ttu-id="0a4c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4c3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a4c3-112">Список managementConditions</span><span class="sxs-lookup"><span data-stu-id="0a4c3-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="0a4c3-113">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a4c3-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="0a4c3-114">Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0a4c3-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0a4c3-115">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="0a4c3-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="0a4c3-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="0a4c3-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="0a4c3-117">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0a4c3-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="0a4c3-118">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="0a4c3-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="0a4c3-119">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a4c3-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="0a4c3-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0a4c3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0a4c3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a4c3-121">Properties</span></span>
|<span data-ttu-id="0a4c3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a4c3-122">Property</span></span>|<span data-ttu-id="0a4c3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0a4c3-123">Type</span></span>|<span data-ttu-id="0a4c3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4c3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4c3-125">id</span><span class="sxs-lookup"><span data-stu-id="0a4c3-125">id</span></span>|<span data-ttu-id="0a4c3-126">String</span><span class="sxs-lookup"><span data-stu-id="0a4c3-126">String</span></span>|<span data-ttu-id="0a4c3-127">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="0a4c3-128">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0a4c3-129">уникального имени</span><span class="sxs-lookup"><span data-stu-id="0a4c3-129">uniqueName</span></span>|<span data-ttu-id="0a4c3-130">String</span><span class="sxs-lookup"><span data-stu-id="0a4c3-130">String</span></span>|<span data-ttu-id="0a4c3-131">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-131">Unique name for the management condition.</span></span> <span data-ttu-id="0a4c3-132">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="0a4c3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0a4c3-133">displayName</span></span>|<span data-ttu-id="0a4c3-134">String</span><span class="sxs-lookup"><span data-stu-id="0a4c3-134">String</span></span>|<span data-ttu-id="0a4c3-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="0a4c3-136">описание</span><span class="sxs-lookup"><span data-stu-id="0a4c3-136">description</span></span>|<span data-ttu-id="0a4c3-137">String</span><span class="sxs-lookup"><span data-stu-id="0a4c3-137">String</span></span>|<span data-ttu-id="0a4c3-138">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="0a4c3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a4c3-139">createdDateTime</span></span>|<span data-ttu-id="0a4c3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a4c3-140">DateTimeOffset</span></span>|<span data-ttu-id="0a4c3-141">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-141">The time the management condition was created.</span></span> <span data-ttu-id="0a4c3-142">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-142">Generated service side.</span></span>|
|<span data-ttu-id="0a4c3-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a4c3-143">modifiedDateTime</span></span>|<span data-ttu-id="0a4c3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a4c3-144">DateTimeOffset</span></span>|<span data-ttu-id="0a4c3-145">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-145">The time the management condition was last modified.</span></span> <span data-ttu-id="0a4c3-146">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-146">Updated service side.</span></span>|
|<span data-ttu-id="0a4c3-147">eTag</span><span class="sxs-lookup"><span data-stu-id="0a4c3-147">eTag</span></span>|<span data-ttu-id="0a4c3-148">String</span><span class="sxs-lookup"><span data-stu-id="0a4c3-148">String</span></span>|<span data-ttu-id="0a4c3-149">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-149">ETag of the management condition.</span></span> <span data-ttu-id="0a4c3-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-150">Updated service side.</span></span>|
|<span data-ttu-id="0a4c3-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="0a4c3-151">applicablePlatforms</span></span>|<span data-ttu-id="0a4c3-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a4c3-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0a4c3-153">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a4c3-154">Связи</span><span class="sxs-lookup"><span data-stu-id="0a4c3-154">Relationships</span></span>
|<span data-ttu-id="0a4c3-155">Связь</span><span class="sxs-lookup"><span data-stu-id="0a4c3-155">Relationship</span></span>|<span data-ttu-id="0a4c3-156">Тип</span><span class="sxs-lookup"><span data-stu-id="0a4c3-156">Type</span></span>|<span data-ttu-id="0a4c3-157">Description</span><span class="sxs-lookup"><span data-stu-id="0a4c3-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4c3-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="0a4c3-158">managementConditionStatements</span></span>|<span data-ttu-id="0a4c3-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="0a4c3-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0a4c3-160">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a4c3-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a4c3-161">JSON Representation</span></span>
<span data-ttu-id="0a4c3-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a4c3-162">Here is a JSON representation of the resource.</span></span>
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





