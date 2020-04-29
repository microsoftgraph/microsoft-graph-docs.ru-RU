---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dae22c8a2e939d7ab06a645726f139d5b02ac724
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407052"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="dcafc-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-104">detectedApp resource type</span></span>

<span data-ttu-id="dcafc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcafc-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcafc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dcafc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcafc-107">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="dcafc-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="dcafc-108">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="dcafc-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="dcafc-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dcafc-109">Methods</span></span>
|<span data-ttu-id="dcafc-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dcafc-110">Method</span></span>|<span data-ttu-id="dcafc-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dcafc-111">Return Type</span></span>|<span data-ttu-id="dcafc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dcafc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dcafc-113">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="dcafc-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="dcafc-114">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="dcafc-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="dcafc-115">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcafc-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="dcafc-116">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|<span data-ttu-id="dcafc-117">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="dcafc-117">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="dcafc-118">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcafc-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="dcafc-119">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|<span data-ttu-id="dcafc-120">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="dcafc-120">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="dcafc-121">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcafc-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="dcafc-122">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="dcafc-123">Нет</span><span class="sxs-lookup"><span data-stu-id="dcafc-123">None</span></span>|<span data-ttu-id="dcafc-124">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcafc-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="dcafc-125">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="dcafc-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="dcafc-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="dcafc-127">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="dcafc-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dcafc-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcafc-128">Properties</span></span>
|<span data-ttu-id="dcafc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcafc-129">Property</span></span>|<span data-ttu-id="dcafc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dcafc-130">Type</span></span>|<span data-ttu-id="dcafc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dcafc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcafc-132">id</span><span class="sxs-lookup"><span data-stu-id="dcafc-132">id</span></span>|<span data-ttu-id="dcafc-133">String</span><span class="sxs-lookup"><span data-stu-id="dcafc-133">String</span></span>|<span data-ttu-id="dcafc-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="dcafc-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="dcafc-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="dcafc-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="dcafc-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcafc-136">Read-only.</span></span>|
|<span data-ttu-id="dcafc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dcafc-137">displayName</span></span>|<span data-ttu-id="dcafc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="dcafc-138">String</span></span>|<span data-ttu-id="dcafc-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="dcafc-139">Name of the discovered application.</span></span> <span data-ttu-id="dcafc-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="dcafc-140">Read-only</span></span>|
|<span data-ttu-id="dcafc-141">version</span><span class="sxs-lookup"><span data-stu-id="dcafc-141">version</span></span>|<span data-ttu-id="dcafc-142">String</span><span class="sxs-lookup"><span data-stu-id="dcafc-142">String</span></span>|<span data-ttu-id="dcafc-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="dcafc-143">Version of the discovered application.</span></span> <span data-ttu-id="dcafc-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="dcafc-144">Read-only</span></span>|
|<span data-ttu-id="dcafc-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="dcafc-145">sizeInByte</span></span>|<span data-ttu-id="dcafc-146">Int64</span><span class="sxs-lookup"><span data-stu-id="dcafc-146">Int64</span></span>|<span data-ttu-id="dcafc-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="dcafc-147">Discovered application size in bytes.</span></span> <span data-ttu-id="dcafc-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="dcafc-148">Read-only</span></span>|
|<span data-ttu-id="dcafc-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="dcafc-149">deviceCount</span></span>|<span data-ttu-id="dcafc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="dcafc-150">Int32</span></span>|<span data-ttu-id="dcafc-151">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="dcafc-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcafc-152">Связи</span><span class="sxs-lookup"><span data-stu-id="dcafc-152">Relationships</span></span>
|<span data-ttu-id="dcafc-153">Связь</span><span class="sxs-lookup"><span data-stu-id="dcafc-153">Relationship</span></span>|<span data-ttu-id="dcafc-154">Тип</span><span class="sxs-lookup"><span data-stu-id="dcafc-154">Type</span></span>|<span data-ttu-id="dcafc-155">Описание</span><span class="sxs-lookup"><span data-stu-id="dcafc-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcafc-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="dcafc-156">managedDevices</span></span>|<span data-ttu-id="dcafc-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="dcafc-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="dcafc-158">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="dcafc-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dcafc-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcafc-159">JSON Representation</span></span>
<span data-ttu-id="dcafc-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcafc-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```







