---
title: Тип ресурса Манажементкондитион
description: Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb7f6ecb00072fb5280cb4033a39fb2041524b7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031384"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="af8dd-103">Тип ресурса Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="af8dd-103">managementCondition resource type</span></span>

<span data-ttu-id="af8dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af8dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af8dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af8dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af8dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af8dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af8dd-107">Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.</span><span class="sxs-lookup"><span data-stu-id="af8dd-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="af8dd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="af8dd-108">Methods</span></span>
|<span data-ttu-id="af8dd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="af8dd-109">Method</span></span>|<span data-ttu-id="af8dd-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="af8dd-110">Return Type</span></span>|<span data-ttu-id="af8dd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="af8dd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af8dd-112">Список Манажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="af8dd-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="af8dd-113">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="af8dd-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="af8dd-114">Список свойств и связей объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="af8dd-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="af8dd-115">Получение Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="af8dd-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="af8dd-116">манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="af8dd-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="af8dd-117">Чтение свойств и связей объекта [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="af8dd-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="af8dd-118">Функция Жетманажементкондитионсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="af8dd-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="af8dd-119">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="af8dd-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="af8dd-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af8dd-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="af8dd-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="af8dd-121">Properties</span></span>
|<span data-ttu-id="af8dd-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="af8dd-122">Property</span></span>|<span data-ttu-id="af8dd-123">Тип</span><span class="sxs-lookup"><span data-stu-id="af8dd-123">Type</span></span>|<span data-ttu-id="af8dd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="af8dd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8dd-125">id</span><span class="sxs-lookup"><span data-stu-id="af8dd-125">id</span></span>|<span data-ttu-id="af8dd-126">String</span><span class="sxs-lookup"><span data-stu-id="af8dd-126">String</span></span>|<span data-ttu-id="af8dd-127">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="af8dd-128">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="af8dd-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="af8dd-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="af8dd-129">uniqueName</span></span>|<span data-ttu-id="af8dd-130">String</span><span class="sxs-lookup"><span data-stu-id="af8dd-130">String</span></span>|<span data-ttu-id="af8dd-131">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-131">Unique name for the management condition.</span></span> <span data-ttu-id="af8dd-132">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="af8dd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="af8dd-133">displayName</span></span>|<span data-ttu-id="af8dd-134">String</span><span class="sxs-lookup"><span data-stu-id="af8dd-134">String</span></span>|<span data-ttu-id="af8dd-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="af8dd-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="af8dd-136">description</span><span class="sxs-lookup"><span data-stu-id="af8dd-136">description</span></span>|<span data-ttu-id="af8dd-137">String</span><span class="sxs-lookup"><span data-stu-id="af8dd-137">String</span></span>|<span data-ttu-id="af8dd-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="af8dd-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="af8dd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af8dd-139">createdDateTime</span></span>|<span data-ttu-id="af8dd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8dd-140">DateTimeOffset</span></span>|<span data-ttu-id="af8dd-141">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-141">The time the management condition was created.</span></span> <span data-ttu-id="af8dd-142">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="af8dd-142">Generated service side.</span></span>|
|<span data-ttu-id="af8dd-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af8dd-143">modifiedDateTime</span></span>|<span data-ttu-id="af8dd-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af8dd-144">DateTimeOffset</span></span>|<span data-ttu-id="af8dd-145">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-145">The time the management condition was last modified.</span></span> <span data-ttu-id="af8dd-146">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="af8dd-146">Updated service side.</span></span>|
|<span data-ttu-id="af8dd-147">eTag</span><span class="sxs-lookup"><span data-stu-id="af8dd-147">eTag</span></span>|<span data-ttu-id="af8dd-148">String</span><span class="sxs-lookup"><span data-stu-id="af8dd-148">String</span></span>|<span data-ttu-id="af8dd-149">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-149">ETag of the management condition.</span></span> <span data-ttu-id="af8dd-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="af8dd-150">Updated service side.</span></span>|
|<span data-ttu-id="af8dd-151">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="af8dd-151">applicablePlatforms</span></span>|<span data-ttu-id="af8dd-152">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="af8dd-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="af8dd-153">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af8dd-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="af8dd-154">Relationships</span></span>
|<span data-ttu-id="af8dd-155">Связь</span><span class="sxs-lookup"><span data-stu-id="af8dd-155">Relationship</span></span>|<span data-ttu-id="af8dd-156">Тип</span><span class="sxs-lookup"><span data-stu-id="af8dd-156">Type</span></span>|<span data-ttu-id="af8dd-157">Описание</span><span class="sxs-lookup"><span data-stu-id="af8dd-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af8dd-158">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="af8dd-158">managementConditionStatements</span></span>|<span data-ttu-id="af8dd-159">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="af8dd-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="af8dd-160">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="af8dd-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af8dd-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af8dd-161">JSON Representation</span></span>
<span data-ttu-id="af8dd-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af8dd-162">Here is a JSON representation of the resource.</span></span>
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






