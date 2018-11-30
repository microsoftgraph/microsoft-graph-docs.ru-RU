---
title: Тип ресурса settingStateDeviceSummary
description: Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств
ms.openlocfilehash: 9f2cca6be1773a7698dcc56fab00f9979e4ee071
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076182"
---
# <a name="settingstatedevicesummary-resource-type"></a><span data-ttu-id="17f64-103">Тип ресурса settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-103">settingStateDeviceSummary resource type</span></span>

> <span data-ttu-id="17f64-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17f64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17f64-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17f64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17f64-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17f64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17f64-107">Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств</span><span class="sxs-lookup"><span data-stu-id="17f64-107">Device Compilance Policy and Configuration for a Setting State summary</span></span>
## <a name="methods"></a><span data-ttu-id="17f64-108">Методы</span><span class="sxs-lookup"><span data-stu-id="17f64-108">Methods</span></span>
|<span data-ttu-id="17f64-109">Метод</span><span class="sxs-lookup"><span data-stu-id="17f64-109">Method</span></span>|<span data-ttu-id="17f64-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17f64-110">Return Type</span></span>|<span data-ttu-id="17f64-111">Описание</span><span class="sxs-lookup"><span data-stu-id="17f64-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17f64-112">Список объектов settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-112">List settingStateDeviceSummaries</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|<span data-ttu-id="17f64-113">Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="17f64-113">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="17f64-114">Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17f64-114">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>|
|[<span data-ttu-id="17f64-115">Получение объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-115">Get settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[<span data-ttu-id="17f64-116">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-116">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="17f64-117">Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17f64-117">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="17f64-118">Создание объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-118">Create settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[<span data-ttu-id="17f64-119">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-119">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="17f64-120">Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17f64-120">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|
|[<span data-ttu-id="17f64-121">Удаление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-121">Delete settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|<span data-ttu-id="17f64-122">Нет</span><span class="sxs-lookup"><span data-stu-id="17f64-122">None</span></span>|<span data-ttu-id="17f64-123">Удаляет объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17f64-123">Deletes a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span></span>|
|[<span data-ttu-id="17f64-124">Обновление объекта settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-124">Update settingStateDeviceSummary</span></span>](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[<span data-ttu-id="17f64-125">settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="17f64-125">settingStateDeviceSummary</span></span>](../resources/intune-deviceconfig-settingstatedevicesummary.md)|<span data-ttu-id="17f64-126">Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).</span><span class="sxs-lookup"><span data-stu-id="17f64-126">Update the properties of a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17f64-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="17f64-127">Properties</span></span>
|<span data-ttu-id="17f64-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="17f64-128">Property</span></span>|<span data-ttu-id="17f64-129">Тип</span><span class="sxs-lookup"><span data-stu-id="17f64-129">Type</span></span>|<span data-ttu-id="17f64-130">Описание</span><span class="sxs-lookup"><span data-stu-id="17f64-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f64-131">id</span><span class="sxs-lookup"><span data-stu-id="17f64-131">id</span></span>|<span data-ttu-id="17f64-132">String</span><span class="sxs-lookup"><span data-stu-id="17f64-132">String</span></span>|<span data-ttu-id="17f64-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="17f64-133">Key of the entity.</span></span>|
|<span data-ttu-id="17f64-134">settingName</span><span class="sxs-lookup"><span data-stu-id="17f64-134">settingName</span></span>|<span data-ttu-id="17f64-135">String</span><span class="sxs-lookup"><span data-stu-id="17f64-135">String</span></span>|<span data-ttu-id="17f64-136">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-136">Name of the setting</span></span>|
|<span data-ttu-id="17f64-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="17f64-137">instancePath</span></span>|<span data-ttu-id="17f64-138">String</span><span class="sxs-lookup"><span data-stu-id="17f64-138">String</span></span>|<span data-ttu-id="17f64-139">Имя пути к экземпляру для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="17f64-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-140">unknownDeviceCount</span></span>|<span data-ttu-id="17f64-141">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-141">Int32</span></span>|<span data-ttu-id="17f64-142">Количество неизвестных устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="17f64-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="17f64-144">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-144">Int32</span></span>|<span data-ttu-id="17f64-145">Количество неприменимых устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="17f64-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-146">compliantDeviceCount</span></span>|<span data-ttu-id="17f64-147">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-147">Int32</span></span>|<span data-ttu-id="17f64-148">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="17f64-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-149">remediatedDeviceCount</span></span>|<span data-ttu-id="17f64-150">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-150">Int32</span></span>|<span data-ttu-id="17f64-151">Количество соответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="17f64-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="17f64-153">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-153">Int32</span></span>|<span data-ttu-id="17f64-154">Количество несоответствующих устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="17f64-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-155">errorDeviceCount</span></span>|<span data-ttu-id="17f64-156">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-156">Int32</span></span>|<span data-ttu-id="17f64-157">Количество ошибок устройств для параметра.</span><span class="sxs-lookup"><span data-stu-id="17f64-157">Device error count for the setting</span></span>|
|<span data-ttu-id="17f64-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="17f64-158">conflictDeviceCount</span></span>|<span data-ttu-id="17f64-159">Int32</span><span class="sxs-lookup"><span data-stu-id="17f64-159">Int32</span></span>|<span data-ttu-id="17f64-160">Количество конфликтов устройств для параметра</span><span class="sxs-lookup"><span data-stu-id="17f64-160">Device conflict error count for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="17f64-161">Связи</span><span class="sxs-lookup"><span data-stu-id="17f64-161">Relationships</span></span>
<span data-ttu-id="17f64-162">Нет</span><span class="sxs-lookup"><span data-stu-id="17f64-162">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17f64-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17f64-163">JSON Representation</span></span>
<span data-ttu-id="17f64-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17f64-164">Here is a JSON representation of the resource.</span></span>
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





