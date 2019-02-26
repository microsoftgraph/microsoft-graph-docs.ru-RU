---
title: Тип ресурса deviceHealthAttestationState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256149"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="d4834-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d4834-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="d4834-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4834-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4834-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d4834-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d4834-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4834-106">Properties</span></span>
|<span data-ttu-id="d4834-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4834-107">Property</span></span>|<span data-ttu-id="d4834-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d4834-108">Type</span></span>|<span data-ttu-id="d4834-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4834-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4834-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d4834-110">lastUpdateDateTime</span></span>|<span data-ttu-id="d4834-111">String</span><span class="sxs-lookup"><span data-stu-id="d4834-111">String</span></span>|<span data-ttu-id="d4834-112">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="d4834-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="d4834-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="d4834-113">contentNamespaceUrl</span></span>|<span data-ttu-id="d4834-114">String</span><span class="sxs-lookup"><span data-stu-id="d4834-114">String</span></span>|<span data-ttu-id="d4834-115">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="d4834-115">The DHA report version.</span></span> <span data-ttu-id="d4834-116">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="d4834-116">(Namespace version)</span></span>|
|<span data-ttu-id="d4834-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="d4834-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="d4834-118">String</span><span class="sxs-lookup"><span data-stu-id="d4834-118">String</span></span>|<span data-ttu-id="d4834-119">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="d4834-119">The DHA report version.</span></span> <span data-ttu-id="d4834-120">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="d4834-120">(Namespace version)</span></span>|
|<span data-ttu-id="d4834-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-121">contentVersion</span></span>|<span data-ttu-id="d4834-122">String</span><span class="sxs-lookup"><span data-stu-id="d4834-122">String</span></span>|<span data-ttu-id="d4834-123">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="d4834-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="d4834-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4834-124">issuedDateTime</span></span>|<span data-ttu-id="d4834-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4834-125">DateTimeOffset</span></span>|<span data-ttu-id="d4834-126">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="d4834-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="d4834-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="d4834-127">attestationIdentityKey</span></span>|<span data-ttu-id="d4834-128">String</span><span class="sxs-lookup"><span data-stu-id="d4834-128">String</span></span>|<span data-ttu-id="d4834-129">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="d4834-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="d4834-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="d4834-130">resetCount</span></span>|<span data-ttu-id="d4834-131">Int64</span><span class="sxs-lookup"><span data-stu-id="d4834-131">Int64</span></span>|<span data-ttu-id="d4834-132">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="d4834-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="d4834-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="d4834-133">restartCount</span></span>|<span data-ttu-id="d4834-134">Int64</span><span class="sxs-lookup"><span data-stu-id="d4834-134">Int64</span></span>|<span data-ttu-id="d4834-135">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="d4834-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="d4834-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="d4834-136">dataExcutionPolicy</span></span>|<span data-ttu-id="d4834-137">String</span><span class="sxs-lookup"><span data-stu-id="d4834-137">String</span></span>|<span data-ttu-id="d4834-138">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="d4834-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="d4834-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="d4834-139">bitLockerStatus</span></span>|<span data-ttu-id="d4834-140">String</span><span class="sxs-lookup"><span data-stu-id="d4834-140">String</span></span>|<span data-ttu-id="d4834-141">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d4834-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="d4834-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-142">bootManagerVersion</span></span>|<span data-ttu-id="d4834-143">String</span><span class="sxs-lookup"><span data-stu-id="d4834-143">String</span></span>|<span data-ttu-id="d4834-144">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="d4834-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="d4834-146">String</span><span class="sxs-lookup"><span data-stu-id="d4834-146">String</span></span>|<span data-ttu-id="d4834-147">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="d4834-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="d4834-148">secureBoot</span></span>|<span data-ttu-id="d4834-149">String</span><span class="sxs-lookup"><span data-stu-id="d4834-149">String</span></span>|<span data-ttu-id="d4834-150">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="d4834-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="d4834-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="d4834-151">bootDebugging</span></span>|<span data-ttu-id="d4834-152">String</span><span class="sxs-lookup"><span data-stu-id="d4834-152">String</span></span>|<span data-ttu-id="d4834-153">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="d4834-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="d4834-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="d4834-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="d4834-155">String</span><span class="sxs-lookup"><span data-stu-id="d4834-155">String</span></span>|<span data-ttu-id="d4834-156">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="d4834-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="d4834-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="d4834-157">codeIntegrity</span></span>|<span data-ttu-id="d4834-158">String</span><span class="sxs-lookup"><span data-stu-id="d4834-158">String</span></span>| <span data-ttu-id="d4834-159">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="d4834-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="d4834-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="d4834-160">testSigning</span></span>|<span data-ttu-id="d4834-161">String</span><span class="sxs-lookup"><span data-stu-id="d4834-161">String</span></span>|<span data-ttu-id="d4834-162">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="d4834-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="d4834-163">safeMode</span></span>|<span data-ttu-id="d4834-164">String</span><span class="sxs-lookup"><span data-stu-id="d4834-164">String</span></span>|<span data-ttu-id="d4834-165">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="d4834-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="d4834-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="d4834-166">windowsPE</span></span>|<span data-ttu-id="d4834-167">String</span><span class="sxs-lookup"><span data-stu-id="d4834-167">String</span></span>|<span data-ttu-id="d4834-168">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="d4834-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="d4834-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="d4834-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="d4834-170">String</span><span class="sxs-lookup"><span data-stu-id="d4834-170">String</span></span>|<span data-ttu-id="d4834-171">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="d4834-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="d4834-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="d4834-172">virtualSecureMode</span></span>|<span data-ttu-id="d4834-173">String</span><span class="sxs-lookup"><span data-stu-id="d4834-173">String</span></span>|<span data-ttu-id="d4834-174">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="d4834-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="d4834-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d4834-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="d4834-176">String</span><span class="sxs-lookup"><span data-stu-id="d4834-176">String</span></span>|<span data-ttu-id="d4834-177">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="d4834-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="d4834-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="d4834-179">String</span><span class="sxs-lookup"><span data-stu-id="d4834-179">String</span></span>|<span data-ttu-id="d4834-180">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d4834-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="d4834-182">String</span><span class="sxs-lookup"><span data-stu-id="d4834-182">String</span></span>|<span data-ttu-id="d4834-183">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d4834-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="d4834-184">tpmVersion</span></span>|<span data-ttu-id="d4834-185">String</span><span class="sxs-lookup"><span data-stu-id="d4834-185">String</span></span>|<span data-ttu-id="d4834-186">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d4834-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="d4834-187">pcr0</span></span>|<span data-ttu-id="d4834-188">String</span><span class="sxs-lookup"><span data-stu-id="d4834-188">String</span></span>|<span data-ttu-id="d4834-189">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="d4834-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="d4834-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="d4834-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="d4834-191">String</span><span class="sxs-lookup"><span data-stu-id="d4834-191">String</span></span>|<span data-ttu-id="d4834-192">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="d4834-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="d4834-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="d4834-194">String</span><span class="sxs-lookup"><span data-stu-id="d4834-194">String</span></span>|<span data-ttu-id="d4834-195">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="d4834-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="d4834-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="d4834-196">bootRevisionListInfo</span></span>|<span data-ttu-id="d4834-197">String</span><span class="sxs-lookup"><span data-stu-id="d4834-197">String</span></span>|<span data-ttu-id="d4834-198">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d4834-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="d4834-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="d4834-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="d4834-200">String</span><span class="sxs-lookup"><span data-stu-id="d4834-200">String</span></span>|<span data-ttu-id="d4834-201">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d4834-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="d4834-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="d4834-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="d4834-203">String</span><span class="sxs-lookup"><span data-stu-id="d4834-203">String</span></span>|<span data-ttu-id="d4834-204">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="d4834-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="d4834-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="d4834-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="d4834-206">String</span><span class="sxs-lookup"><span data-stu-id="d4834-206">String</span></span>|<span data-ttu-id="d4834-207">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="d4834-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4834-208">Связи</span><span class="sxs-lookup"><span data-stu-id="d4834-208">Relationships</span></span>
<span data-ttu-id="d4834-209">Нет</span><span class="sxs-lookup"><span data-stu-id="d4834-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4834-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4834-210">JSON Representation</span></span>
<span data-ttu-id="d4834-211">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4834-211">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```



