---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2985f55e76081674b94b0b3adb6e7080eb317026
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464061"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="d1db9-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-104">detectedApp resource type</span></span>

<span data-ttu-id="d1db9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1db9-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1db9-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1db9-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1db9-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1db9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1db9-108">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d1db9-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="d1db9-109">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="d1db9-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="d1db9-110">Методы</span><span class="sxs-lookup"><span data-stu-id="d1db9-110">Methods</span></span>
|<span data-ttu-id="d1db9-111">Метод</span><span class="sxs-lookup"><span data-stu-id="d1db9-111">Method</span></span>|<span data-ttu-id="d1db9-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d1db9-112">Return Type</span></span>|<span data-ttu-id="d1db9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d1db9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1db9-114">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="d1db9-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="d1db9-115">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d1db9-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="d1db9-116">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="d1db9-117">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|<span data-ttu-id="d1db9-118">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="d1db9-118">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="d1db9-119">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d1db9-120">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|<span data-ttu-id="d1db9-121">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="d1db9-121">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="d1db9-122">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d1db9-123">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="d1db9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d1db9-124">None</span></span>|<span data-ttu-id="d1db9-125">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="d1db9-126">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="d1db9-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d1db9-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d1db9-128">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d1db9-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1db9-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1db9-129">Properties</span></span>
|<span data-ttu-id="d1db9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1db9-130">Property</span></span>|<span data-ttu-id="d1db9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d1db9-131">Type</span></span>|<span data-ttu-id="d1db9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d1db9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1db9-133">id</span><span class="sxs-lookup"><span data-stu-id="d1db9-133">id</span></span>|<span data-ttu-id="d1db9-134">String</span><span class="sxs-lookup"><span data-stu-id="d1db9-134">String</span></span>|<span data-ttu-id="d1db9-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d1db9-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="d1db9-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="d1db9-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="d1db9-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1db9-137">Read-only.</span></span>|
|<span data-ttu-id="d1db9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d1db9-138">displayName</span></span>|<span data-ttu-id="d1db9-139">Строка</span><span class="sxs-lookup"><span data-stu-id="d1db9-139">String</span></span>|<span data-ttu-id="d1db9-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d1db9-140">Name of the discovered application.</span></span> <span data-ttu-id="d1db9-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d1db9-141">Read-only</span></span>|
|<span data-ttu-id="d1db9-142">version</span><span class="sxs-lookup"><span data-stu-id="d1db9-142">version</span></span>|<span data-ttu-id="d1db9-143">String</span><span class="sxs-lookup"><span data-stu-id="d1db9-143">String</span></span>|<span data-ttu-id="d1db9-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d1db9-144">Version of the discovered application.</span></span> <span data-ttu-id="d1db9-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d1db9-145">Read-only</span></span>|
|<span data-ttu-id="d1db9-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="d1db9-146">sizeInByte</span></span>|<span data-ttu-id="d1db9-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d1db9-147">Int64</span></span>|<span data-ttu-id="d1db9-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="d1db9-148">Discovered application size in bytes.</span></span> <span data-ttu-id="d1db9-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d1db9-149">Read-only</span></span>|
|<span data-ttu-id="d1db9-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d1db9-150">deviceCount</span></span>|<span data-ttu-id="d1db9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d1db9-151">Int32</span></span>|<span data-ttu-id="d1db9-152">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="d1db9-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1db9-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="d1db9-153">Relationships</span></span>
|<span data-ttu-id="d1db9-154">Связь</span><span class="sxs-lookup"><span data-stu-id="d1db9-154">Relationship</span></span>|<span data-ttu-id="d1db9-155">Тип</span><span class="sxs-lookup"><span data-stu-id="d1db9-155">Type</span></span>|<span data-ttu-id="d1db9-156">Описание</span><span class="sxs-lookup"><span data-stu-id="d1db9-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1db9-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d1db9-157">managedDevices</span></span>|<span data-ttu-id="d1db9-158">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d1db9-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="d1db9-159">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="d1db9-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1db9-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1db9-160">JSON Representation</span></span>
<span data-ttu-id="d1db9-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1db9-161">Here is a JSON representation of the resource.</span></span>
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



