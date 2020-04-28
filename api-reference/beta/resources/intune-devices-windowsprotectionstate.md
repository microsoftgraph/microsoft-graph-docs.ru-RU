---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f34c6b1a18d5de654409cedbb384f0390933ba9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419622"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="c729b-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c729b-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="c729b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c729b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c729b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c729b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c729b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c729b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c729b-107">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="c729b-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c729b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c729b-108">Methods</span></span>
|<span data-ttu-id="c729b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c729b-109">Method</span></span>|<span data-ttu-id="c729b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c729b-110">Return Type</span></span>|<span data-ttu-id="c729b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c729b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c729b-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c729b-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="c729b-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c729b-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c729b-114">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c729b-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="c729b-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c729b-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="c729b-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c729b-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c729b-117">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c729b-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c729b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c729b-118">Properties</span></span>
|<span data-ttu-id="c729b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c729b-119">Property</span></span>|<span data-ttu-id="c729b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c729b-120">Type</span></span>|<span data-ttu-id="c729b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c729b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c729b-122">id</span><span class="sxs-lookup"><span data-stu-id="c729b-122">id</span></span>|<span data-ttu-id="c729b-123">String</span><span class="sxs-lookup"><span data-stu-id="c729b-123">String</span></span>|<span data-ttu-id="c729b-124">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="c729b-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="c729b-125">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="c729b-125">This is device id of the device</span></span>|
|<span data-ttu-id="c729b-126">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="c729b-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="c729b-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-127">Boolean</span></span>|<span data-ttu-id="c729b-128">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="c729b-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="c729b-129">девицестате</span><span class="sxs-lookup"><span data-stu-id="c729b-129">deviceState</span></span>|[<span data-ttu-id="c729b-130">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="c729b-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="c729b-131">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="c729b-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="c729b-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="c729b-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="c729b-133">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="c729b-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="c729b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-134">Boolean</span></span>|<span data-ttu-id="c729b-135">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="c729b-136">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="c729b-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="c729b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-137">Boolean</span></span>|<span data-ttu-id="c729b-138">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="c729b-139">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="c729b-139">quickScanOverdue</span></span>|<span data-ttu-id="c729b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-140">Boolean</span></span>|<span data-ttu-id="c729b-141">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="c729b-142">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="c729b-142">fullScanOverdue</span></span>|<span data-ttu-id="c729b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-143">Boolean</span></span>|<span data-ttu-id="c729b-144">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="c729b-145">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="c729b-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="c729b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-146">Boolean</span></span>|<span data-ttu-id="c729b-147">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="c729b-148">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="c729b-148">rebootRequired</span></span>|<span data-ttu-id="c729b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-149">Boolean</span></span>|<span data-ttu-id="c729b-150">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-150">Reboot required or not?</span></span>|
|<span data-ttu-id="c729b-151">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="c729b-151">fullScanRequired</span></span>|<span data-ttu-id="c729b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c729b-152">Boolean</span></span>|<span data-ttu-id="c729b-153">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="c729b-153">Full scan required or not?</span></span>|
|<span data-ttu-id="c729b-154">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="c729b-154">engineVersion</span></span>|<span data-ttu-id="c729b-155">String</span><span class="sxs-lookup"><span data-stu-id="c729b-155">String</span></span>|<span data-ttu-id="c729b-156">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="c729b-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="c729b-157">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c729b-157">signatureVersion</span></span>|<span data-ttu-id="c729b-158">String</span><span class="sxs-lookup"><span data-stu-id="c729b-158">String</span></span>|<span data-ttu-id="c729b-159">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="c729b-159">Current malware definitions version</span></span>|
|<span data-ttu-id="c729b-160">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="c729b-160">antiMalwareVersion</span></span>|<span data-ttu-id="c729b-161">String</span><span class="sxs-lookup"><span data-stu-id="c729b-161">String</span></span>|<span data-ttu-id="c729b-162">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="c729b-162">Current anti malware version</span></span>|
|<span data-ttu-id="c729b-163">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="c729b-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="c729b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c729b-164">DateTimeOffset</span></span>|<span data-ttu-id="c729b-165">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c729b-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="c729b-166">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="c729b-166">lastFullScanDateTime</span></span>|<span data-ttu-id="c729b-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c729b-167">DateTimeOffset</span></span>|<span data-ttu-id="c729b-168">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c729b-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="c729b-169">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c729b-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="c729b-170">String</span><span class="sxs-lookup"><span data-stu-id="c729b-170">String</span></span>|<span data-ttu-id="c729b-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c729b-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="c729b-172">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c729b-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="c729b-173">String</span><span class="sxs-lookup"><span data-stu-id="c729b-173">String</span></span>|<span data-ttu-id="c729b-174">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="c729b-174">Last full scan signature version</span></span>|
|<span data-ttu-id="c729b-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c729b-175">lastReportedDateTime</span></span>|<span data-ttu-id="c729b-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c729b-176">DateTimeOffset</span></span>|<span data-ttu-id="c729b-177">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="c729b-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="c729b-178">Связи</span><span class="sxs-lookup"><span data-stu-id="c729b-178">Relationships</span></span>
|<span data-ttu-id="c729b-179">Связь</span><span class="sxs-lookup"><span data-stu-id="c729b-179">Relationship</span></span>|<span data-ttu-id="c729b-180">Тип</span><span class="sxs-lookup"><span data-stu-id="c729b-180">Type</span></span>|<span data-ttu-id="c729b-181">Описание</span><span class="sxs-lookup"><span data-stu-id="c729b-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c729b-182">детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="c729b-182">detectedMalwareState</span></span>|<span data-ttu-id="c729b-183">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="c729b-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="c729b-184">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="c729b-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c729b-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c729b-185">JSON Representation</span></span>
<span data-ttu-id="c729b-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c729b-186">Here is a JSON representation of the resource.</span></span>
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



