---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4cba801689cb5051926a3139574d5a27294090a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403100"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="c03cd-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-104">detectedApp resource type</span></span>

> <span data-ttu-id="c03cd-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c03cd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c03cd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c03cd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c03cd-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c03cd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c03cd-108">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="c03cd-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="c03cd-109">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="c03cd-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="c03cd-110">Методы</span><span class="sxs-lookup"><span data-stu-id="c03cd-110">Methods</span></span>
|<span data-ttu-id="c03cd-111">Метод</span><span class="sxs-lookup"><span data-stu-id="c03cd-111">Method</span></span>|<span data-ttu-id="c03cd-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c03cd-112">Return Type</span></span>|<span data-ttu-id="c03cd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c03cd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c03cd-114">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="c03cd-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="c03cd-115">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c03cd-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="c03cd-116">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c03cd-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="c03cd-117">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="c03cd-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="c03cd-119">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c03cd-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="c03cd-120">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="c03cd-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="c03cd-122">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c03cd-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="c03cd-123">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="c03cd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c03cd-124">None</span></span>|<span data-ttu-id="c03cd-125">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c03cd-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="c03cd-126">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="c03cd-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="c03cd-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="c03cd-128">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c03cd-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c03cd-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="c03cd-129">Properties</span></span>
|<span data-ttu-id="c03cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c03cd-130">Property</span></span>|<span data-ttu-id="c03cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c03cd-131">Type</span></span>|<span data-ttu-id="c03cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c03cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c03cd-133">id</span><span class="sxs-lookup"><span data-stu-id="c03cd-133">id</span></span>|<span data-ttu-id="c03cd-134">String</span><span class="sxs-lookup"><span data-stu-id="c03cd-134">String</span></span>|<span data-ttu-id="c03cd-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="c03cd-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="c03cd-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="c03cd-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="c03cd-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c03cd-137">Read-only.</span></span>|
|<span data-ttu-id="c03cd-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c03cd-138">displayName</span></span>|<span data-ttu-id="c03cd-139">String</span><span class="sxs-lookup"><span data-stu-id="c03cd-139">String</span></span>|<span data-ttu-id="c03cd-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="c03cd-140">Name of the discovered application.</span></span> <span data-ttu-id="c03cd-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c03cd-141">Read-only</span></span>|
|<span data-ttu-id="c03cd-142">version</span><span class="sxs-lookup"><span data-stu-id="c03cd-142">version</span></span>|<span data-ttu-id="c03cd-143">String</span><span class="sxs-lookup"><span data-stu-id="c03cd-143">String</span></span>|<span data-ttu-id="c03cd-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="c03cd-144">Version of the discovered application.</span></span> <span data-ttu-id="c03cd-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c03cd-145">Read-only</span></span>|
|<span data-ttu-id="c03cd-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="c03cd-146">sizeInByte</span></span>|<span data-ttu-id="c03cd-147">Int64</span><span class="sxs-lookup"><span data-stu-id="c03cd-147">Int64</span></span>|<span data-ttu-id="c03cd-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="c03cd-148">Discovered application size in bytes.</span></span> <span data-ttu-id="c03cd-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c03cd-149">Read-only</span></span>|
|<span data-ttu-id="c03cd-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c03cd-150">deviceCount</span></span>|<span data-ttu-id="c03cd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c03cd-151">Int32</span></span>|<span data-ttu-id="c03cd-152">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="c03cd-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="c03cd-153">Связи</span><span class="sxs-lookup"><span data-stu-id="c03cd-153">Relationships</span></span>
|<span data-ttu-id="c03cd-154">Связь</span><span class="sxs-lookup"><span data-stu-id="c03cd-154">Relationship</span></span>|<span data-ttu-id="c03cd-155">Тип</span><span class="sxs-lookup"><span data-stu-id="c03cd-155">Type</span></span>|<span data-ttu-id="c03cd-156">Описание</span><span class="sxs-lookup"><span data-stu-id="c03cd-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c03cd-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="c03cd-157">managedDevices</span></span>|<span data-ttu-id="c03cd-158">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="c03cd-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="c03cd-159">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="c03cd-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c03cd-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c03cd-160">JSON Representation</span></span>
<span data-ttu-id="c03cd-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c03cd-161">Here is a JSON representation of the resource.</span></span>
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




