---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15369ff988d13e7d083358dceb874da2a0ffa6a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470644"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="85e56-103">Тип ресурса Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="85e56-103">hardwareInformation resource type</span></span>

<span data-ttu-id="85e56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85e56-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85e56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85e56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e56-107">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="85e56-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="85e56-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85e56-108">Properties</span></span>
|<span data-ttu-id="85e56-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85e56-109">Property</span></span>|<span data-ttu-id="85e56-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85e56-110">Type</span></span>|<span data-ttu-id="85e56-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85e56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e56-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="85e56-112">serialNumber</span></span>|<span data-ttu-id="85e56-113">Строка</span><span class="sxs-lookup"><span data-stu-id="85e56-113">String</span></span>|<span data-ttu-id="85e56-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="85e56-114">Serial number.</span></span>|
|<span data-ttu-id="85e56-115">тоталсторажеспаце</span><span class="sxs-lookup"><span data-stu-id="85e56-115">totalStorageSpace</span></span>|<span data-ttu-id="85e56-116">Int64</span><span class="sxs-lookup"><span data-stu-id="85e56-116">Int64</span></span>|<span data-ttu-id="85e56-117">Общий объем хранилища устройства.</span><span class="sxs-lookup"><span data-stu-id="85e56-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="85e56-118">фристоражеспаце</span><span class="sxs-lookup"><span data-stu-id="85e56-118">freeStorageSpace</span></span>|<span data-ttu-id="85e56-119">Int64</span><span class="sxs-lookup"><span data-stu-id="85e56-119">Int64</span></span>|<span data-ttu-id="85e56-120">Свободное место на устройстве.</span><span class="sxs-lookup"><span data-stu-id="85e56-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="85e56-121">imei</span><span class="sxs-lookup"><span data-stu-id="85e56-121">imei</span></span>|<span data-ttu-id="85e56-122">String</span><span class="sxs-lookup"><span data-stu-id="85e56-122">String</span></span>|<span data-ttu-id="85e56-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="85e56-123">IMEI</span></span>|
|<span data-ttu-id="85e56-124">meid</span><span class="sxs-lookup"><span data-stu-id="85e56-124">meid</span></span>|<span data-ttu-id="85e56-125">String</span><span class="sxs-lookup"><span data-stu-id="85e56-125">String</span></span>|<span data-ttu-id="85e56-126">MEID</span><span class="sxs-lookup"><span data-stu-id="85e56-126">MEID</span></span>|
|<span data-ttu-id="85e56-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="85e56-127">manufacturer</span></span>|<span data-ttu-id="85e56-128">String</span><span class="sxs-lookup"><span data-stu-id="85e56-128">String</span></span>|<span data-ttu-id="85e56-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="85e56-130">model</span><span class="sxs-lookup"><span data-stu-id="85e56-130">model</span></span>|<span data-ttu-id="85e56-131">String</span><span class="sxs-lookup"><span data-stu-id="85e56-131">String</span></span>|<span data-ttu-id="85e56-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-132">Model of the device</span></span>|
|<span data-ttu-id="85e56-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="85e56-133">phoneNumber</span></span>|<span data-ttu-id="85e56-134">String</span><span class="sxs-lookup"><span data-stu-id="85e56-134">String</span></span>|<span data-ttu-id="85e56-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-135">Phone number of the device</span></span>|
|<span data-ttu-id="85e56-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="85e56-136">subscriberCarrier</span></span>|<span data-ttu-id="85e56-137">String</span><span class="sxs-lookup"><span data-stu-id="85e56-137">String</span></span>|<span data-ttu-id="85e56-138">Абонентская перевозчик устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="85e56-139">целлулартечнологи</span><span class="sxs-lookup"><span data-stu-id="85e56-139">cellularTechnology</span></span>|<span data-ttu-id="85e56-140">String</span><span class="sxs-lookup"><span data-stu-id="85e56-140">String</span></span>|<span data-ttu-id="85e56-141">Технология сотовой связи устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="85e56-142">вифимак</span><span class="sxs-lookup"><span data-stu-id="85e56-142">wifiMac</span></span>|<span data-ttu-id="85e56-143">String</span><span class="sxs-lookup"><span data-stu-id="85e56-143">String</span></span>|<span data-ttu-id="85e56-144">MAC-адрес устройства Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="85e56-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="85e56-145">оператингсистемлангуаже</span><span class="sxs-lookup"><span data-stu-id="85e56-145">operatingSystemLanguage</span></span>|<span data-ttu-id="85e56-146">String</span><span class="sxs-lookup"><span data-stu-id="85e56-146">String</span></span>|<span data-ttu-id="85e56-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-147">Operating system language of the device</span></span>|
|<span data-ttu-id="85e56-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="85e56-148">isSupervised</span></span>|<span data-ttu-id="85e56-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e56-149">Boolean</span></span>|<span data-ttu-id="85e56-150">Контролируемый режим устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="85e56-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="85e56-151">isEncrypted</span></span>|<span data-ttu-id="85e56-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e56-152">Boolean</span></span>|<span data-ttu-id="85e56-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="85e56-153">Encryption status of the device</span></span>|
|<span data-ttu-id="85e56-154">Свойства isshareddevice</span><span class="sxs-lookup"><span data-stu-id="85e56-154">isSharedDevice</span></span>|<span data-ttu-id="85e56-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e56-155">Boolean</span></span>|<span data-ttu-id="85e56-156">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="85e56-156">Shared iPad</span></span>|
|<span data-ttu-id="85e56-157">шареддевицекачедусерс</span><span class="sxs-lookup"><span data-stu-id="85e56-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="85e56-158">Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="85e56-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="85e56-159">Все пользователи на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="85e56-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="85e56-160">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="85e56-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="85e56-161">String</span><span class="sxs-lookup"><span data-stu-id="85e56-161">String</span></span>|<span data-ttu-id="85e56-162">Строка, указывающая версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="85e56-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="85e56-163">оператингсистемедитион</span><span class="sxs-lookup"><span data-stu-id="85e56-163">operatingSystemEdition</span></span>|<span data-ttu-id="85e56-164">String</span><span class="sxs-lookup"><span data-stu-id="85e56-164">String</span></span>|<span data-ttu-id="85e56-165">Строка, задающая выпуск операционной системы.</span><span class="sxs-lookup"><span data-stu-id="85e56-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="85e56-166">девицефуллкуалифиеддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="85e56-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="85e56-167">String</span><span class="sxs-lookup"><span data-stu-id="85e56-167">String</span></span>|<span data-ttu-id="85e56-168">Возвращает полное доменное имя устройства (при наличии).</span><span class="sxs-lookup"><span data-stu-id="85e56-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="85e56-169">Если устройство не присоединено к домену, возвращается пустая строка.</span><span class="sxs-lookup"><span data-stu-id="85e56-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="85e56-170">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="85e56-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="85e56-171">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="85e56-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="85e56-172">Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="85e56-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="85e56-173">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="85e56-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="85e56-174">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="85e56-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="85e56-175">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="85e56-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="85e56-176">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="85e56-176">Virtualization-based security status.</span></span> <span data-ttu-id="85e56-177">.</span><span class="sxs-lookup"><span data-stu-id="85e56-177">.</span></span> <span data-ttu-id="85e56-178">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="85e56-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="85e56-179">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="85e56-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="85e56-180">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="85e56-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="85e56-181">Состояние Credential Guard в администраторе локальной системы (LSA).</span><span class="sxs-lookup"><span data-stu-id="85e56-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="85e56-182">.</span><span class="sxs-lookup"><span data-stu-id="85e56-182">.</span></span> <span data-ttu-id="85e56-183">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="85e56-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="85e56-184">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="85e56-184">osBuildNumber</span></span>|<span data-ttu-id="85e56-185">String</span><span class="sxs-lookup"><span data-stu-id="85e56-185">String</span></span>|<span data-ttu-id="85e56-186">Номер сборки операционной системы на устройстве с Android</span><span class="sxs-lookup"><span data-stu-id="85e56-186">Operating System Build Number on Android device</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e56-187">Отношения</span><span class="sxs-lookup"><span data-stu-id="85e56-187">Relationships</span></span>
<span data-ttu-id="85e56-188">Нет</span><span class="sxs-lookup"><span data-stu-id="85e56-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e56-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85e56-189">JSON Representation</span></span>
<span data-ttu-id="85e56-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85e56-190">Here is a JSON representation of the resource.</span></span>
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



