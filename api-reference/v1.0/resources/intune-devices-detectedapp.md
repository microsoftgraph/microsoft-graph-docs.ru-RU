---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd0d683ebcada0bbc7ef2b1baa9269e912faf03c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030872"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="8ab90-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-104">detectedApp resource type</span></span>

> <span data-ttu-id="8ab90-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ab90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab90-106">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="8ab90-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="8ab90-107">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="8ab90-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="8ab90-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8ab90-108">Methods</span></span>
|<span data-ttu-id="8ab90-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8ab90-109">Method</span></span>|<span data-ttu-id="8ab90-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8ab90-110">Return Type</span></span>|<span data-ttu-id="8ab90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab90-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ab90-112">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="8ab90-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="8ab90-113">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8ab90-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="8ab90-114">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ab90-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="8ab90-115">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|<span data-ttu-id="8ab90-116">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="8ab90-116">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="8ab90-117">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ab90-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8ab90-118">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|<span data-ttu-id="8ab90-119">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="8ab90-119">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="8ab90-120">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ab90-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="8ab90-121">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="8ab90-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8ab90-122">None</span></span>|<span data-ttu-id="8ab90-123">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ab90-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="8ab90-124">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="8ab90-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="8ab90-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="8ab90-126">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8ab90-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ab90-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ab90-127">Properties</span></span>
|<span data-ttu-id="8ab90-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ab90-128">Property</span></span>|<span data-ttu-id="8ab90-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8ab90-129">Type</span></span>|<span data-ttu-id="8ab90-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab90-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab90-131">id</span><span class="sxs-lookup"><span data-stu-id="8ab90-131">id</span></span>|<span data-ttu-id="8ab90-132">String</span><span class="sxs-lookup"><span data-stu-id="8ab90-132">String</span></span>|<span data-ttu-id="8ab90-133">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="8ab90-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="8ab90-134">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="8ab90-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="8ab90-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ab90-135">Read-only.</span></span>|
|<span data-ttu-id="8ab90-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8ab90-136">displayName</span></span>|<span data-ttu-id="8ab90-137">Строка</span><span class="sxs-lookup"><span data-stu-id="8ab90-137">String</span></span>|<span data-ttu-id="8ab90-138">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="8ab90-138">Name of the discovered application.</span></span> <span data-ttu-id="8ab90-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="8ab90-139">Read-only</span></span>|
|<span data-ttu-id="8ab90-140">version</span><span class="sxs-lookup"><span data-stu-id="8ab90-140">version</span></span>|<span data-ttu-id="8ab90-141">String</span><span class="sxs-lookup"><span data-stu-id="8ab90-141">String</span></span>|<span data-ttu-id="8ab90-142">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="8ab90-142">Version of the discovered application.</span></span> <span data-ttu-id="8ab90-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="8ab90-143">Read-only</span></span>|
|<span data-ttu-id="8ab90-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="8ab90-144">sizeInByte</span></span>|<span data-ttu-id="8ab90-145">Int64</span><span class="sxs-lookup"><span data-stu-id="8ab90-145">Int64</span></span>|<span data-ttu-id="8ab90-146">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="8ab90-146">Discovered application size in bytes.</span></span> <span data-ttu-id="8ab90-147">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="8ab90-147">Read-only</span></span>|
|<span data-ttu-id="8ab90-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8ab90-148">deviceCount</span></span>|<span data-ttu-id="8ab90-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8ab90-149">Int32</span></span>|<span data-ttu-id="8ab90-150">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="8ab90-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab90-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="8ab90-151">Relationships</span></span>
|<span data-ttu-id="8ab90-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="8ab90-152">Relationship</span></span>|<span data-ttu-id="8ab90-153">Тип</span><span class="sxs-lookup"><span data-stu-id="8ab90-153">Type</span></span>|<span data-ttu-id="8ab90-154">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab90-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab90-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="8ab90-155">managedDevices</span></span>|<span data-ttu-id="8ab90-156">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="8ab90-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="8ab90-157">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="8ab90-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ab90-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ab90-158">JSON Representation</span></span>
<span data-ttu-id="8ab90-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ab90-159">Here is a JSON representation of the resource.</span></span>
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



