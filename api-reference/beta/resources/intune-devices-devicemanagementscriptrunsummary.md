---
title: Тип ресурса Девицеманажементскриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6807114ebaf7ba3a778520c7b2a383f5a13c31f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522449"
---
# <a name="devicemanagementscriptrunsummary-resource-type"></a><span data-ttu-id="cf141-103">Тип ресурса Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="cf141-103">deviceManagementScriptRunSummary resource type</span></span>

> <span data-ttu-id="cf141-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf141-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf141-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf141-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf141-106">Содержит свойства сводки по запуску сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf141-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="cf141-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cf141-107">Methods</span></span>
|<span data-ttu-id="cf141-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cf141-108">Method</span></span>|<span data-ttu-id="cf141-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf141-109">Return Type</span></span>|<span data-ttu-id="cf141-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cf141-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf141-111">Получение Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="cf141-111">Get deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-get.md)|<span data-ttu-id="cf141-112">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="cf141-112">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="cf141-113">Чтение свойств и связей объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cf141-113">Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="cf141-114">Обновление Девицеманажементскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="cf141-114">Update deviceManagementScriptRunSummary</span></span>](../api/intune-devices-devicemanagementscriptrunsummary-update.md)|<span data-ttu-id="cf141-115">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);</span><span class="sxs-lookup"><span data-stu-id="cf141-115">[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)</span></span>|<span data-ttu-id="cf141-116">Обновление свойств объекта [девицеманажементскриптрунсуммари](../resources/intune-devices-devicemanagementscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cf141-116">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf141-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf141-117">Properties</span></span>
|<span data-ttu-id="cf141-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf141-118">Property</span></span>|<span data-ttu-id="cf141-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cf141-119">Type</span></span>|<span data-ttu-id="cf141-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cf141-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf141-121">id</span><span class="sxs-lookup"><span data-stu-id="cf141-121">id</span></span>|<span data-ttu-id="cf141-122">String</span><span class="sxs-lookup"><span data-stu-id="cf141-122">String</span></span>|<span data-ttu-id="cf141-123">Key объекта сводки запуска сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="cf141-123">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="cf141-124">Сукцессдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cf141-124">successDeviceCount</span></span>|<span data-ttu-id="cf141-125">Int32</span><span class="sxs-lookup"><span data-stu-id="cf141-125">Int32</span></span>|<span data-ttu-id="cf141-126">Число устройств для успешной попытки.</span><span class="sxs-lookup"><span data-stu-id="cf141-126">Success device count.</span></span>|
|<span data-ttu-id="cf141-127">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cf141-127">errorDeviceCount</span></span>|<span data-ttu-id="cf141-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cf141-128">Int32</span></span>|<span data-ttu-id="cf141-129">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="cf141-129">Error device count.</span></span>|
|<span data-ttu-id="cf141-130">Сукцессусеркаунт</span><span class="sxs-lookup"><span data-stu-id="cf141-130">successUserCount</span></span>|<span data-ttu-id="cf141-131">Int32</span><span class="sxs-lookup"><span data-stu-id="cf141-131">Int32</span></span>|<span data-ttu-id="cf141-132">Число пользователей Success.</span><span class="sxs-lookup"><span data-stu-id="cf141-132">Success user count.</span></span>|
|<span data-ttu-id="cf141-133">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="cf141-133">errorUserCount</span></span>|<span data-ttu-id="cf141-134">Int32</span><span class="sxs-lookup"><span data-stu-id="cf141-134">Int32</span></span>|<span data-ttu-id="cf141-135">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="cf141-135">Error user count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf141-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="cf141-136">Relationships</span></span>
<span data-ttu-id="cf141-137">Нет</span><span class="sxs-lookup"><span data-stu-id="cf141-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf141-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf141-138">JSON Representation</span></span>
<span data-ttu-id="cf141-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf141-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "successUserCount": 1024,
  "errorUserCount": 1024
}
```





