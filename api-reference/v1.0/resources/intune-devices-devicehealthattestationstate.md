---
title: Тип ресурса deviceHealthAttestationState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d246e5bd4235a3bc121d2809e95a59788bf9441
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972154"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="35cb0-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="35cb0-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="35cb0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35cb0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35cb0-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="35cb0-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="35cb0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="35cb0-106">Properties</span></span>
|<span data-ttu-id="35cb0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="35cb0-107">Property</span></span>|<span data-ttu-id="35cb0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="35cb0-108">Type</span></span>|<span data-ttu-id="35cb0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35cb0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35cb0-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="35cb0-110">lastUpdateDateTime</span></span>|<span data-ttu-id="35cb0-111">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-111">String</span></span>|<span data-ttu-id="35cb0-112">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="35cb0-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="35cb0-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="35cb0-113">contentNamespaceUrl</span></span>|<span data-ttu-id="35cb0-114">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-114">String</span></span>|<span data-ttu-id="35cb0-115">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="35cb0-115">The DHA report version.</span></span> <span data-ttu-id="35cb0-116">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="35cb0-116">(Namespace version)</span></span>|
|<span data-ttu-id="35cb0-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="35cb0-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="35cb0-118">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-118">String</span></span>|<span data-ttu-id="35cb0-119">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="35cb0-119">The DHA report version.</span></span> <span data-ttu-id="35cb0-120">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="35cb0-120">(Namespace version)</span></span>|
|<span data-ttu-id="35cb0-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-121">contentVersion</span></span>|<span data-ttu-id="35cb0-122">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-122">String</span></span>|<span data-ttu-id="35cb0-123">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="35cb0-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="35cb0-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="35cb0-124">issuedDateTime</span></span>|<span data-ttu-id="35cb0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35cb0-125">DateTimeOffset</span></span>|<span data-ttu-id="35cb0-126">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="35cb0-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="35cb0-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="35cb0-127">attestationIdentityKey</span></span>|<span data-ttu-id="35cb0-128">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-128">String</span></span>|<span data-ttu-id="35cb0-129">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="35cb0-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="35cb0-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="35cb0-130">resetCount</span></span>|<span data-ttu-id="35cb0-131">Int64</span><span class="sxs-lookup"><span data-stu-id="35cb0-131">Int64</span></span>|<span data-ttu-id="35cb0-132">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="35cb0-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="35cb0-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="35cb0-133">restartCount</span></span>|<span data-ttu-id="35cb0-134">Int64</span><span class="sxs-lookup"><span data-stu-id="35cb0-134">Int64</span></span>|<span data-ttu-id="35cb0-135">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="35cb0-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="35cb0-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="35cb0-136">dataExcutionPolicy</span></span>|<span data-ttu-id="35cb0-137">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-137">String</span></span>|<span data-ttu-id="35cb0-138">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="35cb0-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="35cb0-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="35cb0-139">bitLockerStatus</span></span>|<span data-ttu-id="35cb0-140">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-140">String</span></span>|<span data-ttu-id="35cb0-141">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="35cb0-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="35cb0-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-142">bootManagerVersion</span></span>|<span data-ttu-id="35cb0-143">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-143">String</span></span>|<span data-ttu-id="35cb0-144">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="35cb0-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="35cb0-146">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-146">String</span></span>|<span data-ttu-id="35cb0-147">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="35cb0-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="35cb0-148">secureBoot</span></span>|<span data-ttu-id="35cb0-149">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-149">String</span></span>|<span data-ttu-id="35cb0-150">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="35cb0-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="35cb0-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="35cb0-151">bootDebugging</span></span>|<span data-ttu-id="35cb0-152">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-152">String</span></span>|<span data-ttu-id="35cb0-153">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="35cb0-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="35cb0-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="35cb0-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="35cb0-155">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-155">String</span></span>|<span data-ttu-id="35cb0-156">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="35cb0-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="35cb0-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="35cb0-157">codeIntegrity</span></span>|<span data-ttu-id="35cb0-158">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-158">String</span></span>| <span data-ttu-id="35cb0-159">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="35cb0-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="35cb0-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="35cb0-160">testSigning</span></span>|<span data-ttu-id="35cb0-161">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-161">String</span></span>|<span data-ttu-id="35cb0-162">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="35cb0-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="35cb0-163">safeMode</span></span>|<span data-ttu-id="35cb0-164">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-164">String</span></span>|<span data-ttu-id="35cb0-165">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="35cb0-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="35cb0-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="35cb0-166">windowsPE</span></span>|<span data-ttu-id="35cb0-167">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-167">String</span></span>|<span data-ttu-id="35cb0-168">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="35cb0-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="35cb0-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="35cb0-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="35cb0-170">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-170">String</span></span>|<span data-ttu-id="35cb0-171">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="35cb0-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="35cb0-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="35cb0-172">virtualSecureMode</span></span>|<span data-ttu-id="35cb0-173">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-173">String</span></span>|<span data-ttu-id="35cb0-174">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="35cb0-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="35cb0-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="35cb0-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="35cb0-176">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-176">String</span></span>|<span data-ttu-id="35cb0-177">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="35cb0-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="35cb0-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="35cb0-179">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-179">String</span></span>|<span data-ttu-id="35cb0-180">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="35cb0-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="35cb0-182">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-182">String</span></span>|<span data-ttu-id="35cb0-183">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="35cb0-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="35cb0-184">tpmVersion</span></span>|<span data-ttu-id="35cb0-185">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-185">String</span></span>|<span data-ttu-id="35cb0-186">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="35cb0-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="35cb0-187">pcr0</span></span>|<span data-ttu-id="35cb0-188">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-188">String</span></span>|<span data-ttu-id="35cb0-189">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="35cb0-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="35cb0-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="35cb0-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="35cb0-191">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-191">String</span></span>|<span data-ttu-id="35cb0-192">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="35cb0-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="35cb0-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="35cb0-194">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-194">String</span></span>|<span data-ttu-id="35cb0-195">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="35cb0-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="35cb0-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="35cb0-196">bootRevisionListInfo</span></span>|<span data-ttu-id="35cb0-197">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-197">String</span></span>|<span data-ttu-id="35cb0-198">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="35cb0-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="35cb0-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="35cb0-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="35cb0-200">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-200">String</span></span>|<span data-ttu-id="35cb0-201">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="35cb0-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="35cb0-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="35cb0-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="35cb0-203">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-203">String</span></span>|<span data-ttu-id="35cb0-204">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="35cb0-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="35cb0-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="35cb0-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="35cb0-206">String</span><span class="sxs-lookup"><span data-stu-id="35cb0-206">String</span></span>|<span data-ttu-id="35cb0-207">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="35cb0-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="35cb0-208">Связи</span><span class="sxs-lookup"><span data-stu-id="35cb0-208">Relationships</span></span>
<span data-ttu-id="35cb0-209">Нет</span><span class="sxs-lookup"><span data-stu-id="35cb0-209">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35cb0-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35cb0-210">JSON Representation</span></span>
<span data-ttu-id="35cb0-211">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35cb0-211">Here is a JSON representation of the resource.</span></span>
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



