---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803103"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="46cbe-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="46cbe-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="46cbe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46cbe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46cbe-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="46cbe-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="46cbe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="46cbe-107">Methods</span></span>
|<span data-ttu-id="46cbe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="46cbe-108">Method</span></span>|<span data-ttu-id="46cbe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="46cbe-109">Return Type</span></span>|<span data-ttu-id="46cbe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="46cbe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46cbe-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="46cbe-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="46cbe-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="46cbe-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="46cbe-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="46cbe-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="46cbe-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="46cbe-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="46cbe-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="46cbe-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="46cbe-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="46cbe-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="46cbe-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="46cbe-117">Properties</span></span>
|<span data-ttu-id="46cbe-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="46cbe-118">Property</span></span>|<span data-ttu-id="46cbe-119">Тип</span><span class="sxs-lookup"><span data-stu-id="46cbe-119">Type</span></span>|<span data-ttu-id="46cbe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="46cbe-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46cbe-121">id</span><span class="sxs-lookup"><span data-stu-id="46cbe-121">id</span></span>|<span data-ttu-id="46cbe-122">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-122">String</span></span>|<span data-ttu-id="46cbe-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="46cbe-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="46cbe-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="46cbe-124">This is device id of the device</span></span>|
|<span data-ttu-id="46cbe-125">Малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="46cbe-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="46cbe-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-126">Boolean</span></span>|<span data-ttu-id="46cbe-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="46cbe-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="46cbe-128">Девицестате</span><span class="sxs-lookup"><span data-stu-id="46cbe-128">deviceState</span></span>|[<span data-ttu-id="46cbe-129">Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="46cbe-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="46cbe-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="46cbe-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="46cbe-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="46cbe-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="46cbe-132">Реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="46cbe-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="46cbe-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-133">Boolean</span></span>|<span data-ttu-id="46cbe-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="46cbe-135">Нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="46cbe-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="46cbe-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-136">Boolean</span></span>|<span data-ttu-id="46cbe-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="46cbe-138">Куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="46cbe-138">quickScanOverdue</span></span>|<span data-ttu-id="46cbe-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-139">Boolean</span></span>|<span data-ttu-id="46cbe-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="46cbe-141">Фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="46cbe-141">fullScanOverdue</span></span>|<span data-ttu-id="46cbe-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-142">Boolean</span></span>|<span data-ttu-id="46cbe-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="46cbe-144">Сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="46cbe-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="46cbe-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-145">Boolean</span></span>|<span data-ttu-id="46cbe-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="46cbe-147">Ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="46cbe-147">rebootRequired</span></span>|<span data-ttu-id="46cbe-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-148">Boolean</span></span>|<span data-ttu-id="46cbe-149">Требуется переЗагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-149">Reboot required or not?</span></span>|
|<span data-ttu-id="46cbe-150">Фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="46cbe-150">fullScanRequired</span></span>|<span data-ttu-id="46cbe-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="46cbe-151">Boolean</span></span>|<span data-ttu-id="46cbe-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="46cbe-152">Full scan required or not?</span></span>|
|<span data-ttu-id="46cbe-153">Енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="46cbe-153">engineVersion</span></span>|<span data-ttu-id="46cbe-154">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-154">String</span></span>|<span data-ttu-id="46cbe-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="46cbe-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="46cbe-156">Сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="46cbe-156">signatureVersion</span></span>|<span data-ttu-id="46cbe-157">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-157">String</span></span>|<span data-ttu-id="46cbe-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="46cbe-158">Current malware definitions version</span></span>|
|<span data-ttu-id="46cbe-159">Антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="46cbe-159">antiMalwareVersion</span></span>|<span data-ttu-id="46cbe-160">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-160">String</span></span>|<span data-ttu-id="46cbe-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="46cbe-161">Current anti malware version</span></span>|
|<span data-ttu-id="46cbe-162">Ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="46cbe-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="46cbe-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46cbe-163">DateTimeOffset</span></span>|<span data-ttu-id="46cbe-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="46cbe-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="46cbe-165">Ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="46cbe-165">lastFullScanDateTime</span></span>|<span data-ttu-id="46cbe-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46cbe-166">DateTimeOffset</span></span>|<span data-ttu-id="46cbe-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="46cbe-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="46cbe-168">Ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="46cbe-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="46cbe-169">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-169">String</span></span>|<span data-ttu-id="46cbe-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="46cbe-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="46cbe-171">Ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="46cbe-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="46cbe-172">String</span><span class="sxs-lookup"><span data-stu-id="46cbe-172">String</span></span>|<span data-ttu-id="46cbe-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="46cbe-173">Last full scan signature version</span></span>|
|<span data-ttu-id="46cbe-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="46cbe-174">lastReportedDateTime</span></span>|<span data-ttu-id="46cbe-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46cbe-175">DateTimeOffset</span></span>|<span data-ttu-id="46cbe-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="46cbe-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="46cbe-177">Связи</span><span class="sxs-lookup"><span data-stu-id="46cbe-177">Relationships</span></span>
|<span data-ttu-id="46cbe-178">Отношение</span><span class="sxs-lookup"><span data-stu-id="46cbe-178">Relationship</span></span>|<span data-ttu-id="46cbe-179">Тип</span><span class="sxs-lookup"><span data-stu-id="46cbe-179">Type</span></span>|<span data-ttu-id="46cbe-180">Описание</span><span class="sxs-lookup"><span data-stu-id="46cbe-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46cbe-181">Детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="46cbe-181">detectedMalwareState</span></span>|<span data-ttu-id="46cbe-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="46cbe-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="46cbe-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="46cbe-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46cbe-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46cbe-184">JSON Representation</span></span>
<span data-ttu-id="46cbe-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46cbe-185">Here is a JSON representation of the resource.</span></span>
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





