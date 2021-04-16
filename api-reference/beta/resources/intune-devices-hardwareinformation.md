---
title: Тип ресурса hardwareInformation
description: Сведения о оборудовании данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e17df5baad3df0237218f314cdb1c5ee99f03c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868178"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="30d83-103">Тип ресурса hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="30d83-103">hardwareInformation resource type</span></span>

<span data-ttu-id="30d83-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30d83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30d83-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30d83-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30d83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d83-107">Сведения о оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="30d83-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="30d83-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="30d83-108">Properties</span></span>
|<span data-ttu-id="30d83-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="30d83-109">Property</span></span>|<span data-ttu-id="30d83-110">Тип</span><span class="sxs-lookup"><span data-stu-id="30d83-110">Type</span></span>|<span data-ttu-id="30d83-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30d83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d83-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="30d83-112">serialNumber</span></span>|<span data-ttu-id="30d83-113">String</span><span class="sxs-lookup"><span data-stu-id="30d83-113">String</span></span>|<span data-ttu-id="30d83-114">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="30d83-114">Serial number.</span></span>|
|<span data-ttu-id="30d83-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="30d83-115">totalStorageSpace</span></span>|<span data-ttu-id="30d83-116">Int64</span><span class="sxs-lookup"><span data-stu-id="30d83-116">Int64</span></span>|<span data-ttu-id="30d83-117">Общее пространство хранилища устройства.</span><span class="sxs-lookup"><span data-stu-id="30d83-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="30d83-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="30d83-118">freeStorageSpace</span></span>|<span data-ttu-id="30d83-119">Int64</span><span class="sxs-lookup"><span data-stu-id="30d83-119">Int64</span></span>|<span data-ttu-id="30d83-120">Свободное пространство для хранения устройства.</span><span class="sxs-lookup"><span data-stu-id="30d83-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="30d83-121">imei</span><span class="sxs-lookup"><span data-stu-id="30d83-121">imei</span></span>|<span data-ttu-id="30d83-122">String</span><span class="sxs-lookup"><span data-stu-id="30d83-122">String</span></span>|<span data-ttu-id="30d83-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="30d83-123">IMEI</span></span>|
|<span data-ttu-id="30d83-124">meid</span><span class="sxs-lookup"><span data-stu-id="30d83-124">meid</span></span>|<span data-ttu-id="30d83-125">String</span><span class="sxs-lookup"><span data-stu-id="30d83-125">String</span></span>|<span data-ttu-id="30d83-126">MEID</span><span class="sxs-lookup"><span data-stu-id="30d83-126">MEID</span></span>|
|<span data-ttu-id="30d83-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="30d83-127">manufacturer</span></span>|<span data-ttu-id="30d83-128">String</span><span class="sxs-lookup"><span data-stu-id="30d83-128">String</span></span>|<span data-ttu-id="30d83-129">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="30d83-130">model</span><span class="sxs-lookup"><span data-stu-id="30d83-130">model</span></span>|<span data-ttu-id="30d83-131">String</span><span class="sxs-lookup"><span data-stu-id="30d83-131">String</span></span>|<span data-ttu-id="30d83-132">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-132">Model of the device</span></span>|
|<span data-ttu-id="30d83-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="30d83-133">phoneNumber</span></span>|<span data-ttu-id="30d83-134">String</span><span class="sxs-lookup"><span data-stu-id="30d83-134">String</span></span>|<span data-ttu-id="30d83-135">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-135">Phone number of the device</span></span>|
|<span data-ttu-id="30d83-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="30d83-136">subscriberCarrier</span></span>|<span data-ttu-id="30d83-137">String</span><span class="sxs-lookup"><span data-stu-id="30d83-137">String</span></span>|<span data-ttu-id="30d83-138">Оператор абонента устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="30d83-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="30d83-139">cellularTechnology</span></span>|<span data-ttu-id="30d83-140">String</span><span class="sxs-lookup"><span data-stu-id="30d83-140">String</span></span>|<span data-ttu-id="30d83-141">Клеточная технология устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="30d83-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="30d83-142">wifiMac</span></span>|<span data-ttu-id="30d83-143">String</span><span class="sxs-lookup"><span data-stu-id="30d83-143">String</span></span>|<span data-ttu-id="30d83-144">Mac-адрес WiFi устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="30d83-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="30d83-145">operatingSystemLanguage</span></span>|<span data-ttu-id="30d83-146">String</span><span class="sxs-lookup"><span data-stu-id="30d83-146">String</span></span>|<span data-ttu-id="30d83-147">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-147">Operating system language of the device</span></span>|
|<span data-ttu-id="30d83-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="30d83-148">isSupervised</span></span>|<span data-ttu-id="30d83-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d83-149">Boolean</span></span>|<span data-ttu-id="30d83-150">Контролируемый режим устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="30d83-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="30d83-151">isEncrypted</span></span>|<span data-ttu-id="30d83-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="30d83-152">Boolean</span></span>|<span data-ttu-id="30d83-153">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-153">Encryption status of the device</span></span>|
|<span data-ttu-id="30d83-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="30d83-154">batterySerialNumber</span></span>|<span data-ttu-id="30d83-155">String</span><span class="sxs-lookup"><span data-stu-id="30d83-155">String</span></span>|<span data-ttu-id="30d83-156">Серийный номер текущего аккумулятора устройства</span><span class="sxs-lookup"><span data-stu-id="30d83-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="30d83-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="30d83-157">batteryHealthPercentage</span></span>|<span data-ttu-id="30d83-158">Int32</span><span class="sxs-lookup"><span data-stu-id="30d83-158">Int32</span></span>|<span data-ttu-id="30d83-159">Процент состояния текущего аккумулятора устройства.</span><span class="sxs-lookup"><span data-stu-id="30d83-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="30d83-160">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="30d83-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="30d83-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="30d83-161">batteryChargeCycles</span></span>|<span data-ttu-id="30d83-162">Int32</span><span class="sxs-lookup"><span data-stu-id="30d83-162">Int32</span></span>|<span data-ttu-id="30d83-163">Количество циклов заряда текущего аккумулятора устройства прошло.</span><span class="sxs-lookup"><span data-stu-id="30d83-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="30d83-164">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="30d83-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="30d83-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="30d83-165">isSharedDevice</span></span>|<span data-ttu-id="30d83-166">Логический</span><span class="sxs-lookup"><span data-stu-id="30d83-166">Boolean</span></span>|<span data-ttu-id="30d83-167">Общий iPad</span><span class="sxs-lookup"><span data-stu-id="30d83-167">Shared iPad</span></span>|
|<span data-ttu-id="30d83-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="30d83-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="30d83-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span><span class="sxs-lookup"><span data-stu-id="30d83-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="30d83-170">Все пользователи на совместном устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="30d83-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="30d83-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="30d83-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="30d83-172">String</span><span class="sxs-lookup"><span data-stu-id="30d83-172">String</span></span>|<span data-ttu-id="30d83-173">Строка, которая указывает версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="30d83-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="30d83-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="30d83-174">operatingSystemEdition</span></span>|<span data-ttu-id="30d83-175">String</span><span class="sxs-lookup"><span data-stu-id="30d83-175">String</span></span>|<span data-ttu-id="30d83-176">Строка, заданная в выпуске ОС.</span><span class="sxs-lookup"><span data-stu-id="30d83-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="30d83-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="30d83-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="30d83-178">String</span><span class="sxs-lookup"><span data-stu-id="30d83-178">String</span></span>|<span data-ttu-id="30d83-179">Возвращает полностью квалифицированное доменное имя устройства (если таково).</span><span class="sxs-lookup"><span data-stu-id="30d83-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="30d83-180">Если устройство не присоединилось к домену, оно возвращает пустую строку.</span><span class="sxs-lookup"><span data-stu-id="30d83-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="30d83-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="30d83-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="30d83-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="30d83-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="30d83-183">Состояние требований к оборудованию безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="30d83-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="30d83-184">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="30d83-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="30d83-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="30d83-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="30d83-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="30d83-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="30d83-187">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="30d83-187">Virtualization-based security status.</span></span> <span data-ttu-id="30d83-188">.</span><span class="sxs-lookup"><span data-stu-id="30d83-188">.</span></span> <span data-ttu-id="30d83-189">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="30d83-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="30d83-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="30d83-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="30d83-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="30d83-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="30d83-192">Состояние охраны учетных данных местного управления системы (LSA).</span><span class="sxs-lookup"><span data-stu-id="30d83-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="30d83-193">.</span><span class="sxs-lookup"><span data-stu-id="30d83-193">.</span></span> <span data-ttu-id="30d83-194">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="30d83-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="30d83-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="30d83-195">osBuildNumber</span></span>|<span data-ttu-id="30d83-196">String</span><span class="sxs-lookup"><span data-stu-id="30d83-196">String</span></span>|<span data-ttu-id="30d83-197">Номер сборки операционной системы на устройстве Android</span><span class="sxs-lookup"><span data-stu-id="30d83-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="30d83-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="30d83-198">operatingSystemProductType</span></span>|<span data-ttu-id="30d83-199">Int32</span><span class="sxs-lookup"><span data-stu-id="30d83-199">Int32</span></span>|<span data-ttu-id="30d83-200">Int, который указывает продукт Операционной системы Windows.</span><span class="sxs-lookup"><span data-stu-id="30d83-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="30d83-201">Дополнительные сведения здесь https://go.microsoft.com/fwlink/?linkid=2126950 .</span><span class="sxs-lookup"><span data-stu-id="30d83-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="30d83-202">Допустимые значения от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="30d83-202">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="30d83-203">ipAddressV4</span><span class="sxs-lookup"><span data-stu-id="30d83-203">ipAddressV4</span></span>|<span data-ttu-id="30d83-204">String</span><span class="sxs-lookup"><span data-stu-id="30d83-204">String</span></span>|<span data-ttu-id="30d83-205">IPAddressV4</span><span class="sxs-lookup"><span data-stu-id="30d83-205">IPAddressV4</span></span>|
|<span data-ttu-id="30d83-206">subnetAddress</span><span class="sxs-lookup"><span data-stu-id="30d83-206">subnetAddress</span></span>|<span data-ttu-id="30d83-207">String</span><span class="sxs-lookup"><span data-stu-id="30d83-207">String</span></span>|<span data-ttu-id="30d83-208">SubnetAddress</span><span class="sxs-lookup"><span data-stu-id="30d83-208">SubnetAddress</span></span>|
|<span data-ttu-id="30d83-209">esimIdentifier</span><span class="sxs-lookup"><span data-stu-id="30d83-209">esimIdentifier</span></span>|<span data-ttu-id="30d83-210">String</span><span class="sxs-lookup"><span data-stu-id="30d83-210">String</span></span>|<span data-ttu-id="30d83-211">идентификатор eSIM</span><span class="sxs-lookup"><span data-stu-id="30d83-211">eSIM identifier</span></span>|
|<span data-ttu-id="30d83-212">systemManagementBIOSVersion</span><span class="sxs-lookup"><span data-stu-id="30d83-212">systemManagementBIOSVersion</span></span>|<span data-ttu-id="30d83-213">String</span><span class="sxs-lookup"><span data-stu-id="30d83-213">String</span></span>|<span data-ttu-id="30d83-214">Версия BIOS, как сообщает SMBIOS</span><span class="sxs-lookup"><span data-stu-id="30d83-214">BIOS version as reported by SMBIOS</span></span>|
|<span data-ttu-id="30d83-215">tpmManufacturer</span><span class="sxs-lookup"><span data-stu-id="30d83-215">tpmManufacturer</span></span>|<span data-ttu-id="30d83-216">String</span><span class="sxs-lookup"><span data-stu-id="30d83-216">String</span></span>|<span data-ttu-id="30d83-217">Идентифицирующие сведения, уникальные имена производителя TPM</span><span class="sxs-lookup"><span data-stu-id="30d83-217">The identifying information that uniquely names the TPM manufacturer</span></span>|
|<span data-ttu-id="30d83-218">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="30d83-218">tpmVersion</span></span>|<span data-ttu-id="30d83-219">String</span><span class="sxs-lookup"><span data-stu-id="30d83-219">String</span></span>|<span data-ttu-id="30d83-220">Версия TPM, указанная производителем</span><span class="sxs-lookup"><span data-stu-id="30d83-220">The version of the TPM, as specified by the manufacturer</span></span>|

## <a name="relationships"></a><span data-ttu-id="30d83-221">Связи</span><span class="sxs-lookup"><span data-stu-id="30d83-221">Relationships</span></span>
<span data-ttu-id="30d83-222">Нет</span><span class="sxs-lookup"><span data-stu-id="30d83-222">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30d83-223">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30d83-223">JSON Representation</span></span>
<span data-ttu-id="30d83-224">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30d83-224">Here is a JSON representation of the resource.</span></span>
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
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String"
}
```




