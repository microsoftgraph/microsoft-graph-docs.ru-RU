---
title: Тип ресурса detectedApp
description: Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство. Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddc854a825241b2a7b87d18faaaa7e8399c2fb1c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968892"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="1dafe-104">Тип ресурса detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-104">detectedApp resource type</span></span>

> <span data-ttu-id="1dafe-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1dafe-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dafe-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dafe-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dafe-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1dafe-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dafe-108">Управляемое или неуправляемое приложение, которое устанавливается на управляемое устройство.</span><span class="sxs-lookup"><span data-stu-id="1dafe-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="1dafe-109">Неуправляемые приложения отображаются только на устройствах, относящихся к корпоративной собственности.</span><span class="sxs-lookup"><span data-stu-id="1dafe-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="1dafe-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1dafe-110">Methods</span></span>
|<span data-ttu-id="1dafe-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1dafe-111">Method</span></span>|<span data-ttu-id="1dafe-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1dafe-112">Return Type</span></span>|<span data-ttu-id="1dafe-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1dafe-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1dafe-114">Список detectedApps</span><span class="sxs-lookup"><span data-stu-id="1dafe-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="1dafe-115">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1dafe-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="1dafe-116">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dafe-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="1dafe-117">Получение detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="1dafe-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="1dafe-119">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dafe-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="1dafe-120">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="1dafe-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="1dafe-122">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dafe-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="1dafe-123">Удаление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="1dafe-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1dafe-124">None</span></span>|<span data-ttu-id="1dafe-125">Удаление объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dafe-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="1dafe-126">Обновление detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="1dafe-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="1dafe-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="1dafe-128">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1dafe-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1dafe-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dafe-129">Properties</span></span>
|<span data-ttu-id="1dafe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dafe-130">Property</span></span>|<span data-ttu-id="1dafe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1dafe-131">Type</span></span>|<span data-ttu-id="1dafe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1dafe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dafe-133">id</span><span class="sxs-lookup"><span data-stu-id="1dafe-133">id</span></span>|<span data-ttu-id="1dafe-134">String</span><span class="sxs-lookup"><span data-stu-id="1dafe-134">String</span></span>|<span data-ttu-id="1dafe-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="1dafe-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="1dafe-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="1dafe-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="1dafe-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1dafe-137">Read-only.</span></span>|
|<span data-ttu-id="1dafe-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1dafe-138">displayName</span></span>|<span data-ttu-id="1dafe-139">String</span><span class="sxs-lookup"><span data-stu-id="1dafe-139">String</span></span>|<span data-ttu-id="1dafe-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="1dafe-140">Name of the discovered application.</span></span> <span data-ttu-id="1dafe-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1dafe-141">Read-only</span></span>|
|<span data-ttu-id="1dafe-142">version</span><span class="sxs-lookup"><span data-stu-id="1dafe-142">version</span></span>|<span data-ttu-id="1dafe-143">String</span><span class="sxs-lookup"><span data-stu-id="1dafe-143">String</span></span>|<span data-ttu-id="1dafe-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="1dafe-144">Version of the discovered application.</span></span> <span data-ttu-id="1dafe-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1dafe-145">Read-only</span></span>|
|<span data-ttu-id="1dafe-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="1dafe-146">sizeInByte</span></span>|<span data-ttu-id="1dafe-147">Int64</span><span class="sxs-lookup"><span data-stu-id="1dafe-147">Int64</span></span>|<span data-ttu-id="1dafe-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="1dafe-148">Discovered application size in bytes.</span></span> <span data-ttu-id="1dafe-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1dafe-149">Read-only</span></span>|
|<span data-ttu-id="1dafe-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1dafe-150">deviceCount</span></span>|<span data-ttu-id="1dafe-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1dafe-151">Int32</span></span>|<span data-ttu-id="1dafe-152">Количество устройств, на которых было успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="1dafe-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dafe-153">Связи</span><span class="sxs-lookup"><span data-stu-id="1dafe-153">Relationships</span></span>
|<span data-ttu-id="1dafe-154">Связь</span><span class="sxs-lookup"><span data-stu-id="1dafe-154">Relationship</span></span>|<span data-ttu-id="1dafe-155">Тип</span><span class="sxs-lookup"><span data-stu-id="1dafe-155">Type</span></span>|<span data-ttu-id="1dafe-156">Описание</span><span class="sxs-lookup"><span data-stu-id="1dafe-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dafe-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="1dafe-157">managedDevices</span></span>|<span data-ttu-id="1dafe-158">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="1dafe-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="1dafe-159">Устройства, на которых установлено обнаруженное приложение</span><span class="sxs-lookup"><span data-stu-id="1dafe-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dafe-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dafe-160">JSON Representation</span></span>
<span data-ttu-id="1dafe-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dafe-161">Here is a JSON representation of the resource.</span></span>
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





