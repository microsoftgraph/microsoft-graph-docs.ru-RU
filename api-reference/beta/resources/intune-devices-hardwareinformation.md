---
title: Тип ресурса hardwareInformation
description: Сведения об оборудовании данного устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394826"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="fc4ff-103">Тип ресурса hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="fc4ff-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="fc4ff-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc4ff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc4ff-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc4ff-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="fc4ff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-108">Properties</span></span>
|<span data-ttu-id="fc4ff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc4ff-109">Property</span></span>|<span data-ttu-id="fc4ff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc4ff-110">Type</span></span>|<span data-ttu-id="fc4ff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc4ff-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="fc4ff-112">serialNumber</span></span>|<span data-ttu-id="fc4ff-113">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-113">String</span></span>|<span data-ttu-id="fc4ff-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-114">Serial number.</span></span>|
|<span data-ttu-id="fc4ff-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="fc4ff-115">totalStorageSpace</span></span>|<span data-ttu-id="fc4ff-116">Int64</span><span class="sxs-lookup"><span data-stu-id="fc4ff-116">Int64</span></span>|<span data-ttu-id="fc4ff-117">Общий объем хранилища на диске устройства.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="fc4ff-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="fc4ff-118">freeStorageSpace</span></span>|<span data-ttu-id="fc4ff-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fc4ff-119">Int64</span></span>|<span data-ttu-id="fc4ff-120">Свободное дисковое пространство устройства.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="fc4ff-121">imei</span><span class="sxs-lookup"><span data-stu-id="fc4ff-121">imei</span></span>|<span data-ttu-id="fc4ff-122">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-122">String</span></span>|<span data-ttu-id="fc4ff-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="fc4ff-123">IMEI</span></span>|
|<span data-ttu-id="fc4ff-124">meid</span><span class="sxs-lookup"><span data-stu-id="fc4ff-124">meid</span></span>|<span data-ttu-id="fc4ff-125">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-125">String</span></span>|<span data-ttu-id="fc4ff-126">MEID</span><span class="sxs-lookup"><span data-stu-id="fc4ff-126">MEID</span></span>|
|<span data-ttu-id="fc4ff-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="fc4ff-127">manufacturer</span></span>|<span data-ttu-id="fc4ff-128">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-128">String</span></span>|<span data-ttu-id="fc4ff-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="fc4ff-130">model</span><span class="sxs-lookup"><span data-stu-id="fc4ff-130">model</span></span>|<span data-ttu-id="fc4ff-131">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-131">String</span></span>|<span data-ttu-id="fc4ff-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-132">Model of the device</span></span>|
|<span data-ttu-id="fc4ff-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="fc4ff-133">phoneNumber</span></span>|<span data-ttu-id="fc4ff-134">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-134">String</span></span>|<span data-ttu-id="fc4ff-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-135">Phone number of the device</span></span>|
|<span data-ttu-id="fc4ff-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="fc4ff-136">subscriberCarrier</span></span>|<span data-ttu-id="fc4ff-137">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-137">String</span></span>|<span data-ttu-id="fc4ff-138">Подписчик на поставщика устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="fc4ff-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="fc4ff-139">cellularTechnology</span></span>|<span data-ttu-id="fc4ff-140">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-140">String</span></span>|<span data-ttu-id="fc4ff-141">Сотовой связи технология устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="fc4ff-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="fc4ff-142">wifiMac</span></span>|<span data-ttu-id="fc4ff-143">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-143">String</span></span>|<span data-ttu-id="fc4ff-144">WiFi MAC-адрес устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="fc4ff-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="fc4ff-145">operatingSystemLanguage</span></span>|<span data-ttu-id="fc4ff-146">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-146">String</span></span>|<span data-ttu-id="fc4ff-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-147">Operating system language of the device</span></span>|
|<span data-ttu-id="fc4ff-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="fc4ff-148">isSupervised</span></span>|<span data-ttu-id="fc4ff-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc4ff-149">Boolean</span></span>|<span data-ttu-id="fc4ff-150">Контролируемом режим устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="fc4ff-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="fc4ff-151">isEncrypted</span></span>|<span data-ttu-id="fc4ff-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc4ff-152">Boolean</span></span>|<span data-ttu-id="fc4ff-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="fc4ff-153">Encryption status of the device</span></span>|
|<span data-ttu-id="fc4ff-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="fc4ff-154">isSharedDevice</span></span>|<span data-ttu-id="fc4ff-155">Логический</span><span class="sxs-lookup"><span data-stu-id="fc4ff-155">Boolean</span></span>|<span data-ttu-id="fc4ff-156">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="fc4ff-156">Shared iPad</span></span>|
|<span data-ttu-id="fc4ff-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="fc4ff-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="fc4ff-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fc4ff-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="fc4ff-159">Всем пользователям, включенным общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="fc4ff-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="fc4ff-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="fc4ff-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="fc4ff-161">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-161">String</span></span>|<span data-ttu-id="fc4ff-162">Строка, которая указывает версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="fc4ff-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="fc4ff-163">operatingSystemEdition</span></span>|<span data-ttu-id="fc4ff-164">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-164">String</span></span>|<span data-ttu-id="fc4ff-165">Строка, определяющая версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="fc4ff-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="fc4ff-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="fc4ff-167">String</span><span class="sxs-lookup"><span data-stu-id="fc4ff-167">String</span></span>|<span data-ttu-id="fc4ff-168">Возвращает полное доменное имя устройства (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="fc4ff-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="fc4ff-169">Если устройство не присоединенный к домену, возвращает пустую строку.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="fc4ff-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="fc4ff-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="fc4ff-172">Состояние требования безопасности на основе виртуализации оборудования.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="fc4ff-173">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="fc4ff-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="fc4ff-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="fc4ff-176">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-176">Virtualization-based security status.</span></span> <span data-ttu-id="fc4ff-177">.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-177"></span></span> <span data-ttu-id="fc4ff-178">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="fc4ff-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="fc4ff-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="fc4ff-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="fc4ff-181">Состояние защиты локальной системы Администратор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="fc4ff-182">.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-182"></span></span> <span data-ttu-id="fc4ff-183">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc4ff-184">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc4ff-184">Relationships</span></span>
<span data-ttu-id="fc4ff-185">Нет</span><span class="sxs-lookup"><span data-stu-id="fc4ff-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc4ff-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc4ff-186">JSON Representation</span></span>
<span data-ttu-id="fc4ff-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc4ff-187">Here is a JSON representation of the resource.</span></span>
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




