---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: tfitzmac
ms.openlocfilehash: 27e3595156699cd345215959a78a7642399c43bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359278"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="e68fd-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-104">detectedApp resource type</span></span>

> <span data-ttu-id="e68fd-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e68fd-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e68fd-106">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="e68fd-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="e68fd-107">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="e68fd-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="e68fd-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e68fd-108">Methods</span></span>
|<span data-ttu-id="e68fd-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e68fd-109">Method</span></span>|<span data-ttu-id="e68fd-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e68fd-110">Return Type</span></span>|<span data-ttu-id="e68fd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e68fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e68fd-112">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="e68fd-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="e68fd-113">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e68fd-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="e68fd-114">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e68fd-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="e68fd-115">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="e68fd-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="e68fd-117">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e68fd-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="e68fd-118">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="e68fd-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="e68fd-120">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e68fd-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="e68fd-121">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="e68fd-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e68fd-122">None</span></span>|<span data-ttu-id="e68fd-123">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e68fd-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="e68fd-124">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="e68fd-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e68fd-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="e68fd-126">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e68fd-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e68fd-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e68fd-127">Properties</span></span>
|<span data-ttu-id="e68fd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e68fd-128">Property</span></span>|<span data-ttu-id="e68fd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e68fd-129">Type</span></span>|<span data-ttu-id="e68fd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e68fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68fd-131">id</span><span class="sxs-lookup"><span data-stu-id="e68fd-131">id</span></span>|<span data-ttu-id="e68fd-132">String</span><span class="sxs-lookup"><span data-stu-id="e68fd-132">String</span></span>|<span data-ttu-id="e68fd-133">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="e68fd-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="e68fd-134">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="e68fd-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="e68fd-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e68fd-135">Read-only.</span></span>|
|<span data-ttu-id="e68fd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e68fd-136">displayName</span></span>|<span data-ttu-id="e68fd-137">String</span><span class="sxs-lookup"><span data-stu-id="e68fd-137">String</span></span>|<span data-ttu-id="e68fd-138">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="e68fd-138">Name of the discovered application.</span></span> <span data-ttu-id="e68fd-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e68fd-139">Read-only</span></span>|
|<span data-ttu-id="e68fd-140">version</span><span class="sxs-lookup"><span data-stu-id="e68fd-140">version</span></span>|<span data-ttu-id="e68fd-141">String</span><span class="sxs-lookup"><span data-stu-id="e68fd-141">String</span></span>|<span data-ttu-id="e68fd-142">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="e68fd-142">Version of the discovered application.</span></span> <span data-ttu-id="e68fd-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e68fd-143">Read-only</span></span>|
|<span data-ttu-id="e68fd-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="e68fd-144">sizeInByte</span></span>|<span data-ttu-id="e68fd-145">Int64</span><span class="sxs-lookup"><span data-stu-id="e68fd-145">Int64</span></span>|<span data-ttu-id="e68fd-146">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e68fd-146">Discovered application size in bytes.</span></span> <span data-ttu-id="e68fd-147">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e68fd-147">Read-only</span></span>|
|<span data-ttu-id="e68fd-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e68fd-148">deviceCount</span></span>|<span data-ttu-id="e68fd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e68fd-149">Int32</span></span>|<span data-ttu-id="e68fd-150">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="e68fd-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e68fd-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e68fd-151">Relationships</span></span>
|<span data-ttu-id="e68fd-152">Связь</span><span class="sxs-lookup"><span data-stu-id="e68fd-152">Relationship</span></span>|<span data-ttu-id="e68fd-153">Тип</span><span class="sxs-lookup"><span data-stu-id="e68fd-153">Type</span></span>|<span data-ttu-id="e68fd-154">Описание</span><span class="sxs-lookup"><span data-stu-id="e68fd-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e68fd-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="e68fd-155">managedDevices</span></span>|<span data-ttu-id="e68fd-156">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="e68fd-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="e68fd-157">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="e68fd-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e68fd-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e68fd-158">JSON Representation</span></span>
<span data-ttu-id="e68fd-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e68fd-159">Here is a JSON representation of the resource.</span></span>
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



