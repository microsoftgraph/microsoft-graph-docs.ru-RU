---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40edcecb7c581722b7c423e4d76f181689a6020d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784035"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="8b066-103">Тип ресурса Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="8b066-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="8b066-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b066-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b066-106">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="8b066-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8b066-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b066-107">Properties</span></span>
|<span data-ttu-id="8b066-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b066-108">Property</span></span>|<span data-ttu-id="8b066-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b066-109">Type</span></span>|<span data-ttu-id="8b066-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b066-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b066-111">serialNumber</span><span class="sxs-lookup"><span data-stu-id="8b066-111">serialNumber</span></span>|<span data-ttu-id="8b066-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8b066-112">String</span></span>|<span data-ttu-id="8b066-113">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="8b066-113">Serial number.</span></span>|
|<span data-ttu-id="8b066-114">тоталсторажеспаце</span><span class="sxs-lookup"><span data-stu-id="8b066-114">totalStorageSpace</span></span>|<span data-ttu-id="8b066-115">Int64</span><span class="sxs-lookup"><span data-stu-id="8b066-115">Int64</span></span>|<span data-ttu-id="8b066-116">Общий объем хранилища устройства.</span><span class="sxs-lookup"><span data-stu-id="8b066-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="8b066-117">фристоражеспаце</span><span class="sxs-lookup"><span data-stu-id="8b066-117">freeStorageSpace</span></span>|<span data-ttu-id="8b066-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8b066-118">Int64</span></span>|<span data-ttu-id="8b066-119">Свободное место на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8b066-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="8b066-120">imei</span><span class="sxs-lookup"><span data-stu-id="8b066-120">imei</span></span>|<span data-ttu-id="8b066-121">String</span><span class="sxs-lookup"><span data-stu-id="8b066-121">String</span></span>|<span data-ttu-id="8b066-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="8b066-122">IMEI</span></span>|
|<span data-ttu-id="8b066-123">meid</span><span class="sxs-lookup"><span data-stu-id="8b066-123">meid</span></span>|<span data-ttu-id="8b066-124">String</span><span class="sxs-lookup"><span data-stu-id="8b066-124">String</span></span>|<span data-ttu-id="8b066-125">MEID</span><span class="sxs-lookup"><span data-stu-id="8b066-125">MEID</span></span>|
|<span data-ttu-id="8b066-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8b066-126">manufacturer</span></span>|<span data-ttu-id="8b066-127">String</span><span class="sxs-lookup"><span data-stu-id="8b066-127">String</span></span>|<span data-ttu-id="8b066-128">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="8b066-129">model</span><span class="sxs-lookup"><span data-stu-id="8b066-129">model</span></span>|<span data-ttu-id="8b066-130">String</span><span class="sxs-lookup"><span data-stu-id="8b066-130">String</span></span>|<span data-ttu-id="8b066-131">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-131">Model of the device</span></span>|
|<span data-ttu-id="8b066-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="8b066-132">phoneNumber</span></span>|<span data-ttu-id="8b066-133">String</span><span class="sxs-lookup"><span data-stu-id="8b066-133">String</span></span>|<span data-ttu-id="8b066-134">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-134">Phone number of the device</span></span>|
|<span data-ttu-id="8b066-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="8b066-135">subscriberCarrier</span></span>|<span data-ttu-id="8b066-136">String</span><span class="sxs-lookup"><span data-stu-id="8b066-136">String</span></span>|<span data-ttu-id="8b066-137">Абонентская перевозчик устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="8b066-138">целлулартечнологи</span><span class="sxs-lookup"><span data-stu-id="8b066-138">cellularTechnology</span></span>|<span data-ttu-id="8b066-139">String</span><span class="sxs-lookup"><span data-stu-id="8b066-139">String</span></span>|<span data-ttu-id="8b066-140">Технология сотовой связи устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="8b066-141">вифимак</span><span class="sxs-lookup"><span data-stu-id="8b066-141">wifiMac</span></span>|<span data-ttu-id="8b066-142">String</span><span class="sxs-lookup"><span data-stu-id="8b066-142">String</span></span>|<span data-ttu-id="8b066-143">MAC-адрес устройства Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="8b066-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="8b066-144">оператингсистемлангуаже</span><span class="sxs-lookup"><span data-stu-id="8b066-144">operatingSystemLanguage</span></span>|<span data-ttu-id="8b066-145">String</span><span class="sxs-lookup"><span data-stu-id="8b066-145">String</span></span>|<span data-ttu-id="8b066-146">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-146">Operating system language of the device</span></span>|
|<span data-ttu-id="8b066-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="8b066-147">isSupervised</span></span>|<span data-ttu-id="8b066-148">Логический</span><span class="sxs-lookup"><span data-stu-id="8b066-148">Boolean</span></span>|<span data-ttu-id="8b066-149">Контролируемый режим устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="8b066-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="8b066-150">isEncrypted</span></span>|<span data-ttu-id="8b066-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b066-151">Boolean</span></span>|<span data-ttu-id="8b066-152">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="8b066-152">Encryption status of the device</span></span>|
|<span data-ttu-id="8b066-153">Свойства isshareddevice</span><span class="sxs-lookup"><span data-stu-id="8b066-153">isSharedDevice</span></span>|<span data-ttu-id="8b066-154">Логический</span><span class="sxs-lookup"><span data-stu-id="8b066-154">Boolean</span></span>|<span data-ttu-id="8b066-155">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="8b066-155">Shared iPad</span></span>|
|<span data-ttu-id="8b066-156">шареддевицекачедусерс</span><span class="sxs-lookup"><span data-stu-id="8b066-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="8b066-157">Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="8b066-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="8b066-158">Все пользователи на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="8b066-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="8b066-159">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="8b066-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="8b066-160">String</span><span class="sxs-lookup"><span data-stu-id="8b066-160">String</span></span>|<span data-ttu-id="8b066-161">Строка, указывающая версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="8b066-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="8b066-162">оператингсистемедитион</span><span class="sxs-lookup"><span data-stu-id="8b066-162">operatingSystemEdition</span></span>|<span data-ttu-id="8b066-163">String</span><span class="sxs-lookup"><span data-stu-id="8b066-163">String</span></span>|<span data-ttu-id="8b066-164">Строка, задающая выпуск операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8b066-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="8b066-165">девицефуллкуалифиеддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="8b066-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="8b066-166">String</span><span class="sxs-lookup"><span data-stu-id="8b066-166">String</span></span>|<span data-ttu-id="8b066-167">Возвращает полное доменное имя устройства (при наличии).</span><span class="sxs-lookup"><span data-stu-id="8b066-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="8b066-168">Если устройство не присоединено к домену, возвращается пустая строка.</span><span class="sxs-lookup"><span data-stu-id="8b066-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="8b066-169">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="8b066-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="8b066-170">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="8b066-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="8b066-171">Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="8b066-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="8b066-172">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="8b066-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="8b066-173">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="8b066-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="8b066-174">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="8b066-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="8b066-175">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="8b066-175">Virtualization-based security status.</span></span> <span data-ttu-id="8b066-176">.</span><span class="sxs-lookup"><span data-stu-id="8b066-176">.</span></span> <span data-ttu-id="8b066-177">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="8b066-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="8b066-178">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="8b066-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="8b066-179">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="8b066-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="8b066-180">Состояние Credential Guard в администраторе локальной системы (LSA).</span><span class="sxs-lookup"><span data-stu-id="8b066-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="8b066-181">.</span><span class="sxs-lookup"><span data-stu-id="8b066-181">.</span></span> <span data-ttu-id="8b066-182">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="8b066-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="8b066-183">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="8b066-183">osBuildNumber</span></span>|<span data-ttu-id="8b066-184">String</span><span class="sxs-lookup"><span data-stu-id="8b066-184">String</span></span>|<span data-ttu-id="8b066-185">Номер сборки операционной системы на устройстве с Android</span><span class="sxs-lookup"><span data-stu-id="8b066-185">Operating System Build Number on Android device</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b066-186">Связи</span><span class="sxs-lookup"><span data-stu-id="8b066-186">Relationships</span></span>
<span data-ttu-id="8b066-187">Нет</span><span class="sxs-lookup"><span data-stu-id="8b066-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b066-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b066-188">JSON Representation</span></span>
<span data-ttu-id="8b066-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b066-189">Here is a JSON representation of the resource.</span></span>
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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String"
}
```



