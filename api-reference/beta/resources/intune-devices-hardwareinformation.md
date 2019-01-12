---
title: Тип ресурса hardwareInformation
description: Сведения об оборудовании данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0665152e3cc483f2303f458b79c891658651d91f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930315"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="387c6-103">Тип ресурса hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="387c6-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="387c6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="387c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="387c6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="387c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="387c6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="387c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="387c6-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="387c6-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="387c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="387c6-108">Properties</span></span>
|<span data-ttu-id="387c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="387c6-109">Property</span></span>|<span data-ttu-id="387c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="387c6-110">Type</span></span>|<span data-ttu-id="387c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="387c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="387c6-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="387c6-112">serialNumber</span></span>|<span data-ttu-id="387c6-113">String</span><span class="sxs-lookup"><span data-stu-id="387c6-113">String</span></span>|<span data-ttu-id="387c6-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="387c6-114">Serial number.</span></span>|
|<span data-ttu-id="387c6-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="387c6-115">totalStorageSpace</span></span>|<span data-ttu-id="387c6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="387c6-116">Int64</span></span>|<span data-ttu-id="387c6-117">Общий объем хранилища на диске устройства.</span><span class="sxs-lookup"><span data-stu-id="387c6-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="387c6-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="387c6-118">freeStorageSpace</span></span>|<span data-ttu-id="387c6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="387c6-119">Int64</span></span>|<span data-ttu-id="387c6-120">Свободное дисковое пространство устройства.</span><span class="sxs-lookup"><span data-stu-id="387c6-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="387c6-121">imei</span><span class="sxs-lookup"><span data-stu-id="387c6-121">imei</span></span>|<span data-ttu-id="387c6-122">String</span><span class="sxs-lookup"><span data-stu-id="387c6-122">String</span></span>|<span data-ttu-id="387c6-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="387c6-123">IMEI</span></span>|
|<span data-ttu-id="387c6-124">meid</span><span class="sxs-lookup"><span data-stu-id="387c6-124">meid</span></span>|<span data-ttu-id="387c6-125">String</span><span class="sxs-lookup"><span data-stu-id="387c6-125">String</span></span>|<span data-ttu-id="387c6-126">MEID</span><span class="sxs-lookup"><span data-stu-id="387c6-126">MEID</span></span>|
|<span data-ttu-id="387c6-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="387c6-127">manufacturer</span></span>|<span data-ttu-id="387c6-128">String</span><span class="sxs-lookup"><span data-stu-id="387c6-128">String</span></span>|<span data-ttu-id="387c6-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="387c6-130">model</span><span class="sxs-lookup"><span data-stu-id="387c6-130">model</span></span>|<span data-ttu-id="387c6-131">String</span><span class="sxs-lookup"><span data-stu-id="387c6-131">String</span></span>|<span data-ttu-id="387c6-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-132">Model of the device</span></span>|
|<span data-ttu-id="387c6-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="387c6-133">phoneNumber</span></span>|<span data-ttu-id="387c6-134">String</span><span class="sxs-lookup"><span data-stu-id="387c6-134">String</span></span>|<span data-ttu-id="387c6-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-135">Phone number of the device</span></span>|
|<span data-ttu-id="387c6-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="387c6-136">subscriberCarrier</span></span>|<span data-ttu-id="387c6-137">String</span><span class="sxs-lookup"><span data-stu-id="387c6-137">String</span></span>|<span data-ttu-id="387c6-138">Подписчик на поставщика устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="387c6-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="387c6-139">cellularTechnology</span></span>|<span data-ttu-id="387c6-140">String</span><span class="sxs-lookup"><span data-stu-id="387c6-140">String</span></span>|<span data-ttu-id="387c6-141">Сотовой связи технология устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="387c6-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="387c6-142">wifiMac</span></span>|<span data-ttu-id="387c6-143">String</span><span class="sxs-lookup"><span data-stu-id="387c6-143">String</span></span>|<span data-ttu-id="387c6-144">WiFi MAC-адрес устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="387c6-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="387c6-145">operatingSystemLanguage</span></span>|<span data-ttu-id="387c6-146">String</span><span class="sxs-lookup"><span data-stu-id="387c6-146">String</span></span>|<span data-ttu-id="387c6-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-147">Operating system language of the device</span></span>|
|<span data-ttu-id="387c6-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="387c6-148">isSupervised</span></span>|<span data-ttu-id="387c6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="387c6-149">Boolean</span></span>|<span data-ttu-id="387c6-150">Контролируемом режим устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="387c6-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="387c6-151">isEncrypted</span></span>|<span data-ttu-id="387c6-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="387c6-152">Boolean</span></span>|<span data-ttu-id="387c6-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="387c6-153">Encryption status of the device</span></span>|
|<span data-ttu-id="387c6-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="387c6-154">isSharedDevice</span></span>|<span data-ttu-id="387c6-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="387c6-155">Boolean</span></span>|<span data-ttu-id="387c6-156">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="387c6-156">Shared iPad</span></span>|
|<span data-ttu-id="387c6-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="387c6-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="387c6-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="387c6-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="387c6-159">Всем пользователям, включенным общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="387c6-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="387c6-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="387c6-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="387c6-161">String</span><span class="sxs-lookup"><span data-stu-id="387c6-161">String</span></span>|<span data-ttu-id="387c6-162">Строка, которая указывает версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="387c6-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="387c6-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="387c6-163">operatingSystemEdition</span></span>|<span data-ttu-id="387c6-164">String</span><span class="sxs-lookup"><span data-stu-id="387c6-164">String</span></span>|<span data-ttu-id="387c6-165">Строка, определяющая версии операционной системы.</span><span class="sxs-lookup"><span data-stu-id="387c6-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="387c6-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="387c6-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="387c6-167">String</span><span class="sxs-lookup"><span data-stu-id="387c6-167">String</span></span>|<span data-ttu-id="387c6-168">Возвращает полное доменное имя устройства (при его наличии).</span><span class="sxs-lookup"><span data-stu-id="387c6-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="387c6-169">Если устройство не присоединенный к домену, возвращает пустую строку.</span><span class="sxs-lookup"><span data-stu-id="387c6-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="387c6-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="387c6-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="387c6-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="387c6-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="387c6-172">Состояние требования безопасности на основе виртуализации оборудования.</span><span class="sxs-lookup"><span data-stu-id="387c6-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="387c6-173">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="387c6-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="387c6-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="387c6-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="387c6-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="387c6-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="387c6-176">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="387c6-176">Virtualization-based security status.</span></span> <span data-ttu-id="387c6-177">.</span><span class="sxs-lookup"><span data-stu-id="387c6-177"></span></span> <span data-ttu-id="387c6-178">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="387c6-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="387c6-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="387c6-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="387c6-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="387c6-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="387c6-181">Состояние защиты локальной системы Администратор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="387c6-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="387c6-182">.</span><span class="sxs-lookup"><span data-stu-id="387c6-182"></span></span> <span data-ttu-id="387c6-183">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="387c6-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="387c6-184">Связи</span><span class="sxs-lookup"><span data-stu-id="387c6-184">Relationships</span></span>
<span data-ttu-id="387c6-185">Нет</span><span class="sxs-lookup"><span data-stu-id="387c6-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="387c6-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="387c6-186">JSON Representation</span></span>
<span data-ttu-id="387c6-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="387c6-187">Here is a JSON representation of the resource.</span></span>
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





