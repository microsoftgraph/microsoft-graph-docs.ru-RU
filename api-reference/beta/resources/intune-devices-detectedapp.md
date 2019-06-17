---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 098ad481c854514e988037e755cefd3dbecd8165
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983157"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="11729-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-104">detectedApp resource type</span></span>

> <span data-ttu-id="11729-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11729-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11729-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11729-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11729-107">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="11729-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="11729-108">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="11729-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="11729-109">Методы</span><span class="sxs-lookup"><span data-stu-id="11729-109">Methods</span></span>
|<span data-ttu-id="11729-110">Метод</span><span class="sxs-lookup"><span data-stu-id="11729-110">Method</span></span>|<span data-ttu-id="11729-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11729-111">Return Type</span></span>|<span data-ttu-id="11729-112">Описание</span><span class="sxs-lookup"><span data-stu-id="11729-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11729-113">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="11729-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="11729-114">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="11729-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="11729-115">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="11729-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="11729-116">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|<span data-ttu-id="11729-117">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="11729-117">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="11729-118">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="11729-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="11729-119">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|<span data-ttu-id="11729-120">[detectedApp](../resources/intune-devices-detectedapp.md);</span><span class="sxs-lookup"><span data-stu-id="11729-120">[detectedApp](../resources/intune-devices-detectedapp.md)</span></span>|<span data-ttu-id="11729-121">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="11729-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="11729-122">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="11729-123">Нет</span><span class="sxs-lookup"><span data-stu-id="11729-123">None</span></span>|<span data-ttu-id="11729-124">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="11729-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="11729-125">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="11729-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="11729-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="11729-127">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="11729-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11729-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="11729-128">Properties</span></span>
|<span data-ttu-id="11729-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="11729-129">Property</span></span>|<span data-ttu-id="11729-130">Тип</span><span class="sxs-lookup"><span data-stu-id="11729-130">Type</span></span>|<span data-ttu-id="11729-131">Описание</span><span class="sxs-lookup"><span data-stu-id="11729-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11729-132">id</span><span class="sxs-lookup"><span data-stu-id="11729-132">id</span></span>|<span data-ttu-id="11729-133">String</span><span class="sxs-lookup"><span data-stu-id="11729-133">String</span></span>|<span data-ttu-id="11729-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="11729-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="11729-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="11729-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="11729-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11729-136">Read-only.</span></span>|
|<span data-ttu-id="11729-137">displayName</span><span class="sxs-lookup"><span data-stu-id="11729-137">displayName</span></span>|<span data-ttu-id="11729-138">Строка</span><span class="sxs-lookup"><span data-stu-id="11729-138">String</span></span>|<span data-ttu-id="11729-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="11729-139">Name of the discovered application.</span></span> <span data-ttu-id="11729-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="11729-140">Read-only</span></span>|
|<span data-ttu-id="11729-141">version</span><span class="sxs-lookup"><span data-stu-id="11729-141">version</span></span>|<span data-ttu-id="11729-142">String</span><span class="sxs-lookup"><span data-stu-id="11729-142">String</span></span>|<span data-ttu-id="11729-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="11729-143">Version of the discovered application.</span></span> <span data-ttu-id="11729-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="11729-144">Read-only</span></span>|
|<span data-ttu-id="11729-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="11729-145">sizeInByte</span></span>|<span data-ttu-id="11729-146">Int64</span><span class="sxs-lookup"><span data-stu-id="11729-146">Int64</span></span>|<span data-ttu-id="11729-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="11729-147">Discovered application size in bytes.</span></span> <span data-ttu-id="11729-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="11729-148">Read-only</span></span>|
|<span data-ttu-id="11729-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="11729-149">deviceCount</span></span>|<span data-ttu-id="11729-150">Int32</span><span class="sxs-lookup"><span data-stu-id="11729-150">Int32</span></span>|<span data-ttu-id="11729-151">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="11729-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="11729-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="11729-152">Relationships</span></span>
|<span data-ttu-id="11729-153">Отношение</span><span class="sxs-lookup"><span data-stu-id="11729-153">Relationship</span></span>|<span data-ttu-id="11729-154">Тип</span><span class="sxs-lookup"><span data-stu-id="11729-154">Type</span></span>|<span data-ttu-id="11729-155">Описание</span><span class="sxs-lookup"><span data-stu-id="11729-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11729-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="11729-156">managedDevices</span></span>|<span data-ttu-id="11729-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="11729-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="11729-158">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="11729-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11729-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11729-159">JSON Representation</span></span>
<span data-ttu-id="11729-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11729-160">Here is a JSON representation of the resource.</span></span>
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





