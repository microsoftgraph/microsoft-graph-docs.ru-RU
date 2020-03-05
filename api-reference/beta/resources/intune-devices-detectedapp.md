---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 25d0c77fd9cd0621837b0e6f879136dced6cf208
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525119"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="28d1d-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-104">detectedApp resource type</span></span>

<span data-ttu-id="28d1d-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="28d1d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28d1d-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d1d-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28d1d-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28d1d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28d1d-108">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="28d1d-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="28d1d-109">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="28d1d-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="28d1d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="28d1d-110">Methods</span></span>
|<span data-ttu-id="28d1d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="28d1d-111">Method</span></span>|<span data-ttu-id="28d1d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="28d1d-112">Return Type</span></span>|<span data-ttu-id="28d1d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="28d1d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28d1d-114">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="28d1d-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="28d1d-115">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="28d1d-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="28d1d-116">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28d1d-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="28d1d-117">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|<span data-ttu-id="28d1d-118">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="28d1d-118">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="28d1d-119">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28d1d-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="28d1d-120">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|<span data-ttu-id="28d1d-121">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="28d1d-121">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="28d1d-122">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28d1d-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="28d1d-123">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="28d1d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="28d1d-124">None</span></span>|<span data-ttu-id="28d1d-125">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28d1d-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="28d1d-126">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="28d1d-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="28d1d-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="28d1d-128">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="28d1d-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28d1d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="28d1d-129">Properties</span></span>
|<span data-ttu-id="28d1d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28d1d-130">Property</span></span>|<span data-ttu-id="28d1d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28d1d-131">Type</span></span>|<span data-ttu-id="28d1d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28d1d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28d1d-133">id</span><span class="sxs-lookup"><span data-stu-id="28d1d-133">id</span></span>|<span data-ttu-id="28d1d-134">String</span><span class="sxs-lookup"><span data-stu-id="28d1d-134">String</span></span>|<span data-ttu-id="28d1d-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="28d1d-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="28d1d-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="28d1d-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="28d1d-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28d1d-137">Read-only.</span></span>|
|<span data-ttu-id="28d1d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="28d1d-138">displayName</span></span>|<span data-ttu-id="28d1d-139">Строка</span><span class="sxs-lookup"><span data-stu-id="28d1d-139">String</span></span>|<span data-ttu-id="28d1d-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="28d1d-140">Name of the discovered application.</span></span> <span data-ttu-id="28d1d-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="28d1d-141">Read-only</span></span>|
|<span data-ttu-id="28d1d-142">version</span><span class="sxs-lookup"><span data-stu-id="28d1d-142">version</span></span>|<span data-ttu-id="28d1d-143">String</span><span class="sxs-lookup"><span data-stu-id="28d1d-143">String</span></span>|<span data-ttu-id="28d1d-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="28d1d-144">Version of the discovered application.</span></span> <span data-ttu-id="28d1d-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="28d1d-145">Read-only</span></span>|
|<span data-ttu-id="28d1d-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="28d1d-146">sizeInByte</span></span>|<span data-ttu-id="28d1d-147">Int64</span><span class="sxs-lookup"><span data-stu-id="28d1d-147">Int64</span></span>|<span data-ttu-id="28d1d-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="28d1d-148">Discovered application size in bytes.</span></span> <span data-ttu-id="28d1d-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="28d1d-149">Read-only</span></span>|
|<span data-ttu-id="28d1d-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="28d1d-150">deviceCount</span></span>|<span data-ttu-id="28d1d-151">Int32</span><span class="sxs-lookup"><span data-stu-id="28d1d-151">Int32</span></span>|<span data-ttu-id="28d1d-152">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="28d1d-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="28d1d-153">Связи</span><span class="sxs-lookup"><span data-stu-id="28d1d-153">Relationships</span></span>
|<span data-ttu-id="28d1d-154">Связь</span><span class="sxs-lookup"><span data-stu-id="28d1d-154">Relationship</span></span>|<span data-ttu-id="28d1d-155">Тип</span><span class="sxs-lookup"><span data-stu-id="28d1d-155">Type</span></span>|<span data-ttu-id="28d1d-156">Описание</span><span class="sxs-lookup"><span data-stu-id="28d1d-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28d1d-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="28d1d-157">managedDevices</span></span>|<span data-ttu-id="28d1d-158">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="28d1d-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="28d1d-159">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="28d1d-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28d1d-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28d1d-160">JSON Representation</span></span>
<span data-ttu-id="28d1d-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28d1d-161">Here is a JSON representation of the resource.</span></span>
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



