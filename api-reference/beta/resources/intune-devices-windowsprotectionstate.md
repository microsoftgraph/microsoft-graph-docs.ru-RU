---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00a04fe2f20270cdd0892829406fdccb240989ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080462"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="5e253-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5e253-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="5e253-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e253-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e253-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e253-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e253-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e253-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e253-107">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="5e253-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5e253-108">Методы</span><span class="sxs-lookup"><span data-stu-id="5e253-108">Methods</span></span>
|<span data-ttu-id="5e253-109">Метод</span><span class="sxs-lookup"><span data-stu-id="5e253-109">Method</span></span>|<span data-ttu-id="5e253-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e253-110">Return Type</span></span>|<span data-ttu-id="5e253-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e253-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e253-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5e253-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="5e253-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5e253-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5e253-114">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5e253-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="5e253-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5e253-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="5e253-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="5e253-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="5e253-117">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="5e253-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e253-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e253-118">Properties</span></span>
|<span data-ttu-id="5e253-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e253-119">Property</span></span>|<span data-ttu-id="5e253-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5e253-120">Type</span></span>|<span data-ttu-id="5e253-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5e253-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e253-122">id</span><span class="sxs-lookup"><span data-stu-id="5e253-122">id</span></span>|<span data-ttu-id="5e253-123">String</span><span class="sxs-lookup"><span data-stu-id="5e253-123">String</span></span>|<span data-ttu-id="5e253-124">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="5e253-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="5e253-125">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="5e253-125">This is device id of the device</span></span>|
|<span data-ttu-id="5e253-126">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="5e253-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="5e253-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-127">Boolean</span></span>|<span data-ttu-id="5e253-128">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="5e253-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="5e253-129">девицестате</span><span class="sxs-lookup"><span data-stu-id="5e253-129">deviceState</span></span>|[<span data-ttu-id="5e253-130">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="5e253-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="5e253-131">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5e253-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="5e253-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="5e253-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="5e253-133">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="5e253-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="5e253-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-134">Boolean</span></span>|<span data-ttu-id="5e253-135">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="5e253-136">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="5e253-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="5e253-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-137">Boolean</span></span>|<span data-ttu-id="5e253-138">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="5e253-139">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="5e253-139">quickScanOverdue</span></span>|<span data-ttu-id="5e253-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-140">Boolean</span></span>|<span data-ttu-id="5e253-141">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="5e253-142">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="5e253-142">fullScanOverdue</span></span>|<span data-ttu-id="5e253-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-143">Boolean</span></span>|<span data-ttu-id="5e253-144">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="5e253-145">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="5e253-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="5e253-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-146">Boolean</span></span>|<span data-ttu-id="5e253-147">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="5e253-148">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="5e253-148">rebootRequired</span></span>|<span data-ttu-id="5e253-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-149">Boolean</span></span>|<span data-ttu-id="5e253-150">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-150">Reboot required or not?</span></span>|
|<span data-ttu-id="5e253-151">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="5e253-151">fullScanRequired</span></span>|<span data-ttu-id="5e253-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e253-152">Boolean</span></span>|<span data-ttu-id="5e253-153">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="5e253-153">Full scan required or not?</span></span>|
|<span data-ttu-id="5e253-154">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="5e253-154">engineVersion</span></span>|<span data-ttu-id="5e253-155">String</span><span class="sxs-lookup"><span data-stu-id="5e253-155">String</span></span>|<span data-ttu-id="5e253-156">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="5e253-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="5e253-157">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5e253-157">signatureVersion</span></span>|<span data-ttu-id="5e253-158">String</span><span class="sxs-lookup"><span data-stu-id="5e253-158">String</span></span>|<span data-ttu-id="5e253-159">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="5e253-159">Current malware definitions version</span></span>|
|<span data-ttu-id="5e253-160">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="5e253-160">antiMalwareVersion</span></span>|<span data-ttu-id="5e253-161">String</span><span class="sxs-lookup"><span data-stu-id="5e253-161">String</span></span>|<span data-ttu-id="5e253-162">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="5e253-162">Current anti malware version</span></span>|
|<span data-ttu-id="5e253-163">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="5e253-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="5e253-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e253-164">DateTimeOffset</span></span>|<span data-ttu-id="5e253-165">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5e253-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="5e253-166">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="5e253-166">lastFullScanDateTime</span></span>|<span data-ttu-id="5e253-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e253-167">DateTimeOffset</span></span>|<span data-ttu-id="5e253-168">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5e253-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="5e253-169">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5e253-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="5e253-170">String</span><span class="sxs-lookup"><span data-stu-id="5e253-170">String</span></span>|<span data-ttu-id="5e253-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="5e253-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="5e253-172">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="5e253-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="5e253-173">String</span><span class="sxs-lookup"><span data-stu-id="5e253-173">String</span></span>|<span data-ttu-id="5e253-174">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="5e253-174">Last full scan signature version</span></span>|
|<span data-ttu-id="5e253-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e253-175">lastReportedDateTime</span></span>|<span data-ttu-id="5e253-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e253-176">DateTimeOffset</span></span>|<span data-ttu-id="5e253-177">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="5e253-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e253-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e253-178">Relationships</span></span>
|<span data-ttu-id="5e253-179">Связь</span><span class="sxs-lookup"><span data-stu-id="5e253-179">Relationship</span></span>|<span data-ttu-id="5e253-180">Тип</span><span class="sxs-lookup"><span data-stu-id="5e253-180">Type</span></span>|<span data-ttu-id="5e253-181">Описание</span><span class="sxs-lookup"><span data-stu-id="5e253-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e253-182">детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="5e253-182">detectedMalwareState</span></span>|<span data-ttu-id="5e253-183">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="5e253-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="5e253-184">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="5e253-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e253-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e253-185">JSON Representation</span></span>
<span data-ttu-id="5e253-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e253-186">Here is a JSON representation of the resource.</span></span>
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






