---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2710d1085cca36f84331a1a89e1307e5475db427
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365190"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="623e3-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="623e3-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="623e3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="623e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="623e3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="623e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623e3-106">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="623e3-106">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="623e3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="623e3-107">Methods</span></span>
|<span data-ttu-id="623e3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="623e3-108">Method</span></span>|<span data-ttu-id="623e3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="623e3-109">Return Type</span></span>|<span data-ttu-id="623e3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="623e3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="623e3-111">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="623e3-111">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="623e3-112">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="623e3-112">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="623e3-113">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="623e3-113">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="623e3-114">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="623e3-114">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="623e3-115">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="623e3-115">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="623e3-116">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="623e3-116">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="623e3-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="623e3-117">Properties</span></span>
|<span data-ttu-id="623e3-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="623e3-118">Property</span></span>|<span data-ttu-id="623e3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="623e3-119">Type</span></span>|<span data-ttu-id="623e3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="623e3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623e3-121">id</span><span class="sxs-lookup"><span data-stu-id="623e3-121">id</span></span>|<span data-ttu-id="623e3-122">String</span><span class="sxs-lookup"><span data-stu-id="623e3-122">String</span></span>|<span data-ttu-id="623e3-123">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="623e3-123">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="623e3-124">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="623e3-124">This is device id of the device</span></span>|
|<span data-ttu-id="623e3-125">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="623e3-125">malwareProtectionEnabled</span></span>|<span data-ttu-id="623e3-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-126">Boolean</span></span>|<span data-ttu-id="623e3-127">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="623e3-127">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="623e3-128">девицестате</span><span class="sxs-lookup"><span data-stu-id="623e3-128">deviceState</span></span>|[<span data-ttu-id="623e3-129">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="623e3-129">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="623e3-130">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="623e3-130">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="623e3-131">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="623e3-131">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="623e3-132">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="623e3-132">realTimeProtectionEnabled</span></span>|<span data-ttu-id="623e3-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-133">Boolean</span></span>|<span data-ttu-id="623e3-134">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-134">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="623e3-135">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="623e3-135">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="623e3-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-136">Boolean</span></span>|<span data-ttu-id="623e3-137">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-137">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="623e3-138">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="623e3-138">quickScanOverdue</span></span>|<span data-ttu-id="623e3-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-139">Boolean</span></span>|<span data-ttu-id="623e3-140">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-140">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="623e3-141">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="623e3-141">fullScanOverdue</span></span>|<span data-ttu-id="623e3-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-142">Boolean</span></span>|<span data-ttu-id="623e3-143">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-143">Full scan overdue or not?</span></span>|
|<span data-ttu-id="623e3-144">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="623e3-144">signatureUpdateOverdue</span></span>|<span data-ttu-id="623e3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-145">Boolean</span></span>|<span data-ttu-id="623e3-146">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-146">Signature out of date or not?</span></span>|
|<span data-ttu-id="623e3-147">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="623e3-147">rebootRequired</span></span>|<span data-ttu-id="623e3-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-148">Boolean</span></span>|<span data-ttu-id="623e3-149">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-149">Reboot required or not?</span></span>|
|<span data-ttu-id="623e3-150">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="623e3-150">fullScanRequired</span></span>|<span data-ttu-id="623e3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="623e3-151">Boolean</span></span>|<span data-ttu-id="623e3-152">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="623e3-152">Full scan required or not?</span></span>|
|<span data-ttu-id="623e3-153">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="623e3-153">engineVersion</span></span>|<span data-ttu-id="623e3-154">String</span><span class="sxs-lookup"><span data-stu-id="623e3-154">String</span></span>|<span data-ttu-id="623e3-155">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="623e3-155">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="623e3-156">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="623e3-156">signatureVersion</span></span>|<span data-ttu-id="623e3-157">String</span><span class="sxs-lookup"><span data-stu-id="623e3-157">String</span></span>|<span data-ttu-id="623e3-158">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="623e3-158">Current malware definitions version</span></span>|
|<span data-ttu-id="623e3-159">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="623e3-159">antiMalwareVersion</span></span>|<span data-ttu-id="623e3-160">String</span><span class="sxs-lookup"><span data-stu-id="623e3-160">String</span></span>|<span data-ttu-id="623e3-161">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="623e3-161">Current anti malware version</span></span>|
|<span data-ttu-id="623e3-162">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="623e3-162">lastQuickScanDateTime</span></span>|<span data-ttu-id="623e3-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623e3-163">DateTimeOffset</span></span>|<span data-ttu-id="623e3-164">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="623e3-164">Last quick scan datetime</span></span>|
|<span data-ttu-id="623e3-165">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="623e3-165">lastFullScanDateTime</span></span>|<span data-ttu-id="623e3-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623e3-166">DateTimeOffset</span></span>|<span data-ttu-id="623e3-167">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="623e3-167">Last quick scan datetime</span></span>|
|<span data-ttu-id="623e3-168">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="623e3-168">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="623e3-169">String</span><span class="sxs-lookup"><span data-stu-id="623e3-169">String</span></span>|<span data-ttu-id="623e3-170">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="623e3-170">Last quick scan signature version</span></span>|
|<span data-ttu-id="623e3-171">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="623e3-171">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="623e3-172">String</span><span class="sxs-lookup"><span data-stu-id="623e3-172">String</span></span>|<span data-ttu-id="623e3-173">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="623e3-173">Last full scan signature version</span></span>|
|<span data-ttu-id="623e3-174">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="623e3-174">lastReportedDateTime</span></span>|<span data-ttu-id="623e3-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623e3-175">DateTimeOffset</span></span>|<span data-ttu-id="623e3-176">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="623e3-176">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="623e3-177">Отношения</span><span class="sxs-lookup"><span data-stu-id="623e3-177">Relationships</span></span>
|<span data-ttu-id="623e3-178">Отношение</span><span class="sxs-lookup"><span data-stu-id="623e3-178">Relationship</span></span>|<span data-ttu-id="623e3-179">Тип</span><span class="sxs-lookup"><span data-stu-id="623e3-179">Type</span></span>|<span data-ttu-id="623e3-180">Описание</span><span class="sxs-lookup"><span data-stu-id="623e3-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="623e3-181">детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="623e3-181">detectedMalwareState</span></span>|<span data-ttu-id="623e3-182">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="623e3-182">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="623e3-183">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="623e3-183">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="623e3-184">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="623e3-184">JSON Representation</span></span>
<span data-ttu-id="623e3-185">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="623e3-185">Here is a JSON representation of the resource.</span></span>
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



