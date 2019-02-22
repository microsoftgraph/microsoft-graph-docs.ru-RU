---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eebf798a41e5cbab27fab849cdead8a288a782e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148316"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="955de-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955de-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="955de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="955de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="955de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="955de-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="955de-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="955de-107">Методы</span><span class="sxs-lookup"><span data-stu-id="955de-107">Methods</span></span>
|<span data-ttu-id="955de-108">Метод</span><span class="sxs-lookup"><span data-stu-id="955de-108">Method</span></span>|<span data-ttu-id="955de-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="955de-109">Return Type</span></span>|<span data-ttu-id="955de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="955de-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="955de-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955de-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="955de-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955de-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="955de-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="955de-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="955de-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955de-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="955de-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="955de-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="955de-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="955de-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="955de-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="955de-117">Properties</span></span>
|<span data-ttu-id="955de-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="955de-118">Property</span></span>|<span data-ttu-id="955de-119">Тип</span><span class="sxs-lookup"><span data-stu-id="955de-119">Type</span></span>|<span data-ttu-id="955de-120">Описание</span><span class="sxs-lookup"><span data-stu-id="955de-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955de-121">id</span><span class="sxs-lookup"><span data-stu-id="955de-121">id</span></span>|<span data-ttu-id="955de-122">String</span><span class="sxs-lookup"><span data-stu-id="955de-122">String</span></span>|<span data-ttu-id="955de-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="955de-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="955de-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="955de-124">This is device id of the device</span></span>|
|<span data-ttu-id="955de-125">Малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="955de-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="955de-126">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-126">Boolean</span></span>|<span data-ttu-id="955de-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="955de-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="955de-128">Девицестате</span><span class="sxs-lookup"><span data-stu-id="955de-128">deviceState</span></span>|[<span data-ttu-id="955de-129">Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="955de-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="955de-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="955de-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="955de-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="955de-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="955de-132">Реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="955de-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="955de-133">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-133">Boolean</span></span>|<span data-ttu-id="955de-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="955de-135">Нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="955de-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="955de-136">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-136">Boolean</span></span>|<span data-ttu-id="955de-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="955de-138">Куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="955de-138">quickScanOverdue</span></span>|<span data-ttu-id="955de-139">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-139">Boolean</span></span>|<span data-ttu-id="955de-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="955de-141">Фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="955de-141">fullScanOverdue</span></span>|<span data-ttu-id="955de-142">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-142">Boolean</span></span>|<span data-ttu-id="955de-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="955de-144">Сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="955de-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="955de-145">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-145">Boolean</span></span>|<span data-ttu-id="955de-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="955de-147">Ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="955de-147">rebootRequired</span></span>|<span data-ttu-id="955de-148">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-148">Boolean</span></span>|<span data-ttu-id="955de-149">Требуется переЗагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-149">Reboot required or not?</span></span>|
|<span data-ttu-id="955de-150">Фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="955de-150">fullScanRequired</span></span>|<span data-ttu-id="955de-151">Логический</span><span class="sxs-lookup"><span data-stu-id="955de-151">Boolean</span></span>|<span data-ttu-id="955de-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="955de-152">Full scan required or not?</span></span>|
|<span data-ttu-id="955de-153">Енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="955de-153">engineVersion</span></span>|<span data-ttu-id="955de-154">String</span><span class="sxs-lookup"><span data-stu-id="955de-154">String</span></span>|<span data-ttu-id="955de-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="955de-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="955de-156">Сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955de-156">signatureVersion</span></span>|<span data-ttu-id="955de-157">String</span><span class="sxs-lookup"><span data-stu-id="955de-157">String</span></span>|<span data-ttu-id="955de-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="955de-158">Current malware definitions version</span></span>|
|<span data-ttu-id="955de-159">Антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="955de-159">antiMalwareVersion</span></span>|<span data-ttu-id="955de-160">String</span><span class="sxs-lookup"><span data-stu-id="955de-160">String</span></span>|<span data-ttu-id="955de-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="955de-161">Current anti malware version</span></span>|
|<span data-ttu-id="955de-162">Ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="955de-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="955de-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955de-163">DateTimeOffset</span></span>|<span data-ttu-id="955de-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955de-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="955de-165">Ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="955de-165">lastFullScanDateTime</span></span>|<span data-ttu-id="955de-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955de-166">DateTimeOffset</span></span>|<span data-ttu-id="955de-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955de-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="955de-168">Ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955de-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="955de-169">String</span><span class="sxs-lookup"><span data-stu-id="955de-169">String</span></span>|<span data-ttu-id="955de-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="955de-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="955de-171">Ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="955de-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="955de-172">String</span><span class="sxs-lookup"><span data-stu-id="955de-172">String</span></span>|<span data-ttu-id="955de-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="955de-173">Last full scan signature version</span></span>|
|<span data-ttu-id="955de-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="955de-174">lastReportedDateTime</span></span>|<span data-ttu-id="955de-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="955de-175">DateTimeOffset</span></span>|<span data-ttu-id="955de-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="955de-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="955de-177">Отношения</span><span class="sxs-lookup"><span data-stu-id="955de-177">Relationships</span></span>
|<span data-ttu-id="955de-178">Связь</span><span class="sxs-lookup"><span data-stu-id="955de-178">Relationship</span></span>|<span data-ttu-id="955de-179">Тип</span><span class="sxs-lookup"><span data-stu-id="955de-179">Type</span></span>|<span data-ttu-id="955de-180">Описание</span><span class="sxs-lookup"><span data-stu-id="955de-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="955de-181">Детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="955de-181">detectedMalwareState</span></span>|<span data-ttu-id="955de-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="955de-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="955de-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="955de-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="955de-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="955de-184">JSON Representation</span></span>
<span data-ttu-id="955de-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="955de-185">Here is a JSON representation of the resource.</span></span>
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




