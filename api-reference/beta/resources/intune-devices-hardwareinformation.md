---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2875ea3a4f8ba7bd00b2a1095ecaf496c36e5ef6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081393"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="536af-103">Тип ресурса Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="536af-103">hardwareInformation resource type</span></span>

<span data-ttu-id="536af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="536af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="536af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="536af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="536af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="536af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="536af-107">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="536af-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="536af-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="536af-108">Properties</span></span>
|<span data-ttu-id="536af-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="536af-109">Property</span></span>|<span data-ttu-id="536af-110">Тип</span><span class="sxs-lookup"><span data-stu-id="536af-110">Type</span></span>|<span data-ttu-id="536af-111">Описание</span><span class="sxs-lookup"><span data-stu-id="536af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="536af-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="536af-112">serialNumber</span></span>|<span data-ttu-id="536af-113">String</span><span class="sxs-lookup"><span data-stu-id="536af-113">String</span></span>|<span data-ttu-id="536af-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="536af-114">Serial number.</span></span>|
|<span data-ttu-id="536af-115">тоталсторажеспаце</span><span class="sxs-lookup"><span data-stu-id="536af-115">totalStorageSpace</span></span>|<span data-ttu-id="536af-116">Int64</span><span class="sxs-lookup"><span data-stu-id="536af-116">Int64</span></span>|<span data-ttu-id="536af-117">Общий объем хранилища устройства.</span><span class="sxs-lookup"><span data-stu-id="536af-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="536af-118">фристоражеспаце</span><span class="sxs-lookup"><span data-stu-id="536af-118">freeStorageSpace</span></span>|<span data-ttu-id="536af-119">Int64</span><span class="sxs-lookup"><span data-stu-id="536af-119">Int64</span></span>|<span data-ttu-id="536af-120">Свободное место на устройстве.</span><span class="sxs-lookup"><span data-stu-id="536af-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="536af-121">imei</span><span class="sxs-lookup"><span data-stu-id="536af-121">imei</span></span>|<span data-ttu-id="536af-122">String</span><span class="sxs-lookup"><span data-stu-id="536af-122">String</span></span>|<span data-ttu-id="536af-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="536af-123">IMEI</span></span>|
|<span data-ttu-id="536af-124">meid</span><span class="sxs-lookup"><span data-stu-id="536af-124">meid</span></span>|<span data-ttu-id="536af-125">String</span><span class="sxs-lookup"><span data-stu-id="536af-125">String</span></span>|<span data-ttu-id="536af-126">MEID</span><span class="sxs-lookup"><span data-stu-id="536af-126">MEID</span></span>|
|<span data-ttu-id="536af-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="536af-127">manufacturer</span></span>|<span data-ttu-id="536af-128">String</span><span class="sxs-lookup"><span data-stu-id="536af-128">String</span></span>|<span data-ttu-id="536af-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="536af-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="536af-130">model</span><span class="sxs-lookup"><span data-stu-id="536af-130">model</span></span>|<span data-ttu-id="536af-131">String</span><span class="sxs-lookup"><span data-stu-id="536af-131">String</span></span>|<span data-ttu-id="536af-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="536af-132">Model of the device</span></span>|
|<span data-ttu-id="536af-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="536af-133">phoneNumber</span></span>|<span data-ttu-id="536af-134">String</span><span class="sxs-lookup"><span data-stu-id="536af-134">String</span></span>|<span data-ttu-id="536af-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="536af-135">Phone number of the device</span></span>|
|<span data-ttu-id="536af-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="536af-136">subscriberCarrier</span></span>|<span data-ttu-id="536af-137">String</span><span class="sxs-lookup"><span data-stu-id="536af-137">String</span></span>|<span data-ttu-id="536af-138">Абонентская перевозчик устройства</span><span class="sxs-lookup"><span data-stu-id="536af-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="536af-139">целлулартечнологи</span><span class="sxs-lookup"><span data-stu-id="536af-139">cellularTechnology</span></span>|<span data-ttu-id="536af-140">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-140">String</span></span>|<span data-ttu-id="536af-141">Технология сотовой связи устройства</span><span class="sxs-lookup"><span data-stu-id="536af-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="536af-142">вифимак</span><span class="sxs-lookup"><span data-stu-id="536af-142">wifiMac</span></span>|<span data-ttu-id="536af-143">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-143">String</span></span>|<span data-ttu-id="536af-144">MAC-адрес устройства Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="536af-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="536af-145">оператингсистемлангуаже</span><span class="sxs-lookup"><span data-stu-id="536af-145">operatingSystemLanguage</span></span>|<span data-ttu-id="536af-146">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-146">String</span></span>|<span data-ttu-id="536af-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="536af-147">Operating system language of the device</span></span>|
|<span data-ttu-id="536af-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="536af-148">isSupervised</span></span>|<span data-ttu-id="536af-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="536af-149">Boolean</span></span>|<span data-ttu-id="536af-150">Контролируемый режим устройства</span><span class="sxs-lookup"><span data-stu-id="536af-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="536af-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="536af-151">isEncrypted</span></span>|<span data-ttu-id="536af-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="536af-152">Boolean</span></span>|<span data-ttu-id="536af-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="536af-153">Encryption status of the device</span></span>|
|<span data-ttu-id="536af-154">баттерисериалнумбер</span><span class="sxs-lookup"><span data-stu-id="536af-154">batterySerialNumber</span></span>|<span data-ttu-id="536af-155">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-155">String</span></span>|<span data-ttu-id="536af-156">Серийный номер текущей батареи устройства</span><span class="sxs-lookup"><span data-stu-id="536af-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="536af-157">баттерихеалсперцентаже</span><span class="sxs-lookup"><span data-stu-id="536af-157">batteryHealthPercentage</span></span>|<span data-ttu-id="536af-158">Int32</span><span class="sxs-lookup"><span data-stu-id="536af-158">Int32</span></span>|<span data-ttu-id="536af-159">Процент работоспособности текущего аккумулятора устройства.</span><span class="sxs-lookup"><span data-stu-id="536af-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="536af-160">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="536af-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="536af-161">баттеричаржециклес</span><span class="sxs-lookup"><span data-stu-id="536af-161">batteryChargeCycles</span></span>|<span data-ttu-id="536af-162">Int32</span><span class="sxs-lookup"><span data-stu-id="536af-162">Int32</span></span>|<span data-ttu-id="536af-163">Количество циклов зарядки, прошедшей через текущий аккумулятор устройства.</span><span class="sxs-lookup"><span data-stu-id="536af-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="536af-164">Допустимые значения — от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="536af-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="536af-165">Свойства isshareddevice</span><span class="sxs-lookup"><span data-stu-id="536af-165">isSharedDevice</span></span>|<span data-ttu-id="536af-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="536af-166">Boolean</span></span>|<span data-ttu-id="536af-167">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="536af-167">Shared iPad</span></span>|
|<span data-ttu-id="536af-168">шареддевицекачедусерс</span><span class="sxs-lookup"><span data-stu-id="536af-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="536af-169">Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="536af-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="536af-170">Все пользователи на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="536af-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="536af-171">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="536af-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="536af-172">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-172">String</span></span>|<span data-ttu-id="536af-173">Строка, указывающая версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="536af-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="536af-174">оператингсистемедитион</span><span class="sxs-lookup"><span data-stu-id="536af-174">operatingSystemEdition</span></span>|<span data-ttu-id="536af-175">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-175">String</span></span>|<span data-ttu-id="536af-176">Строка, задающая выпуск операционной системы.</span><span class="sxs-lookup"><span data-stu-id="536af-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="536af-177">девицефуллкуалифиеддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="536af-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="536af-178">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-178">String</span></span>|<span data-ttu-id="536af-179">Возвращает полное доменное имя устройства (при наличии).</span><span class="sxs-lookup"><span data-stu-id="536af-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="536af-180">Если устройство не присоединено к домену, возвращается пустая строка.</span><span class="sxs-lookup"><span data-stu-id="536af-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="536af-181">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="536af-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="536af-182">девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="536af-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="536af-183">Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="536af-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="536af-184">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="536af-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="536af-185">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="536af-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="536af-186">девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="536af-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="536af-187">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="536af-187">Virtualization-based security status.</span></span> <span data-ttu-id="536af-188">.</span><span class="sxs-lookup"><span data-stu-id="536af-188">.</span></span> <span data-ttu-id="536af-189">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="536af-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="536af-190">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="536af-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="536af-191">девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="536af-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="536af-192">Состояние Credential Guard в администраторе локальной системы (LSA).</span><span class="sxs-lookup"><span data-stu-id="536af-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="536af-193">.</span><span class="sxs-lookup"><span data-stu-id="536af-193">.</span></span> <span data-ttu-id="536af-194">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="536af-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="536af-195">осбуилднумбер</span><span class="sxs-lookup"><span data-stu-id="536af-195">osBuildNumber</span></span>|<span data-ttu-id="536af-196">Строка</span><span class="sxs-lookup"><span data-stu-id="536af-196">String</span></span>|<span data-ttu-id="536af-197">Номер сборки операционной системы на устройстве с Android</span><span class="sxs-lookup"><span data-stu-id="536af-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="536af-198">оператингсистемпродукттипе</span><span class="sxs-lookup"><span data-stu-id="536af-198">operatingSystemProductType</span></span>|<span data-ttu-id="536af-199">Int32</span><span class="sxs-lookup"><span data-stu-id="536af-199">Int32</span></span>|<span data-ttu-id="536af-200">Int, указывающий операционную систему Windows Продукттипе.</span><span class="sxs-lookup"><span data-stu-id="536af-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="536af-201">Дополнительные сведения https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="536af-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="536af-202">Допустимые значения — от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="536af-202">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="536af-203">Связи</span><span class="sxs-lookup"><span data-stu-id="536af-203">Relationships</span></span>
<span data-ttu-id="536af-204">Нет</span><span class="sxs-lookup"><span data-stu-id="536af-204">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="536af-205">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="536af-205">JSON Representation</span></span>
<span data-ttu-id="536af-206">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="536af-206">Here is a JSON representation of the resource.</span></span>
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
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
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
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024
}
```






