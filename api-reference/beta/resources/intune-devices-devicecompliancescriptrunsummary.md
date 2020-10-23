---
title: Тип ресурса Девицекомплианцескриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f1968b9573cf65429e9a01dbd25920e114ff4df
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734156"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a><span data-ttu-id="e3ee6-103">Тип ресурса Девицекомплианцескриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="e3ee6-103">deviceComplianceScriptRunSummary resource type</span></span>

<span data-ttu-id="e3ee6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3ee6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3ee6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3ee6-107">Содержит свойства сводки по запуску сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="e3ee6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e3ee6-108">Methods</span></span>
|<span data-ttu-id="e3ee6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e3ee6-109">Method</span></span>|<span data-ttu-id="e3ee6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e3ee6-110">Return Type</span></span>|<span data-ttu-id="e3ee6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e3ee6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3ee6-112">Получение Девицекомплианцескриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="e3ee6-112">Get deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[<span data-ttu-id="e3ee6-113">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e3ee6-113">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="e3ee6-114">Чтение свойств и связей объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e3ee6-114">Read properties and relationships of the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="e3ee6-115">Обновление Девицекомплианцескриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="e3ee6-115">Update deviceComplianceScriptRunSummary</span></span>](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[<span data-ttu-id="e3ee6-116">deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e3ee6-116">deviceComplianceScriptRunSummary</span></span>](../resources/intune-devices-devicecompliancescriptrunsummary.md)|<span data-ttu-id="e3ee6-117">Обновление свойств объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="e3ee6-117">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3ee6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3ee6-118">Properties</span></span>
|<span data-ttu-id="e3ee6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3ee6-119">Property</span></span>|<span data-ttu-id="e3ee6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e3ee6-120">Type</span></span>|<span data-ttu-id="e3ee6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e3ee6-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3ee6-122">id</span><span class="sxs-lookup"><span data-stu-id="e3ee6-122">id</span></span>|<span data-ttu-id="e3ee6-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e3ee6-123">String</span></span>|<span data-ttu-id="e3ee6-124">Ключевой объект сводки запуска сценария соответствия устройства.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-124">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="e3ee6-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-125">This property is read-only.</span></span>|
|<span data-ttu-id="e3ee6-126">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e3ee6-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="e3ee6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="e3ee6-127">Int32</span></span>|<span data-ttu-id="e3ee6-128">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-128">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="e3ee6-129">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e3ee6-129">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e3ee6-130">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e3ee6-130">issueDetectedDeviceCount</span></span>|<span data-ttu-id="e3ee6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e3ee6-131">Int32</span></span>|<span data-ttu-id="e3ee6-132">Количество устройств, для которых сценарий обнаружения обнаружил неполадку.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-132">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="e3ee6-133">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e3ee6-133">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e3ee6-134">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e3ee6-134">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="e3ee6-135">Int32</span><span class="sxs-lookup"><span data-stu-id="e3ee6-135">Int32</span></span>|<span data-ttu-id="e3ee6-136">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-136">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="e3ee6-137">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e3ee6-137">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e3ee6-138">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e3ee6-138">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="e3ee6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e3ee6-139">Int32</span></span>|<span data-ttu-id="e3ee6-140">Количество устройств, на которых еще не выполнялась последняя версия сценария соответствия требованиям устройства.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-140">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="e3ee6-141">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e3ee6-141">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e3ee6-142">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="e3ee6-142">lastScriptRunDateTime</span></span>|<span data-ttu-id="e3ee6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3ee6-143">DateTimeOffset</span></span>|<span data-ttu-id="e3ee6-144">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="e3ee6-144">Last run time for the script across all devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3ee6-145">Связи</span><span class="sxs-lookup"><span data-stu-id="e3ee6-145">Relationships</span></span>
<span data-ttu-id="e3ee6-146">Нет</span><span class="sxs-lookup"><span data-stu-id="e3ee6-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3ee6-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3ee6-147">JSON Representation</span></span>
<span data-ttu-id="e3ee6-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3ee6-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```





