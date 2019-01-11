---
title: Тип ресурса hardwareInformation
description: Сведения об оборудовании данного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2684f1ff7e7a6407942ac61fae7d45ead16820d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831826"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="f68d3-103">Тип ресурса hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="f68d3-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="f68d3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f68d3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f68d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f68d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f68d3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f68d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f68d3-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="f68d3-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f68d3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f68d3-108">Properties</span></span>
|<span data-ttu-id="f68d3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f68d3-109">Property</span></span>|<span data-ttu-id="f68d3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f68d3-110">Type</span></span>|<span data-ttu-id="f68d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f68d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f68d3-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="f68d3-112">serialNumber</span></span>|<span data-ttu-id="f68d3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-113">String</span></span>|<span data-ttu-id="f68d3-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="f68d3-114">Serial number.</span></span>|
|<span data-ttu-id="f68d3-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="f68d3-115">totalStorageSpace</span></span>|<span data-ttu-id="f68d3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f68d3-116">Int64</span></span>|<span data-ttu-id="f68d3-117">Общий объем хранилища на диске устройства.</span><span class="sxs-lookup"><span data-stu-id="f68d3-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="f68d3-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="f68d3-118">freeStorageSpace</span></span>|<span data-ttu-id="f68d3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f68d3-119">Int64</span></span>|<span data-ttu-id="f68d3-120">Свободное дисковое пространство устройства.</span><span class="sxs-lookup"><span data-stu-id="f68d3-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="f68d3-121">imei</span><span class="sxs-lookup"><span data-stu-id="f68d3-121">imei</span></span>|<span data-ttu-id="f68d3-122">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-122">String</span></span>|<span data-ttu-id="f68d3-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="f68d3-123">IMEI</span></span>|
|<span data-ttu-id="f68d3-124">meid</span><span class="sxs-lookup"><span data-stu-id="f68d3-124">meid</span></span>|<span data-ttu-id="f68d3-125">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-125">String</span></span>|<span data-ttu-id="f68d3-126">MEID</span><span class="sxs-lookup"><span data-stu-id="f68d3-126">MEID</span></span>|
|<span data-ttu-id="f68d3-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f68d3-127">manufacturer</span></span>|<span data-ttu-id="f68d3-128">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-128">String</span></span>|<span data-ttu-id="f68d3-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="f68d3-130">model</span><span class="sxs-lookup"><span data-stu-id="f68d3-130">model</span></span>|<span data-ttu-id="f68d3-131">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-131">String</span></span>|<span data-ttu-id="f68d3-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-132">Model of the device</span></span>|
|<span data-ttu-id="f68d3-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="f68d3-133">phoneNumber</span></span>|<span data-ttu-id="f68d3-134">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-134">String</span></span>|<span data-ttu-id="f68d3-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-135">Phone number of the device</span></span>|
|<span data-ttu-id="f68d3-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="f68d3-136">subscriberCarrier</span></span>|<span data-ttu-id="f68d3-137">String</span><span class="sxs-lookup"><span data-stu-id="f68d3-137">String</span></span>|<span data-ttu-id="f68d3-138">Подписчик на поставщика устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="f68d3-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="f68d3-139">cellularTechnology</span></span>|<span data-ttu-id="f68d3-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-140">String</span></span>|<span data-ttu-id="f68d3-141">Сотовой связи технология устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="f68d3-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="f68d3-142">wifiMac</span></span>|<span data-ttu-id="f68d3-143">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-143">String</span></span>|<span data-ttu-id="f68d3-144">WiFi MAC-адрес устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="f68d3-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="f68d3-145">operatingSystemLanguage</span></span>|<span data-ttu-id="f68d3-146">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-146">String</span></span>|<span data-ttu-id="f68d3-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-147">Operating system language of the device</span></span>|
|<span data-ttu-id="f68d3-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="f68d3-148">isSupervised</span></span>|<span data-ttu-id="f68d3-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f68d3-149">Boolean</span></span>|<span data-ttu-id="f68d3-150">Контролируемом режим устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="f68d3-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f68d3-151">isEncrypted</span></span>|<span data-ttu-id="f68d3-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f68d3-152">Boolean</span></span>|<span data-ttu-id="f68d3-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="f68d3-153">Encryption status of the device</span></span>|
|<span data-ttu-id="f68d3-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="f68d3-154">isSharedDevice</span></span>|<span data-ttu-id="f68d3-155">Логический</span><span class="sxs-lookup"><span data-stu-id="f68d3-155">Boolean</span></span>|<span data-ttu-id="f68d3-156">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="f68d3-156">Shared iPad</span></span>|
|<span data-ttu-id="f68d3-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="f68d3-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="f68d3-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f68d3-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="f68d3-159">Всем пользователям, включенным общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="f68d3-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="f68d3-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="f68d3-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="f68d3-161">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-161">String</span></span>|<span data-ttu-id="f68d3-162">Строка, которая указывает версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="f68d3-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="f68d3-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="f68d3-163">operatingSystemEdition</span></span>|<span data-ttu-id="f68d3-164">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-164">String</span></span>|<span data-ttu-id="f68d3-165">Строка, определяющая версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f68d3-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="f68d3-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="f68d3-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="f68d3-167">Строка</span><span class="sxs-lookup"><span data-stu-id="f68d3-167">String</span></span>|<span data-ttu-id="f68d3-168">Возвращает полное доменное имя устройства (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="f68d3-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="f68d3-169">Если устройство не присоединенный к домену, возвращает пустую строку.</span><span class="sxs-lookup"><span data-stu-id="f68d3-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="f68d3-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="f68d3-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="f68d3-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="f68d3-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="f68d3-172">Состояние требования безопасности на основе виртуализации оборудования.</span><span class="sxs-lookup"><span data-stu-id="f68d3-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="f68d3-173">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="f68d3-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="f68d3-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="f68d3-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="f68d3-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="f68d3-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="f68d3-176">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="f68d3-176">Virtualization-based security status.</span></span> <span data-ttu-id="f68d3-177">.</span><span class="sxs-lookup"><span data-stu-id="f68d3-177"></span></span> <span data-ttu-id="f68d3-178">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="f68d3-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="f68d3-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="f68d3-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="f68d3-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="f68d3-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="f68d3-181">Состояние защиты локальной системы Администратор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f68d3-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="f68d3-182">.</span><span class="sxs-lookup"><span data-stu-id="f68d3-182"></span></span> <span data-ttu-id="f68d3-183">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="f68d3-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f68d3-184">Связи</span><span class="sxs-lookup"><span data-stu-id="f68d3-184">Relationships</span></span>
<span data-ttu-id="f68d3-185">Нет</span><span class="sxs-lookup"><span data-stu-id="f68d3-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f68d3-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f68d3-186">JSON Representation</span></span>
<span data-ttu-id="f68d3-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f68d3-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





