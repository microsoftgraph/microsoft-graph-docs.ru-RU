---
title: Тип ресурса networkManagementCondition
description: Содержит данные для определения состояния управления сети.
author: tfitzmac
ms.openlocfilehash: d906520d30b78b0acdb1f33d7b4d7046d84c53e1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347595"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="74f43-103">Тип ресурса networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="74f43-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="74f43-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74f43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74f43-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74f43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74f43-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="74f43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74f43-107">Содержит данные для определения состояния управления сети.</span><span class="sxs-lookup"><span data-stu-id="74f43-107">Contains the information to define a network management condition.</span></span>

<span data-ttu-id="74f43-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="74f43-109">Методы</span><span class="sxs-lookup"><span data-stu-id="74f43-109">Methods</span></span>
|<span data-ttu-id="74f43-110">Метод</span><span class="sxs-lookup"><span data-stu-id="74f43-110">Method</span></span>|<span data-ttu-id="74f43-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74f43-111">Return Type</span></span>|<span data-ttu-id="74f43-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74f43-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74f43-113">Список networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="74f43-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="74f43-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="74f43-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="74f43-115">Свойства списка и связей объектов [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="74f43-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="74f43-116">Получение networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="74f43-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="74f43-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="74f43-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="74f43-118">Чтение свойства и связи объекта [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="74f43-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74f43-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="74f43-119">Properties</span></span>
|<span data-ttu-id="74f43-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="74f43-120">Property</span></span>|<span data-ttu-id="74f43-121">Тип</span><span class="sxs-lookup"><span data-stu-id="74f43-121">Type</span></span>|<span data-ttu-id="74f43-122">Описание</span><span class="sxs-lookup"><span data-stu-id="74f43-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f43-123">id</span><span class="sxs-lookup"><span data-stu-id="74f43-123">id</span></span>|<span data-ttu-id="74f43-124">Строка</span><span class="sxs-lookup"><span data-stu-id="74f43-124">String</span></span>|<span data-ttu-id="74f43-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="74f43-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="74f43-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="74f43-126">System generated value assigned when created.</span></span> <span data-ttu-id="74f43-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="74f43-128">uniqueName</span></span>|<span data-ttu-id="74f43-129">String.</span><span class="sxs-lookup"><span data-stu-id="74f43-129">String</span></span>|<span data-ttu-id="74f43-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="74f43-130">Unique name for the management condition.</span></span> <span data-ttu-id="74f43-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-131">Used in management condition expressions.</span></span> <span data-ttu-id="74f43-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-133">displayName</span><span class="sxs-lookup"><span data-stu-id="74f43-133">displayName</span></span>|<span data-ttu-id="74f43-134">Строка</span><span class="sxs-lookup"><span data-stu-id="74f43-134">String</span></span>|<span data-ttu-id="74f43-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="74f43-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="74f43-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-137">описание</span><span class="sxs-lookup"><span data-stu-id="74f43-137">description</span></span>|<span data-ttu-id="74f43-138">Строка</span><span class="sxs-lookup"><span data-stu-id="74f43-138">String</span></span>|<span data-ttu-id="74f43-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="74f43-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="74f43-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74f43-141">createdDateTime</span></span>|<span data-ttu-id="74f43-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f43-142">DateTimeOffset</span></span>|<span data-ttu-id="74f43-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-143">The time the management condition was created.</span></span> <span data-ttu-id="74f43-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="74f43-144">Generated service side.</span></span> <span data-ttu-id="74f43-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74f43-146">modifiedDateTime</span></span>|<span data-ttu-id="74f43-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74f43-147">DateTimeOffset</span></span>|<span data-ttu-id="74f43-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-148">The time the management condition was last modified.</span></span> <span data-ttu-id="74f43-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="74f43-149">Updated service side.</span></span> <span data-ttu-id="74f43-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-151">eTag</span><span class="sxs-lookup"><span data-stu-id="74f43-151">eTag</span></span>|<span data-ttu-id="74f43-152">String</span><span class="sxs-lookup"><span data-stu-id="74f43-152">String</span></span>|<span data-ttu-id="74f43-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-153">ETag of the management condition.</span></span> <span data-ttu-id="74f43-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="74f43-154">Updated service side.</span></span> <span data-ttu-id="74f43-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="74f43-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="74f43-156">applicablePlatforms</span></span>|<span data-ttu-id="74f43-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="74f43-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="74f43-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="74f43-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="74f43-160">Связи</span><span class="sxs-lookup"><span data-stu-id="74f43-160">Relationships</span></span>
|<span data-ttu-id="74f43-161">Связь</span><span class="sxs-lookup"><span data-stu-id="74f43-161">Relationship</span></span>|<span data-ttu-id="74f43-162">Тип</span><span class="sxs-lookup"><span data-stu-id="74f43-162">Type</span></span>|<span data-ttu-id="74f43-163">Описание</span><span class="sxs-lookup"><span data-stu-id="74f43-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f43-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="74f43-164">managementConditionStatements</span></span>|<span data-ttu-id="74f43-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="74f43-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="74f43-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="74f43-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="74f43-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="74f43-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74f43-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74f43-168">JSON Representation</span></span>
<span data-ttu-id="74f43-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74f43-169">Here is a JSON representation of the resource.</span></span>
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





