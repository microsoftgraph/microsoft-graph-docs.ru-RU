---
title: Тип ресурса Hardwareinformation.
description: Сведения об оборудовании для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c751b6601c296b01be91792105325e10a52ea2f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792708"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="11f6f-103">Тип ресурса Hardwareinformation.</span><span class="sxs-lookup"><span data-stu-id="11f6f-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="11f6f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11f6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11f6f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11f6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11f6f-106">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="11f6f-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="11f6f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="11f6f-107">Properties</span></span>
|<span data-ttu-id="11f6f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="11f6f-108">Property</span></span>|<span data-ttu-id="11f6f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="11f6f-109">Type</span></span>|<span data-ttu-id="11f6f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11f6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f6f-111">serialNumber</span><span class="sxs-lookup"><span data-stu-id="11f6f-111">serialNumber</span></span>|<span data-ttu-id="11f6f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="11f6f-112">String</span></span>|<span data-ttu-id="11f6f-113">Серийный номер.</span><span class="sxs-lookup"><span data-stu-id="11f6f-113">Serial number.</span></span>|
|<span data-ttu-id="11f6f-114">Тоталсторажеспаце</span><span class="sxs-lookup"><span data-stu-id="11f6f-114">totalStorageSpace</span></span>|<span data-ttu-id="11f6f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="11f6f-115">Int64</span></span>|<span data-ttu-id="11f6f-116">Общий объем хранилища устройства.</span><span class="sxs-lookup"><span data-stu-id="11f6f-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="11f6f-117">Фристоражеспаце</span><span class="sxs-lookup"><span data-stu-id="11f6f-117">freeStorageSpace</span></span>|<span data-ttu-id="11f6f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="11f6f-118">Int64</span></span>|<span data-ttu-id="11f6f-119">Свободное место на устройстве.</span><span class="sxs-lookup"><span data-stu-id="11f6f-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="11f6f-120">imei</span><span class="sxs-lookup"><span data-stu-id="11f6f-120">imei</span></span>|<span data-ttu-id="11f6f-121">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-121">String</span></span>|<span data-ttu-id="11f6f-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="11f6f-122">IMEI</span></span>|
|<span data-ttu-id="11f6f-123">meid</span><span class="sxs-lookup"><span data-stu-id="11f6f-123">meid</span></span>|<span data-ttu-id="11f6f-124">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-124">String</span></span>|<span data-ttu-id="11f6f-125">MEID</span><span class="sxs-lookup"><span data-stu-id="11f6f-125">MEID</span></span>|
|<span data-ttu-id="11f6f-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="11f6f-126">manufacturer</span></span>|<span data-ttu-id="11f6f-127">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-127">String</span></span>|<span data-ttu-id="11f6f-128">Производитель устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="11f6f-129">model</span><span class="sxs-lookup"><span data-stu-id="11f6f-129">model</span></span>|<span data-ttu-id="11f6f-130">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-130">String</span></span>|<span data-ttu-id="11f6f-131">Модель устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-131">Model of the device</span></span>|
|<span data-ttu-id="11f6f-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="11f6f-132">phoneNumber</span></span>|<span data-ttu-id="11f6f-133">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-133">String</span></span>|<span data-ttu-id="11f6f-134">Номер телефона устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-134">Phone number of the device</span></span>|
|<span data-ttu-id="11f6f-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="11f6f-135">subscriberCarrier</span></span>|<span data-ttu-id="11f6f-136">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-136">String</span></span>|<span data-ttu-id="11f6f-137">Абонентская перевозчик устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="11f6f-138">Целлулартечнологи</span><span class="sxs-lookup"><span data-stu-id="11f6f-138">cellularTechnology</span></span>|<span data-ttu-id="11f6f-139">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-139">String</span></span>|<span data-ttu-id="11f6f-140">Технология сотовой связи устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="11f6f-141">Вифимак</span><span class="sxs-lookup"><span data-stu-id="11f6f-141">wifiMac</span></span>|<span data-ttu-id="11f6f-142">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-142">String</span></span>|<span data-ttu-id="11f6f-143">MAC-адрес устройства Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="11f6f-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="11f6f-144">Оператингсистемлангуаже</span><span class="sxs-lookup"><span data-stu-id="11f6f-144">operatingSystemLanguage</span></span>|<span data-ttu-id="11f6f-145">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-145">String</span></span>|<span data-ttu-id="11f6f-146">Язык операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-146">Operating system language of the device</span></span>|
|<span data-ttu-id="11f6f-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="11f6f-147">isSupervised</span></span>|<span data-ttu-id="11f6f-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6f-148">Boolean</span></span>|<span data-ttu-id="11f6f-149">Контролируемый режим устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="11f6f-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="11f6f-150">isEncrypted</span></span>|<span data-ttu-id="11f6f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6f-151">Boolean</span></span>|<span data-ttu-id="11f6f-152">Состояние шифрования устройства</span><span class="sxs-lookup"><span data-stu-id="11f6f-152">Encryption status of the device</span></span>|
|<span data-ttu-id="11f6f-153">Свойства isshareddevice</span><span class="sxs-lookup"><span data-stu-id="11f6f-153">isSharedDevice</span></span>|<span data-ttu-id="11f6f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f6f-154">Boolean</span></span>|<span data-ttu-id="11f6f-155">Общие iPad</span><span class="sxs-lookup"><span data-stu-id="11f6f-155">Shared iPad</span></span>|
|<span data-ttu-id="11f6f-156">Шареддевицекачедусерс</span><span class="sxs-lookup"><span data-stu-id="11f6f-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="11f6f-157">Коллекция [шаредаппледевицеусер](../resources/intune-devices-sharedappledeviceuser.md)</span><span class="sxs-lookup"><span data-stu-id="11f6f-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="11f6f-158">Все пользователи на общем устройстве Apple</span><span class="sxs-lookup"><span data-stu-id="11f6f-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="11f6f-159">ТпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="11f6f-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="11f6f-160">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-160">String</span></span>|<span data-ttu-id="11f6f-161">Строка, указывающая версию спецификации.</span><span class="sxs-lookup"><span data-stu-id="11f6f-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="11f6f-162">Оператингсистемедитион</span><span class="sxs-lookup"><span data-stu-id="11f6f-162">operatingSystemEdition</span></span>|<span data-ttu-id="11f6f-163">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-163">String</span></span>|<span data-ttu-id="11f6f-164">Строка, задающая выпуск операционной системы.</span><span class="sxs-lookup"><span data-stu-id="11f6f-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="11f6f-165">Девицефуллкуалифиеддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="11f6f-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="11f6f-166">String</span><span class="sxs-lookup"><span data-stu-id="11f6f-166">String</span></span>|<span data-ttu-id="11f6f-167">Возвращает полное доменное имя устройства (при наличии).</span><span class="sxs-lookup"><span data-stu-id="11f6f-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="11f6f-168">Если устройство не присоединено к домену, возвращается пустая строка.</span><span class="sxs-lookup"><span data-stu-id="11f6f-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="11f6f-169">Девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="11f6f-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="11f6f-170">Девицегуардвиртуализатионбаседсекуритихардваререкуирементстате</span><span class="sxs-lookup"><span data-stu-id="11f6f-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="11f6f-171">Состояние требования к оборудованию для обеспечения безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="11f6f-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="11f6f-172">Возможные значения: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="11f6f-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="11f6f-173">Девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="11f6f-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="11f6f-174">Девицегуардвиртуализатионбаседсекуритистате</span><span class="sxs-lookup"><span data-stu-id="11f6f-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="11f6f-175">Состояние безопасности на основе виртуализации.</span><span class="sxs-lookup"><span data-stu-id="11f6f-175">Virtualization-based security status.</span></span> <span data-ttu-id="11f6f-176">.</span><span class="sxs-lookup"><span data-stu-id="11f6f-176"></span></span> <span data-ttu-id="11f6f-177">Возможные значения: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span><span class="sxs-lookup"><span data-stu-id="11f6f-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="11f6f-178">Девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="11f6f-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="11f6f-179">Девицегуардлокалсистемаусоритикредентиалгуардстате</span><span class="sxs-lookup"><span data-stu-id="11f6f-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="11f6f-180">Состояние Credential Guard в администраторе локальной системы (LSA).</span><span class="sxs-lookup"><span data-stu-id="11f6f-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="11f6f-181">.</span><span class="sxs-lookup"><span data-stu-id="11f6f-181"></span></span> <span data-ttu-id="11f6f-182">Возможные значения: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span><span class="sxs-lookup"><span data-stu-id="11f6f-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11f6f-183">Отношения</span><span class="sxs-lookup"><span data-stu-id="11f6f-183">Relationships</span></span>
<span data-ttu-id="11f6f-184">Нет</span><span class="sxs-lookup"><span data-stu-id="11f6f-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11f6f-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11f6f-185">JSON Representation</span></span>
<span data-ttu-id="11f6f-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11f6f-186">Here is a JSON representation of the resource.</span></span>
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





