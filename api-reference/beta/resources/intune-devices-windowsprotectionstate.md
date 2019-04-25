---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520083"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="79c39-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="79c39-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="79c39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79c39-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79c39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79c39-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="79c39-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="79c39-107">Методы</span><span class="sxs-lookup"><span data-stu-id="79c39-107">Methods</span></span>
|<span data-ttu-id="79c39-108">Метод</span><span class="sxs-lookup"><span data-stu-id="79c39-108">Method</span></span>|<span data-ttu-id="79c39-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="79c39-109">Return Type</span></span>|<span data-ttu-id="79c39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="79c39-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="79c39-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="79c39-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="79c39-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="79c39-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="79c39-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="79c39-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="79c39-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="79c39-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="79c39-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="79c39-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="79c39-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="79c39-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79c39-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="79c39-117">Properties</span></span>
|<span data-ttu-id="79c39-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="79c39-118">Property</span></span>|<span data-ttu-id="79c39-119">Тип</span><span class="sxs-lookup"><span data-stu-id="79c39-119">Type</span></span>|<span data-ttu-id="79c39-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79c39-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79c39-121">id</span><span class="sxs-lookup"><span data-stu-id="79c39-121">id</span></span>|<span data-ttu-id="79c39-122">String</span><span class="sxs-lookup"><span data-stu-id="79c39-122">String</span></span>|<span data-ttu-id="79c39-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="79c39-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="79c39-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="79c39-124">This is device id of the device</span></span>|
|<span data-ttu-id="79c39-125">Малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="79c39-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="79c39-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-126">Boolean</span></span>|<span data-ttu-id="79c39-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="79c39-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="79c39-128">Девицестате</span><span class="sxs-lookup"><span data-stu-id="79c39-128">deviceState</span></span>|[<span data-ttu-id="79c39-129">Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="79c39-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="79c39-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="79c39-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="79c39-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="79c39-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="79c39-132">Реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="79c39-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="79c39-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-133">Boolean</span></span>|<span data-ttu-id="79c39-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="79c39-135">Нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="79c39-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="79c39-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-136">Boolean</span></span>|<span data-ttu-id="79c39-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="79c39-138">Куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="79c39-138">quickScanOverdue</span></span>|<span data-ttu-id="79c39-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-139">Boolean</span></span>|<span data-ttu-id="79c39-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="79c39-141">Фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="79c39-141">fullScanOverdue</span></span>|<span data-ttu-id="79c39-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-142">Boolean</span></span>|<span data-ttu-id="79c39-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="79c39-144">Сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="79c39-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="79c39-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-145">Boolean</span></span>|<span data-ttu-id="79c39-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="79c39-147">Ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="79c39-147">rebootRequired</span></span>|<span data-ttu-id="79c39-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-148">Boolean</span></span>|<span data-ttu-id="79c39-149">Требуется переЗагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-149">Reboot required or not?</span></span>|
|<span data-ttu-id="79c39-150">Фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="79c39-150">fullScanRequired</span></span>|<span data-ttu-id="79c39-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c39-151">Boolean</span></span>|<span data-ttu-id="79c39-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="79c39-152">Full scan required or not?</span></span>|
|<span data-ttu-id="79c39-153">Енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="79c39-153">engineVersion</span></span>|<span data-ttu-id="79c39-154">String</span><span class="sxs-lookup"><span data-stu-id="79c39-154">String</span></span>|<span data-ttu-id="79c39-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="79c39-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="79c39-156">Сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="79c39-156">signatureVersion</span></span>|<span data-ttu-id="79c39-157">String</span><span class="sxs-lookup"><span data-stu-id="79c39-157">String</span></span>|<span data-ttu-id="79c39-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="79c39-158">Current malware definitions version</span></span>|
|<span data-ttu-id="79c39-159">Антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="79c39-159">antiMalwareVersion</span></span>|<span data-ttu-id="79c39-160">String</span><span class="sxs-lookup"><span data-stu-id="79c39-160">String</span></span>|<span data-ttu-id="79c39-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="79c39-161">Current anti malware version</span></span>|
|<span data-ttu-id="79c39-162">Ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="79c39-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="79c39-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c39-163">DateTimeOffset</span></span>|<span data-ttu-id="79c39-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="79c39-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="79c39-165">Ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="79c39-165">lastFullScanDateTime</span></span>|<span data-ttu-id="79c39-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c39-166">DateTimeOffset</span></span>|<span data-ttu-id="79c39-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="79c39-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="79c39-168">Ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="79c39-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="79c39-169">String</span><span class="sxs-lookup"><span data-stu-id="79c39-169">String</span></span>|<span data-ttu-id="79c39-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="79c39-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="79c39-171">Ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="79c39-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="79c39-172">String</span><span class="sxs-lookup"><span data-stu-id="79c39-172">String</span></span>|<span data-ttu-id="79c39-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="79c39-173">Last full scan signature version</span></span>|
|<span data-ttu-id="79c39-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="79c39-174">lastReportedDateTime</span></span>|<span data-ttu-id="79c39-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79c39-175">DateTimeOffset</span></span>|<span data-ttu-id="79c39-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="79c39-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="79c39-177">Связи</span><span class="sxs-lookup"><span data-stu-id="79c39-177">Relationships</span></span>
|<span data-ttu-id="79c39-178">Отношение</span><span class="sxs-lookup"><span data-stu-id="79c39-178">Relationship</span></span>|<span data-ttu-id="79c39-179">Тип</span><span class="sxs-lookup"><span data-stu-id="79c39-179">Type</span></span>|<span data-ttu-id="79c39-180">Описание</span><span class="sxs-lookup"><span data-stu-id="79c39-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79c39-181">Детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="79c39-181">detectedMalwareState</span></span>|<span data-ttu-id="79c39-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="79c39-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="79c39-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="79c39-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79c39-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79c39-184">JSON Representation</span></span>
<span data-ttu-id="79c39-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79c39-185">Here is a JSON representation of the resource.</span></span>
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





