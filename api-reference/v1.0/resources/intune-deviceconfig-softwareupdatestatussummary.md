---
title: Тип ресурса softwareUpdateStatusSummary
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 8813614be9f0fbc87839924a802fcb486a32ba8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319434"
---
# <a name="softwareupdatestatussummary-resource-type"></a><span data-ttu-id="7a89a-103">Тип ресурса softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7a89a-103">softwareUpdateStatusSummary resource type</span></span>

> <span data-ttu-id="7a89a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7a89a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a89a-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7a89a-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="7a89a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7a89a-106">Methods</span></span>
|<span data-ttu-id="7a89a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7a89a-107">Method</span></span>|<span data-ttu-id="7a89a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7a89a-108">Return Type</span></span>|<span data-ttu-id="7a89a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7a89a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7a89a-110">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7a89a-110">Get softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[<span data-ttu-id="7a89a-111">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7a89a-111">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="7a89a-112">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="7a89a-112">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|
|[<span data-ttu-id="7a89a-113">Обновление объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7a89a-113">Update softwareUpdateStatusSummary</span></span>](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[<span data-ttu-id="7a89a-114">softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7a89a-114">softwareUpdateStatusSummary</span></span>](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|<span data-ttu-id="7a89a-115">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="7a89a-115">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7a89a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a89a-116">Properties</span></span>
|<span data-ttu-id="7a89a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a89a-117">Property</span></span>|<span data-ttu-id="7a89a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7a89a-118">Type</span></span>|<span data-ttu-id="7a89a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7a89a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a89a-120">id</span><span class="sxs-lookup"><span data-stu-id="7a89a-120">id</span></span>|<span data-ttu-id="7a89a-121">Строка</span><span class="sxs-lookup"><span data-stu-id="7a89a-121">String</span></span>|<span data-ttu-id="7a89a-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a89a-122">Key of the entity.</span></span>|
|<span data-ttu-id="7a89a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="7a89a-123">displayName</span></span>|<span data-ttu-id="7a89a-124">String</span><span class="sxs-lookup"><span data-stu-id="7a89a-124">String</span></span>|<span data-ttu-id="7a89a-125">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="7a89a-125">The name of the policy.</span></span>|
|<span data-ttu-id="7a89a-126">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-126">compliantDeviceCount</span></span>|<span data-ttu-id="7a89a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-127">Int32</span></span>|<span data-ttu-id="7a89a-128">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7a89a-128">Number of compliant devices.</span></span>|
|<span data-ttu-id="7a89a-129">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-129">nonCompliantDeviceCount</span></span>|<span data-ttu-id="7a89a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-130">Int32</span></span>|<span data-ttu-id="7a89a-131">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7a89a-131">Number of non compliant devices.</span></span>|
|<span data-ttu-id="7a89a-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-132">remediatedDeviceCount</span></span>|<span data-ttu-id="7a89a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-133">Int32</span></span>|<span data-ttu-id="7a89a-134">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7a89a-134">Number of remediated devices.</span></span>|
|<span data-ttu-id="7a89a-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-135">errorDeviceCount</span></span>|<span data-ttu-id="7a89a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-136">Int32</span></span>|<span data-ttu-id="7a89a-137">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7a89a-137">Number of devices had error.</span></span>|
|<span data-ttu-id="7a89a-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-138">unknownDeviceCount</span></span>|<span data-ttu-id="7a89a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-139">Int32</span></span>|<span data-ttu-id="7a89a-140">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="7a89a-140">Number of unknown devices.</span></span>|
|<span data-ttu-id="7a89a-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-141">conflictDeviceCount</span></span>|<span data-ttu-id="7a89a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-142">Int32</span></span>|<span data-ttu-id="7a89a-143">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="7a89a-143">Number of conflict devices.</span></span>|
|<span data-ttu-id="7a89a-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="7a89a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-145">Int32</span></span>|<span data-ttu-id="7a89a-146">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="7a89a-146">Number of not applicable devices.</span></span>|
|<span data-ttu-id="7a89a-147">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-147">compliantUserCount</span></span>|<span data-ttu-id="7a89a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-148">Int32</span></span>|<span data-ttu-id="7a89a-149">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7a89a-149">Number of compliant users.</span></span>|
|<span data-ttu-id="7a89a-150">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-150">nonCompliantUserCount</span></span>|<span data-ttu-id="7a89a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-151">Int32</span></span>|<span data-ttu-id="7a89a-152">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="7a89a-152">Number of non compliant users.</span></span>|
|<span data-ttu-id="7a89a-153">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-153">remediatedUserCount</span></span>|<span data-ttu-id="7a89a-154">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-154">Int32</span></span>|<span data-ttu-id="7a89a-155">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7a89a-155">Number of remediated users.</span></span>|
|<span data-ttu-id="7a89a-156">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-156">errorUserCount</span></span>|<span data-ttu-id="7a89a-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-157">Int32</span></span>|<span data-ttu-id="7a89a-158">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="7a89a-158">Number of users had error.</span></span>|
|<span data-ttu-id="7a89a-159">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-159">unknownUserCount</span></span>|<span data-ttu-id="7a89a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-160">Int32</span></span>|<span data-ttu-id="7a89a-161">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="7a89a-161">Number of unknown users.</span></span>|
|<span data-ttu-id="7a89a-162">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-162">conflictUserCount</span></span>|<span data-ttu-id="7a89a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-163">Int32</span></span>|<span data-ttu-id="7a89a-164">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="7a89a-164">Number of conflict users.</span></span>|
|<span data-ttu-id="7a89a-165">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="7a89a-165">notApplicableUserCount</span></span>|<span data-ttu-id="7a89a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7a89a-166">Int32</span></span>|<span data-ttu-id="7a89a-167">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="7a89a-167">Number of not applicable users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a89a-168">Связи</span><span class="sxs-lookup"><span data-stu-id="7a89a-168">Relationships</span></span>
<span data-ttu-id="7a89a-169">Нет</span><span class="sxs-lookup"><span data-stu-id="7a89a-169">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a89a-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a89a-170">JSON Representation</span></span>
<span data-ttu-id="7a89a-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a89a-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```



