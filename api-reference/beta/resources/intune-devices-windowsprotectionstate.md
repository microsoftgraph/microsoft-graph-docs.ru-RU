---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd507daef4d9055dcabce1e90481e22a77ec8180
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983920"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="bc477-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc477-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="bc477-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc477-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc477-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc477-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc477-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="bc477-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="bc477-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bc477-107">Methods</span></span>
|<span data-ttu-id="bc477-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bc477-108">Method</span></span>|<span data-ttu-id="bc477-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc477-109">Return Type</span></span>|<span data-ttu-id="bc477-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc477-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc477-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc477-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="bc477-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc477-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="bc477-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bc477-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="bc477-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc477-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="bc477-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="bc477-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="bc477-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="bc477-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc477-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc477-117">Properties</span></span>
|<span data-ttu-id="bc477-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc477-118">Property</span></span>|<span data-ttu-id="bc477-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bc477-119">Type</span></span>|<span data-ttu-id="bc477-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bc477-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc477-121">id</span><span class="sxs-lookup"><span data-stu-id="bc477-121">id</span></span>|<span data-ttu-id="bc477-122">String</span><span class="sxs-lookup"><span data-stu-id="bc477-122">String</span></span>|<span data-ttu-id="bc477-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="bc477-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="bc477-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="bc477-124">This is device id of the device</span></span>|
|<span data-ttu-id="bc477-125">Малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="bc477-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="bc477-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-126">Boolean</span></span>|<span data-ttu-id="bc477-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="bc477-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="bc477-128">Девицестате</span><span class="sxs-lookup"><span data-stu-id="bc477-128">deviceState</span></span>|[<span data-ttu-id="bc477-129">Виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="bc477-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="bc477-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="bc477-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="bc477-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="bc477-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="bc477-132">Реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="bc477-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="bc477-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-133">Boolean</span></span>|<span data-ttu-id="bc477-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="bc477-135">Нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="bc477-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="bc477-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-136">Boolean</span></span>|<span data-ttu-id="bc477-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="bc477-138">Куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="bc477-138">quickScanOverdue</span></span>|<span data-ttu-id="bc477-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-139">Boolean</span></span>|<span data-ttu-id="bc477-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="bc477-141">Фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="bc477-141">fullScanOverdue</span></span>|<span data-ttu-id="bc477-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-142">Boolean</span></span>|<span data-ttu-id="bc477-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="bc477-144">Сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="bc477-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="bc477-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-145">Boolean</span></span>|<span data-ttu-id="bc477-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="bc477-147">Ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="bc477-147">rebootRequired</span></span>|<span data-ttu-id="bc477-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-148">Boolean</span></span>|<span data-ttu-id="bc477-149">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-149">Reboot required or not?</span></span>|
|<span data-ttu-id="bc477-150">Фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="bc477-150">fullScanRequired</span></span>|<span data-ttu-id="bc477-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc477-151">Boolean</span></span>|<span data-ttu-id="bc477-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="bc477-152">Full scan required or not?</span></span>|
|<span data-ttu-id="bc477-153">Енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="bc477-153">engineVersion</span></span>|<span data-ttu-id="bc477-154">String</span><span class="sxs-lookup"><span data-stu-id="bc477-154">String</span></span>|<span data-ttu-id="bc477-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="bc477-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="bc477-156">Сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="bc477-156">signatureVersion</span></span>|<span data-ttu-id="bc477-157">String</span><span class="sxs-lookup"><span data-stu-id="bc477-157">String</span></span>|<span data-ttu-id="bc477-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="bc477-158">Current malware definitions version</span></span>|
|<span data-ttu-id="bc477-159">Антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="bc477-159">antiMalwareVersion</span></span>|<span data-ttu-id="bc477-160">String</span><span class="sxs-lookup"><span data-stu-id="bc477-160">String</span></span>|<span data-ttu-id="bc477-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="bc477-161">Current anti malware version</span></span>|
|<span data-ttu-id="bc477-162">Ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="bc477-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="bc477-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc477-163">DateTimeOffset</span></span>|<span data-ttu-id="bc477-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="bc477-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="bc477-165">Ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="bc477-165">lastFullScanDateTime</span></span>|<span data-ttu-id="bc477-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc477-166">DateTimeOffset</span></span>|<span data-ttu-id="bc477-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="bc477-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="bc477-168">Ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="bc477-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="bc477-169">String</span><span class="sxs-lookup"><span data-stu-id="bc477-169">String</span></span>|<span data-ttu-id="bc477-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="bc477-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="bc477-171">Ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="bc477-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="bc477-172">String</span><span class="sxs-lookup"><span data-stu-id="bc477-172">String</span></span>|<span data-ttu-id="bc477-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="bc477-173">Last full scan signature version</span></span>|
|<span data-ttu-id="bc477-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc477-174">lastReportedDateTime</span></span>|<span data-ttu-id="bc477-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc477-175">DateTimeOffset</span></span>|<span data-ttu-id="bc477-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="bc477-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc477-177">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc477-177">Relationships</span></span>
|<span data-ttu-id="bc477-178">Отношение</span><span class="sxs-lookup"><span data-stu-id="bc477-178">Relationship</span></span>|<span data-ttu-id="bc477-179">Тип</span><span class="sxs-lookup"><span data-stu-id="bc477-179">Type</span></span>|<span data-ttu-id="bc477-180">Описание</span><span class="sxs-lookup"><span data-stu-id="bc477-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc477-181">Детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="bc477-181">detectedMalwareState</span></span>|<span data-ttu-id="bc477-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="bc477-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="bc477-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="bc477-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc477-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc477-184">JSON Representation</span></span>
<span data-ttu-id="bc477-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc477-185">Here is a JSON representation of the resource.</span></span>
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





