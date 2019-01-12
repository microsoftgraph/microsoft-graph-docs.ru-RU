---
title: Тип ресурса deviceHealthAttestationState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03729d2c3a3f61c74bf7966f67a12084b7d24e25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987876"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="67bfc-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="67bfc-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="67bfc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="67bfc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67bfc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67bfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67bfc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="67bfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67bfc-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="67bfc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="67bfc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67bfc-108">Properties</span></span>
|<span data-ttu-id="67bfc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67bfc-109">Property</span></span>|<span data-ttu-id="67bfc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67bfc-110">Type</span></span>|<span data-ttu-id="67bfc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67bfc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bfc-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="67bfc-112">lastUpdateDateTime</span></span>|<span data-ttu-id="67bfc-113">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-113">String</span></span>|<span data-ttu-id="67bfc-114">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="67bfc-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="67bfc-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="67bfc-115">contentNamespaceUrl</span></span>|<span data-ttu-id="67bfc-116">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-116">String</span></span>|<span data-ttu-id="67bfc-117">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="67bfc-117">The DHA report version.</span></span> <span data-ttu-id="67bfc-118">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="67bfc-118">(Namespace version)</span></span>|
|<span data-ttu-id="67bfc-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="67bfc-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="67bfc-120">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-120">String</span></span>|<span data-ttu-id="67bfc-121">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="67bfc-121">The DHA report version.</span></span> <span data-ttu-id="67bfc-122">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="67bfc-122">(Namespace version)</span></span>|
|<span data-ttu-id="67bfc-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-123">contentVersion</span></span>|<span data-ttu-id="67bfc-124">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-124">String</span></span>|<span data-ttu-id="67bfc-125">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="67bfc-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="67bfc-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="67bfc-126">issuedDateTime</span></span>|<span data-ttu-id="67bfc-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67bfc-127">DateTimeOffset</span></span>|<span data-ttu-id="67bfc-128">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="67bfc-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="67bfc-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="67bfc-129">attestationIdentityKey</span></span>|<span data-ttu-id="67bfc-130">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-130">String</span></span>|<span data-ttu-id="67bfc-131">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="67bfc-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="67bfc-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="67bfc-132">resetCount</span></span>|<span data-ttu-id="67bfc-133">Int64</span><span class="sxs-lookup"><span data-stu-id="67bfc-133">Int64</span></span>|<span data-ttu-id="67bfc-134">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="67bfc-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="67bfc-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="67bfc-135">restartCount</span></span>|<span data-ttu-id="67bfc-136">Int64</span><span class="sxs-lookup"><span data-stu-id="67bfc-136">Int64</span></span>|<span data-ttu-id="67bfc-137">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="67bfc-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="67bfc-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="67bfc-138">dataExcutionPolicy</span></span>|<span data-ttu-id="67bfc-139">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-139">String</span></span>|<span data-ttu-id="67bfc-140">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="67bfc-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="67bfc-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="67bfc-141">bitLockerStatus</span></span>|<span data-ttu-id="67bfc-142">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-142">String</span></span>|<span data-ttu-id="67bfc-143">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="67bfc-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="67bfc-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-144">bootManagerVersion</span></span>|<span data-ttu-id="67bfc-145">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-145">String</span></span>|<span data-ttu-id="67bfc-146">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="67bfc-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="67bfc-148">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-148">String</span></span>|<span data-ttu-id="67bfc-149">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="67bfc-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="67bfc-150">secureBoot</span></span>|<span data-ttu-id="67bfc-151">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-151">String</span></span>|<span data-ttu-id="67bfc-152">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="67bfc-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="67bfc-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="67bfc-153">bootDebugging</span></span>|<span data-ttu-id="67bfc-154">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-154">String</span></span>|<span data-ttu-id="67bfc-155">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="67bfc-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="67bfc-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="67bfc-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="67bfc-157">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-157">String</span></span>|<span data-ttu-id="67bfc-158">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="67bfc-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="67bfc-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="67bfc-159">codeIntegrity</span></span>|<span data-ttu-id="67bfc-160">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-160">String</span></span>| <span data-ttu-id="67bfc-161">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="67bfc-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="67bfc-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="67bfc-162">testSigning</span></span>|<span data-ttu-id="67bfc-163">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-163">String</span></span>|<span data-ttu-id="67bfc-164">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="67bfc-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="67bfc-165">safeMode</span></span>|<span data-ttu-id="67bfc-166">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-166">String</span></span>|<span data-ttu-id="67bfc-167">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="67bfc-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="67bfc-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="67bfc-168">windowsPE</span></span>|<span data-ttu-id="67bfc-169">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-169">String</span></span>|<span data-ttu-id="67bfc-170">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="67bfc-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="67bfc-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="67bfc-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="67bfc-172">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-172">String</span></span>|<span data-ttu-id="67bfc-173">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="67bfc-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="67bfc-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="67bfc-174">virtualSecureMode</span></span>|<span data-ttu-id="67bfc-175">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-175">String</span></span>|<span data-ttu-id="67bfc-176">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="67bfc-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="67bfc-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="67bfc-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="67bfc-178">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-178">String</span></span>|<span data-ttu-id="67bfc-179">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="67bfc-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="67bfc-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="67bfc-181">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-181">String</span></span>|<span data-ttu-id="67bfc-182">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="67bfc-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="67bfc-184">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-184">String</span></span>|<span data-ttu-id="67bfc-185">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="67bfc-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="67bfc-186">tpmVersion</span></span>|<span data-ttu-id="67bfc-187">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-187">String</span></span>|<span data-ttu-id="67bfc-188">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="67bfc-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="67bfc-189">pcr0</span></span>|<span data-ttu-id="67bfc-190">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-190">String</span></span>|<span data-ttu-id="67bfc-191">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="67bfc-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="67bfc-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="67bfc-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="67bfc-193">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-193">String</span></span>|<span data-ttu-id="67bfc-194">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="67bfc-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="67bfc-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="67bfc-196">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-196">String</span></span>|<span data-ttu-id="67bfc-197">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="67bfc-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="67bfc-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="67bfc-198">bootRevisionListInfo</span></span>|<span data-ttu-id="67bfc-199">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-199">String</span></span>|<span data-ttu-id="67bfc-200">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="67bfc-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="67bfc-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="67bfc-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="67bfc-202">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-202">String</span></span>|<span data-ttu-id="67bfc-203">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="67bfc-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="67bfc-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="67bfc-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="67bfc-205">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-205">String</span></span>|<span data-ttu-id="67bfc-206">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="67bfc-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="67bfc-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="67bfc-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="67bfc-208">String</span><span class="sxs-lookup"><span data-stu-id="67bfc-208">String</span></span>|<span data-ttu-id="67bfc-209">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="67bfc-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="67bfc-210">Связи</span><span class="sxs-lookup"><span data-stu-id="67bfc-210">Relationships</span></span>
<span data-ttu-id="67bfc-211">Нет</span><span class="sxs-lookup"><span data-stu-id="67bfc-211">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67bfc-212">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67bfc-212">JSON Representation</span></span>
<span data-ttu-id="67bfc-213">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67bfc-213">Here is a JSON representation of the resource.</span></span>
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





