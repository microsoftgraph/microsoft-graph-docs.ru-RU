---
title: Тип ресурса settingStateDeviceSummary
description: Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2104998cfdd65659114b1850d3cfcf1392bf9642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925877"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="6b93d-103">Тип ресурса settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="6b93d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b93d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b93d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b93d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b93d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b93d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b93d-107">Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств</span><span class="sxs-lookup"><span data-stu-id="6b93d-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="6b93d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6b93d-108">Methods</span></span>
|<span data-ttu-id="6b93d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6b93d-109">Method</span></span>|<span data-ttu-id="6b93d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6b93d-110">Return Type</span></span>|<span data-ttu-id="6b93d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6b93d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b93d-112">Список объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="6b93d-113">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="6b93d-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="6b93d-114">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b93d-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="6b93d-115">Получение объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="6b93d-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b93d-117">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b93d-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6b93d-118">Создание объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="6b93d-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b93d-120">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b93d-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="6b93d-121">Удаление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="6b93d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6b93d-122">None</span></span>|<span data-ttu-id="6b93d-123">Удаляет объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b93d-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="6b93d-124">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="6b93d-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6b93d-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="6b93d-126">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b93d-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b93d-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b93d-127">Properties</span></span>
|<span data-ttu-id="6b93d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b93d-128">Property</span></span>|<span data-ttu-id="6b93d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6b93d-129">Type</span></span>|<span data-ttu-id="6b93d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6b93d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b93d-131">id</span><span class="sxs-lookup"><span data-stu-id="6b93d-131">id</span></span>|<span data-ttu-id="6b93d-132">String</span><span class="sxs-lookup"><span data-stu-id="6b93d-132">String</span></span>|<span data-ttu-id="6b93d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b93d-133">Key of the entity.</span></span>|
|<span data-ttu-id="6b93d-134">settingName</span><span class="sxs-lookup"><span data-stu-id="6b93d-134">settingName</span></span>|<span data-ttu-id="6b93d-135">String</span><span class="sxs-lookup"><span data-stu-id="6b93d-135">String</span></span>|<span data-ttu-id="6b93d-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-136">Name of the setting</span></span>|
|<span data-ttu-id="6b93d-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="6b93d-137">instancePath</span></span>|<span data-ttu-id="6b93d-138">String</span><span class="sxs-lookup"><span data-stu-id="6b93d-138">String</span></span>|<span data-ttu-id="6b93d-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="6b93d-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-140">unknownDeviceCount</span></span>|<span data-ttu-id="6b93d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-141">Int32</span></span>|<span data-ttu-id="6b93d-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="6b93d-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="6b93d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-144">Int32</span></span>|<span data-ttu-id="6b93d-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="6b93d-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-146">compliantDeviceCount</span></span>|<span data-ttu-id="6b93d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-147">Int32</span></span>|<span data-ttu-id="6b93d-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6b93d-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-149">remediatedDeviceCount</span></span>|<span data-ttu-id="6b93d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-150">Int32</span></span>|<span data-ttu-id="6b93d-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="6b93d-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="6b93d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-153">Int32</span></span>|<span data-ttu-id="6b93d-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="6b93d-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-155">errorDeviceCount</span></span>|<span data-ttu-id="6b93d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-156">Int32</span></span>|<span data-ttu-id="6b93d-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="6b93d-157">Device error count for the setting</span></span>|
|<span data-ttu-id="6b93d-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6b93d-158">conflictDeviceCount</span></span>|<span data-ttu-id="6b93d-159">Int32</span><span class="sxs-lookup"><span data-stu-id="6b93d-159">Int32</span></span>|<span data-ttu-id="6b93d-160">Количество конфликтов устройств для параметра</span><span class="sxs-lookup"><span data-stu-id="6b93d-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b93d-161">Связи</span><span class="sxs-lookup"><span data-stu-id="6b93d-161">Relationships</span></span>
<span data-ttu-id="6b93d-162">Нет</span><span class="sxs-lookup"><span data-stu-id="6b93d-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b93d-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b93d-163">JSON Representation</span></span>
<span data-ttu-id="6b93d-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b93d-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```





