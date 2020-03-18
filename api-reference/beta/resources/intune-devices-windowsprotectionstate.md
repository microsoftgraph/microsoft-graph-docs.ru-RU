---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d42efcc04a060d9585c8d02d17d72449ae0a9c8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783601"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="41073-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="41073-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="41073-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41073-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41073-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41073-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="41073-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="41073-107">Методы</span><span class="sxs-lookup"><span data-stu-id="41073-107">Methods</span></span>
|<span data-ttu-id="41073-108">Метод</span><span class="sxs-lookup"><span data-stu-id="41073-108">Method</span></span>|<span data-ttu-id="41073-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="41073-109">Return Type</span></span>|<span data-ttu-id="41073-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41073-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="41073-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="41073-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="41073-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="41073-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="41073-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="41073-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="41073-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="41073-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="41073-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="41073-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="41073-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="41073-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="41073-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="41073-117">Properties</span></span>
|<span data-ttu-id="41073-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="41073-118">Property</span></span>|<span data-ttu-id="41073-119">Тип</span><span class="sxs-lookup"><span data-stu-id="41073-119">Type</span></span>|<span data-ttu-id="41073-120">Описание</span><span class="sxs-lookup"><span data-stu-id="41073-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41073-121">id</span><span class="sxs-lookup"><span data-stu-id="41073-121">id</span></span>|<span data-ttu-id="41073-122">String</span><span class="sxs-lookup"><span data-stu-id="41073-122">String</span></span>|<span data-ttu-id="41073-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="41073-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="41073-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="41073-124">This is device id of the device</span></span>|
|<span data-ttu-id="41073-125">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="41073-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="41073-126">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-126">Boolean</span></span>|<span data-ttu-id="41073-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="41073-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="41073-128">девицестате</span><span class="sxs-lookup"><span data-stu-id="41073-128">deviceState</span></span>|[<span data-ttu-id="41073-129">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="41073-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="41073-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="41073-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="41073-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="41073-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="41073-132">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="41073-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="41073-133">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-133">Boolean</span></span>|<span data-ttu-id="41073-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="41073-135">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="41073-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="41073-136">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-136">Boolean</span></span>|<span data-ttu-id="41073-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="41073-138">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="41073-138">quickScanOverdue</span></span>|<span data-ttu-id="41073-139">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-139">Boolean</span></span>|<span data-ttu-id="41073-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="41073-141">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="41073-141">fullScanOverdue</span></span>|<span data-ttu-id="41073-142">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-142">Boolean</span></span>|<span data-ttu-id="41073-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="41073-144">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="41073-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="41073-145">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-145">Boolean</span></span>|<span data-ttu-id="41073-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="41073-147">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="41073-147">rebootRequired</span></span>|<span data-ttu-id="41073-148">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-148">Boolean</span></span>|<span data-ttu-id="41073-149">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-149">Reboot required or not?</span></span>|
|<span data-ttu-id="41073-150">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="41073-150">fullScanRequired</span></span>|<span data-ttu-id="41073-151">Логический</span><span class="sxs-lookup"><span data-stu-id="41073-151">Boolean</span></span>|<span data-ttu-id="41073-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="41073-152">Full scan required or not?</span></span>|
|<span data-ttu-id="41073-153">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="41073-153">engineVersion</span></span>|<span data-ttu-id="41073-154">String</span><span class="sxs-lookup"><span data-stu-id="41073-154">String</span></span>|<span data-ttu-id="41073-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="41073-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="41073-156">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="41073-156">signatureVersion</span></span>|<span data-ttu-id="41073-157">String</span><span class="sxs-lookup"><span data-stu-id="41073-157">String</span></span>|<span data-ttu-id="41073-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="41073-158">Current malware definitions version</span></span>|
|<span data-ttu-id="41073-159">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="41073-159">antiMalwareVersion</span></span>|<span data-ttu-id="41073-160">String</span><span class="sxs-lookup"><span data-stu-id="41073-160">String</span></span>|<span data-ttu-id="41073-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="41073-161">Current anti malware version</span></span>|
|<span data-ttu-id="41073-162">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="41073-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="41073-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41073-163">DateTimeOffset</span></span>|<span data-ttu-id="41073-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="41073-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="41073-165">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="41073-165">lastFullScanDateTime</span></span>|<span data-ttu-id="41073-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41073-166">DateTimeOffset</span></span>|<span data-ttu-id="41073-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="41073-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="41073-168">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="41073-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="41073-169">String</span><span class="sxs-lookup"><span data-stu-id="41073-169">String</span></span>|<span data-ttu-id="41073-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="41073-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="41073-171">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="41073-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="41073-172">String</span><span class="sxs-lookup"><span data-stu-id="41073-172">String</span></span>|<span data-ttu-id="41073-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="41073-173">Last full scan signature version</span></span>|
|<span data-ttu-id="41073-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="41073-174">lastReportedDateTime</span></span>|<span data-ttu-id="41073-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41073-175">DateTimeOffset</span></span>|<span data-ttu-id="41073-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="41073-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="41073-177">Связи</span><span class="sxs-lookup"><span data-stu-id="41073-177">Relationships</span></span>
|<span data-ttu-id="41073-178">Связь</span><span class="sxs-lookup"><span data-stu-id="41073-178">Relationship</span></span>|<span data-ttu-id="41073-179">Тип</span><span class="sxs-lookup"><span data-stu-id="41073-179">Type</span></span>|<span data-ttu-id="41073-180">Описание</span><span class="sxs-lookup"><span data-stu-id="41073-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41073-181">детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="41073-181">detectedMalwareState</span></span>|<span data-ttu-id="41073-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="41073-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="41073-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="41073-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41073-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41073-184">JSON Representation</span></span>
<span data-ttu-id="41073-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41073-185">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```



