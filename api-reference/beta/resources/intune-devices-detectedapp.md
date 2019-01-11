---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f62e41b51d2b22d9524a0e86775e5f1cf9526618
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890078"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="173fc-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-104">detectedApp resource type</span></span>

> <span data-ttu-id="173fc-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="173fc-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="173fc-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="173fc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="173fc-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="173fc-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="173fc-108">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="173fc-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="173fc-109">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="173fc-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="173fc-110">Методы</span><span class="sxs-lookup"><span data-stu-id="173fc-110">Methods</span></span>
|<span data-ttu-id="173fc-111">Метод</span><span class="sxs-lookup"><span data-stu-id="173fc-111">Method</span></span>|<span data-ttu-id="173fc-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="173fc-112">Return Type</span></span>|<span data-ttu-id="173fc-113">Описание</span><span class="sxs-lookup"><span data-stu-id="173fc-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="173fc-114">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="173fc-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="173fc-115">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="173fc-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="173fc-116">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="173fc-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="173fc-117">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="173fc-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="173fc-119">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="173fc-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="173fc-120">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="173fc-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="173fc-122">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="173fc-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="173fc-123">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="173fc-124">Нет</span><span class="sxs-lookup"><span data-stu-id="173fc-124">None</span></span>|<span data-ttu-id="173fc-125">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="173fc-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="173fc-126">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="173fc-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="173fc-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="173fc-128">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="173fc-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="173fc-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="173fc-129">Properties</span></span>
|<span data-ttu-id="173fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="173fc-130">Property</span></span>|<span data-ttu-id="173fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="173fc-131">Type</span></span>|<span data-ttu-id="173fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="173fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173fc-133">id</span><span class="sxs-lookup"><span data-stu-id="173fc-133">id</span></span>|<span data-ttu-id="173fc-134">String</span><span class="sxs-lookup"><span data-stu-id="173fc-134">String</span></span>|<span data-ttu-id="173fc-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="173fc-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="173fc-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="173fc-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="173fc-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="173fc-137">Read-only.</span></span>|
|<span data-ttu-id="173fc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="173fc-138">displayName</span></span>|<span data-ttu-id="173fc-139">String</span><span class="sxs-lookup"><span data-stu-id="173fc-139">String</span></span>|<span data-ttu-id="173fc-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="173fc-140">Name of the discovered application.</span></span> <span data-ttu-id="173fc-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="173fc-141">Read-only</span></span>|
|<span data-ttu-id="173fc-142">version</span><span class="sxs-lookup"><span data-stu-id="173fc-142">version</span></span>|<span data-ttu-id="173fc-143">String</span><span class="sxs-lookup"><span data-stu-id="173fc-143">String</span></span>|<span data-ttu-id="173fc-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="173fc-144">Version of the discovered application.</span></span> <span data-ttu-id="173fc-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="173fc-145">Read-only</span></span>|
|<span data-ttu-id="173fc-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="173fc-146">sizeInByte</span></span>|<span data-ttu-id="173fc-147">Int64</span><span class="sxs-lookup"><span data-stu-id="173fc-147">Int64</span></span>|<span data-ttu-id="173fc-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="173fc-148">Discovered application size in bytes.</span></span> <span data-ttu-id="173fc-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="173fc-149">Read-only</span></span>|
|<span data-ttu-id="173fc-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="173fc-150">deviceCount</span></span>|<span data-ttu-id="173fc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="173fc-151">Int32</span></span>|<span data-ttu-id="173fc-152">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="173fc-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="173fc-153">Связи</span><span class="sxs-lookup"><span data-stu-id="173fc-153">Relationships</span></span>
|<span data-ttu-id="173fc-154">Связь</span><span class="sxs-lookup"><span data-stu-id="173fc-154">Relationship</span></span>|<span data-ttu-id="173fc-155">Тип</span><span class="sxs-lookup"><span data-stu-id="173fc-155">Type</span></span>|<span data-ttu-id="173fc-156">Описание</span><span class="sxs-lookup"><span data-stu-id="173fc-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173fc-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="173fc-157">managedDevices</span></span>|<span data-ttu-id="173fc-158">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="173fc-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="173fc-159">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="173fc-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="173fc-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="173fc-160">JSON Representation</span></span>
<span data-ttu-id="173fc-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="173fc-161">Here is a JSON representation of the resource.</span></span>
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





