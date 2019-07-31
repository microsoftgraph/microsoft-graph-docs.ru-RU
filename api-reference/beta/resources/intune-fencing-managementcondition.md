---
title: Тип ресурса Манажементкондитион
description: Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41fbe4c93788bfea3f581e4e0788554485f703c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998704"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="24940-103">Тип ресурса Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="24940-103">managementCondition resource type</span></span>

> <span data-ttu-id="24940-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24940-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24940-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24940-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24940-106">Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.</span><span class="sxs-lookup"><span data-stu-id="24940-106">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="24940-107">Методы</span><span class="sxs-lookup"><span data-stu-id="24940-107">Methods</span></span>
|<span data-ttu-id="24940-108">Метод</span><span class="sxs-lookup"><span data-stu-id="24940-108">Method</span></span>|<span data-ttu-id="24940-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24940-109">Return Type</span></span>|<span data-ttu-id="24940-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24940-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24940-111">Список Манажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="24940-111">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="24940-112">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="24940-112">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="24940-113">Список свойств и связей объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="24940-113">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="24940-114">Получение Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="24940-114">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="24940-115">Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="24940-115">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="24940-116">Чтение свойств и связей объекта [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="24940-116">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="24940-117">Функция Жетманажементкондитионсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="24940-117">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="24940-118">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="24940-118">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="24940-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="24940-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="24940-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="24940-120">Properties</span></span>
|<span data-ttu-id="24940-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="24940-121">Property</span></span>|<span data-ttu-id="24940-122">Тип</span><span class="sxs-lookup"><span data-stu-id="24940-122">Type</span></span>|<span data-ttu-id="24940-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24940-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24940-124">id</span><span class="sxs-lookup"><span data-stu-id="24940-124">id</span></span>|<span data-ttu-id="24940-125">String</span><span class="sxs-lookup"><span data-stu-id="24940-125">String</span></span>|<span data-ttu-id="24940-126">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-126">Unique identifier for the management condition.</span></span> <span data-ttu-id="24940-127">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="24940-127">System generated value assigned when created.</span></span>|
|<span data-ttu-id="24940-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="24940-128">uniqueName</span></span>|<span data-ttu-id="24940-129">String</span><span class="sxs-lookup"><span data-stu-id="24940-129">String</span></span>|<span data-ttu-id="24940-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-130">Unique name for the management condition.</span></span> <span data-ttu-id="24940-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-131">Used in management condition expressions.</span></span>|
|<span data-ttu-id="24940-132">displayName</span><span class="sxs-lookup"><span data-stu-id="24940-132">displayName</span></span>|<span data-ttu-id="24940-133">Строка</span><span class="sxs-lookup"><span data-stu-id="24940-133">String</span></span>|<span data-ttu-id="24940-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="24940-134">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="24940-135">description</span><span class="sxs-lookup"><span data-stu-id="24940-135">description</span></span>|<span data-ttu-id="24940-136">String</span><span class="sxs-lookup"><span data-stu-id="24940-136">String</span></span>|<span data-ttu-id="24940-137">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="24940-137">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="24940-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24940-138">createdDateTime</span></span>|<span data-ttu-id="24940-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24940-139">DateTimeOffset</span></span>|<span data-ttu-id="24940-140">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-140">The time the management condition was created.</span></span> <span data-ttu-id="24940-141">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="24940-141">Generated service side.</span></span>|
|<span data-ttu-id="24940-142">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24940-142">modifiedDateTime</span></span>|<span data-ttu-id="24940-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24940-143">DateTimeOffset</span></span>|<span data-ttu-id="24940-144">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-144">The time the management condition was last modified.</span></span> <span data-ttu-id="24940-145">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="24940-145">Updated service side.</span></span>|
|<span data-ttu-id="24940-146">eTag</span><span class="sxs-lookup"><span data-stu-id="24940-146">eTag</span></span>|<span data-ttu-id="24940-147">String</span><span class="sxs-lookup"><span data-stu-id="24940-147">String</span></span>|<span data-ttu-id="24940-148">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-148">ETag of the management condition.</span></span> <span data-ttu-id="24940-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="24940-149">Updated service side.</span></span>|
|<span data-ttu-id="24940-150">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="24940-150">applicablePlatforms</span></span>|<span data-ttu-id="24940-151">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="24940-151">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="24940-152">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="24940-152">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24940-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="24940-153">Relationships</span></span>
|<span data-ttu-id="24940-154">Отношение</span><span class="sxs-lookup"><span data-stu-id="24940-154">Relationship</span></span>|<span data-ttu-id="24940-155">Тип</span><span class="sxs-lookup"><span data-stu-id="24940-155">Type</span></span>|<span data-ttu-id="24940-156">Описание</span><span class="sxs-lookup"><span data-stu-id="24940-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24940-157">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="24940-157">managementConditionStatements</span></span>|<span data-ttu-id="24940-158">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="24940-158">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="24940-159">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="24940-159">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24940-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24940-160">JSON Representation</span></span>
<span data-ttu-id="24940-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24940-161">Here is a JSON representation of the resource.</span></span>
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





