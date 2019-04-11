---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01233111e74da95f84d0cbeb81e4675a5c6e049d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773198"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="d49e5-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-104">detectedApp resource type</span></span>

> <span data-ttu-id="d49e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d49e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d49e5-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d49e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d49e5-107">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d49e5-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="d49e5-108">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="d49e5-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="d49e5-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d49e5-109">Methods</span></span>
|<span data-ttu-id="d49e5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d49e5-110">Method</span></span>|<span data-ttu-id="d49e5-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d49e5-111">Return Type</span></span>|<span data-ttu-id="d49e5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d49e5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d49e5-113">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="d49e5-114">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d49e5-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="d49e5-115">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d49e5-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="d49e5-116">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="d49e5-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d49e5-118">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d49e5-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d49e5-119">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="d49e5-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d49e5-121">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d49e5-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="d49e5-122">Delete detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="d49e5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d49e5-123">None</span></span>|<span data-ttu-id="d49e5-124">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d49e5-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="d49e5-125">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="d49e5-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="d49e5-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="d49e5-127">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d49e5-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d49e5-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="d49e5-128">Properties</span></span>
|<span data-ttu-id="d49e5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d49e5-129">Property</span></span>|<span data-ttu-id="d49e5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d49e5-130">Type</span></span>|<span data-ttu-id="d49e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d49e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d49e5-132">id</span><span class="sxs-lookup"><span data-stu-id="d49e5-132">id</span></span>|<span data-ttu-id="d49e5-133">String</span><span class="sxs-lookup"><span data-stu-id="d49e5-133">String</span></span>|<span data-ttu-id="d49e5-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d49e5-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="d49e5-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="d49e5-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="d49e5-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d49e5-136">Read-only.</span></span>|
|<span data-ttu-id="d49e5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d49e5-137">displayName</span></span>|<span data-ttu-id="d49e5-138">String</span><span class="sxs-lookup"><span data-stu-id="d49e5-138">String</span></span>|<span data-ttu-id="d49e5-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d49e5-139">Name of the discovered application.</span></span> <span data-ttu-id="d49e5-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d49e5-140">Read-only</span></span>|
|<span data-ttu-id="d49e5-141">version</span><span class="sxs-lookup"><span data-stu-id="d49e5-141">version</span></span>|<span data-ttu-id="d49e5-142">String</span><span class="sxs-lookup"><span data-stu-id="d49e5-142">String</span></span>|<span data-ttu-id="d49e5-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="d49e5-143">Version of the discovered application.</span></span> <span data-ttu-id="d49e5-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d49e5-144">Read-only</span></span>|
|<span data-ttu-id="d49e5-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="d49e5-145">sizeInByte</span></span>|<span data-ttu-id="d49e5-146">Int64</span><span class="sxs-lookup"><span data-stu-id="d49e5-146">Int64</span></span>|<span data-ttu-id="d49e5-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="d49e5-147">Discovered application size in bytes.</span></span> <span data-ttu-id="d49e5-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d49e5-148">Read-only</span></span>|
|<span data-ttu-id="d49e5-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d49e5-149">deviceCount</span></span>|<span data-ttu-id="d49e5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d49e5-150">Int32</span></span>|<span data-ttu-id="d49e5-151">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="d49e5-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d49e5-152">Связи</span><span class="sxs-lookup"><span data-stu-id="d49e5-152">Relationships</span></span>
|<span data-ttu-id="d49e5-153">Отношение</span><span class="sxs-lookup"><span data-stu-id="d49e5-153">Relationship</span></span>|<span data-ttu-id="d49e5-154">Тип</span><span class="sxs-lookup"><span data-stu-id="d49e5-154">Type</span></span>|<span data-ttu-id="d49e5-155">Описание</span><span class="sxs-lookup"><span data-stu-id="d49e5-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d49e5-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="d49e5-156">managedDevices</span></span>|<span data-ttu-id="d49e5-157">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d49e5-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="d49e5-158">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="d49e5-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d49e5-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d49e5-159">JSON Representation</span></span>
<span data-ttu-id="d49e5-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d49e5-160">Here is a JSON representation of the resource.</span></span>
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





