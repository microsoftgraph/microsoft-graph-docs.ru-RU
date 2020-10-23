---
title: Тип ресурса Манажементкондитион
description: Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9707268f648edc60ab7b37292b6e59f7721d983
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722874"
---
# <a name="managementcondition-resource-type"></a><span data-ttu-id="db18d-103">Тип ресурса Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="db18d-103">managementCondition resource type</span></span>

<span data-ttu-id="db18d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db18d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db18d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db18d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db18d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db18d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db18d-107">Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.</span><span class="sxs-lookup"><span data-stu-id="db18d-107">Management conditions are events that can be triggered dynamically such as geo-fences, time-fences, and network-fences.</span></span>

## <a name="methods"></a><span data-ttu-id="db18d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="db18d-108">Methods</span></span>
|<span data-ttu-id="db18d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="db18d-109">Method</span></span>|<span data-ttu-id="db18d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db18d-110">Return Type</span></span>|<span data-ttu-id="db18d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db18d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db18d-112">Список Манажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="db18d-112">List managementConditions</span></span>](../api/intune-fencing-managementcondition-list.md)|<span data-ttu-id="db18d-113">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="db18d-113">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="db18d-114">Список свойств и связей объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="db18d-114">List properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) objects.</span></span>|
|[<span data-ttu-id="db18d-115">Получение Манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="db18d-115">Get managementCondition</span></span>](../api/intune-fencing-managementcondition-get.md)|[<span data-ttu-id="db18d-116">манажементкондитион</span><span class="sxs-lookup"><span data-stu-id="db18d-116">managementCondition</span></span>](../resources/intune-fencing-managementcondition.md)|<span data-ttu-id="db18d-117">Чтение свойств и связей объекта [манажементкондитион](../resources/intune-fencing-managementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="db18d-117">Read properties and relationships of the [managementCondition](../resources/intune-fencing-managementcondition.md) object.</span></span>|
|[<span data-ttu-id="db18d-118">Функция Жетманажементкондитионсфорплатформ</span><span class="sxs-lookup"><span data-stu-id="db18d-118">getManagementConditionsForPlatform function</span></span>](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|<span data-ttu-id="db18d-119">Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="db18d-119">[managementCondition](../resources/intune-fencing-managementcondition.md) collection</span></span>|<span data-ttu-id="db18d-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="db18d-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="db18d-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="db18d-121">Properties</span></span>
|<span data-ttu-id="db18d-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="db18d-122">Property</span></span>|<span data-ttu-id="db18d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="db18d-123">Type</span></span>|<span data-ttu-id="db18d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="db18d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db18d-125">id</span><span class="sxs-lookup"><span data-stu-id="db18d-125">id</span></span>|<span data-ttu-id="db18d-126">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-126">String</span></span>|<span data-ttu-id="db18d-127">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-127">Unique identifier for the management condition.</span></span> <span data-ttu-id="db18d-128">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="db18d-128">System generated value assigned when created.</span></span>|
|<span data-ttu-id="db18d-129">uniqueName</span><span class="sxs-lookup"><span data-stu-id="db18d-129">uniqueName</span></span>|<span data-ttu-id="db18d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-130">String</span></span>|<span data-ttu-id="db18d-131">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-131">Unique name for the management condition.</span></span> <span data-ttu-id="db18d-132">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-132">Used in management condition expressions.</span></span>|
|<span data-ttu-id="db18d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="db18d-133">displayName</span></span>|<span data-ttu-id="db18d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-134">String</span></span>|<span data-ttu-id="db18d-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="db18d-135">The admin defined name of the management condition.</span></span>|
|<span data-ttu-id="db18d-136">description</span><span class="sxs-lookup"><span data-stu-id="db18d-136">description</span></span>|<span data-ttu-id="db18d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="db18d-137">String</span></span>|<span data-ttu-id="db18d-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="db18d-138">The admin defined description of the management condition.</span></span>|
|<span data-ttu-id="db18d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db18d-139">createdDateTime</span></span>|<span data-ttu-id="db18d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db18d-140">DateTimeOffset</span></span>|<span data-ttu-id="db18d-141">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-141">The time the management condition was created.</span></span> <span data-ttu-id="db18d-142">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="db18d-142">Generated service side.</span></span>|
|<span data-ttu-id="db18d-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db18d-143">modifiedDateTime</span></span>|<span data-ttu-id="db18d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db18d-144">DateTimeOffset</span></span>|<span data-ttu-id="db18d-145">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-145">The time the management condition was last modified.</span></span> <span data-ttu-id="db18d-146">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="db18d-146">Updated service side.</span></span>|
|<span data-ttu-id="db18d-147">eTag</span><span class="sxs-lookup"><span data-stu-id="db18d-147">eTag</span></span>|<span data-ttu-id="db18d-148">String</span><span class="sxs-lookup"><span data-stu-id="db18d-148">String</span></span>|<span data-ttu-id="db18d-149">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-149">ETag of the management condition.</span></span> <span data-ttu-id="db18d-150">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="db18d-150">Updated service side.</span></span>|
|<span data-ttu-id="db18d-151">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="db18d-151">applicablePlatforms</span></span>|<span data-ttu-id="db18d-152">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="db18d-152">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="db18d-153">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-153">The applicable platforms for this management condition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db18d-154">Связи</span><span class="sxs-lookup"><span data-stu-id="db18d-154">Relationships</span></span>
|<span data-ttu-id="db18d-155">Связь</span><span class="sxs-lookup"><span data-stu-id="db18d-155">Relationship</span></span>|<span data-ttu-id="db18d-156">Тип</span><span class="sxs-lookup"><span data-stu-id="db18d-156">Type</span></span>|<span data-ttu-id="db18d-157">Описание</span><span class="sxs-lookup"><span data-stu-id="db18d-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db18d-158">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="db18d-158">managementConditionStatements</span></span>|<span data-ttu-id="db18d-159">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="db18d-159">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="db18d-160">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="db18d-160">The management condition statements associated to the management condition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db18d-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db18d-161">JSON Representation</span></span>
<span data-ttu-id="db18d-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db18d-162">Here is a JSON representation of the resource.</span></span>
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





