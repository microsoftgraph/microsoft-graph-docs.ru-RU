---
title: Тип ресурса managementCondition
description: События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986744"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="782d1-103">Тип ресурса managementCondition</span><span class="sxs-lookup"><span data-stu-id="782d1-103">managementCondition resource type</span></span>

> <span data-ttu-id="782d1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="782d1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="782d1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="782d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="782d1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="782d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="782d1-107">События, например географически границы, может быть запущено динамически выполняются условия управления временные границы и границы сети.</span><span class="sxs-lookup"><span data-stu-id="782d1-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>
## <a name="methods"></a><span data-ttu-id="782d1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="782d1-108">Methods</span></span>
|<span data-ttu-id="782d1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="782d1-109">Method</span></span>|<span data-ttu-id="782d1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="782d1-110">Return Type</span></span>|<span data-ttu-id="782d1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="782d1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="782d1-112">Список managementConditions</span><span class="sxs-lookup"><span data-stu-id="782d1-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="782d1-113">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="782d1-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="782d1-114">Свойства списка и связей объектов [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="782d1-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="782d1-115">Получение managementCondition</span><span class="sxs-lookup"><span data-stu-id="782d1-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="782d1-116">managementCondition</span><span class="sxs-lookup"><span data-stu-id="782d1-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="782d1-117">Чтение свойства и связи объекта [managementCondition](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="782d1-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="782d1-118">функция getManagementConditionsForPlatform</span><span class="sxs-lookup"><span data-stu-id="782d1-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="782d1-119">[managementCondition](../resources/intune-fencing-managementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="782d1-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="782d1-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="782d1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="782d1-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="782d1-121">Properties</span></span>
|<span data-ttu-id="782d1-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="782d1-122">Property</span></span>|<span data-ttu-id="782d1-123">Тип</span><span class="sxs-lookup"><span data-stu-id="782d1-123">Type</span></span>|<span data-ttu-id="782d1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="782d1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="782d1-125">id</span><span class="sxs-lookup"><span data-stu-id="782d1-125">id</span></span>|<span data-ttu-id="782d1-126">Строка</span><span class="sxs-lookup"><span data-stu-id="782d1-126">String</span></span>|<span data-ttu-id="782d1-127">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="782d1-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="782d1-128">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="782d1-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="782d1-129">уникального имени</span><span class="sxs-lookup"><span data-stu-id="782d1-129">uniqueName</span></span>|<span data-ttu-id="782d1-130">Строка</span><span class="sxs-lookup"><span data-stu-id="782d1-130">String</span></span>|<span data-ttu-id="782d1-131">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="782d1-131">Unique name for the management condition.</span></span> <span data-ttu-id="782d1-132">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="782d1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="782d1-133">displayName</span></span>|<span data-ttu-id="782d1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="782d1-134">String</span></span>|<span data-ttu-id="782d1-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="782d1-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="782d1-136">описание</span><span class="sxs-lookup"><span data-stu-id="782d1-136">description</span></span>|<span data-ttu-id="782d1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="782d1-137">String</span></span>|<span data-ttu-id="782d1-138">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="782d1-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="782d1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="782d1-139">createdDateTime</span></span>|<span data-ttu-id="782d1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="782d1-140">DateTimeOffset</span></span>|<span data-ttu-id="782d1-141">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-141">The time the management condition was created.</span></span> <span data-ttu-id="782d1-142">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="782d1-142">Generated service side.</span></span>|
|<span data-ttu-id="782d1-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="782d1-143">modifiedDateTime</span></span>|<span data-ttu-id="782d1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="782d1-144">DateTimeOffset</span></span>|<span data-ttu-id="782d1-145">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-145">The time the management condition was last modified.</span></span> <span data-ttu-id="782d1-146">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="782d1-146">Updated service side.</span></span>|
|<span data-ttu-id="782d1-147">eTag</span><span class="sxs-lookup"><span data-stu-id="782d1-147">eTag</span></span>|<span data-ttu-id="782d1-148">String</span><span class="sxs-lookup"><span data-stu-id="782d1-148">String</span></span>|<span data-ttu-id="782d1-149">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-149">ETag of the management condition.</span></span> <span data-ttu-id="782d1-150">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="782d1-150">Updated service side.</span></span>|
|<span data-ttu-id="782d1-151">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="782d1-151">applicablePlatforms</span></span>|<span data-ttu-id="782d1-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="782d1-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="782d1-153">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="782d1-154">Связи</span><span class="sxs-lookup"><span data-stu-id="782d1-154">Relationships</span></span>
|<span data-ttu-id="782d1-155">Связь</span><span class="sxs-lookup"><span data-stu-id="782d1-155">Relationship</span></span>|<span data-ttu-id="782d1-156">Тип</span><span class="sxs-lookup"><span data-stu-id="782d1-156">Type</span></span>|<span data-ttu-id="782d1-157">Описание</span><span class="sxs-lookup"><span data-stu-id="782d1-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="782d1-158">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="782d1-158">managementConditionStatements</span></span>|<span data-ttu-id="782d1-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="782d1-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="782d1-160">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="782d1-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="782d1-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="782d1-161">JSON Representation</span></span>
<span data-ttu-id="782d1-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="782d1-162">Here is a JSON representation of the resource.</span></span>
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





