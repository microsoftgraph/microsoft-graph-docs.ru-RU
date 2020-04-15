---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41c9fd4f09749857c9aeb588086ef23ce5775d48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454006"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="d61db-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="d61db-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="d61db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d61db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d61db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61db-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d61db-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d61db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d61db-107">Properties</span></span>
|<span data-ttu-id="d61db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d61db-108">Property</span></span>|<span data-ttu-id="d61db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d61db-109">Type</span></span>|<span data-ttu-id="d61db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d61db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61db-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d61db-111">lastUpdateDateTime</span></span>|<span data-ttu-id="d61db-112">String</span><span class="sxs-lookup"><span data-stu-id="d61db-112">String</span></span>|<span data-ttu-id="d61db-113">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="d61db-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="d61db-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="d61db-114">contentNamespaceUrl</span></span>|<span data-ttu-id="d61db-115">String</span><span class="sxs-lookup"><span data-stu-id="d61db-115">String</span></span>|<span data-ttu-id="d61db-116">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="d61db-116">The DHA report version.</span></span> <span data-ttu-id="d61db-117">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="d61db-117">(Namespace version)</span></span>|
|<span data-ttu-id="d61db-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="d61db-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="d61db-119">String</span><span class="sxs-lookup"><span data-stu-id="d61db-119">String</span></span>|<span data-ttu-id="d61db-120">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="d61db-120">The DHA report version.</span></span> <span data-ttu-id="d61db-121">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="d61db-121">(Namespace version)</span></span>|
|<span data-ttu-id="d61db-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-122">contentVersion</span></span>|<span data-ttu-id="d61db-123">String</span><span class="sxs-lookup"><span data-stu-id="d61db-123">String</span></span>|<span data-ttu-id="d61db-124">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="d61db-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="d61db-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="d61db-125">issuedDateTime</span></span>|<span data-ttu-id="d61db-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d61db-126">DateTimeOffset</span></span>|<span data-ttu-id="d61db-127">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="d61db-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="d61db-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="d61db-128">attestationIdentityKey</span></span>|<span data-ttu-id="d61db-129">String</span><span class="sxs-lookup"><span data-stu-id="d61db-129">String</span></span>|<span data-ttu-id="d61db-130">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="d61db-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="d61db-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="d61db-131">resetCount</span></span>|<span data-ttu-id="d61db-132">Int64</span><span class="sxs-lookup"><span data-stu-id="d61db-132">Int64</span></span>|<span data-ttu-id="d61db-133">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="d61db-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="d61db-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="d61db-134">restartCount</span></span>|<span data-ttu-id="d61db-135">Int64</span><span class="sxs-lookup"><span data-stu-id="d61db-135">Int64</span></span>|<span data-ttu-id="d61db-136">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="d61db-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="d61db-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="d61db-137">dataExcutionPolicy</span></span>|<span data-ttu-id="d61db-138">String</span><span class="sxs-lookup"><span data-stu-id="d61db-138">String</span></span>|<span data-ttu-id="d61db-139">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="d61db-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="d61db-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="d61db-140">bitLockerStatus</span></span>|<span data-ttu-id="d61db-141">String</span><span class="sxs-lookup"><span data-stu-id="d61db-141">String</span></span>|<span data-ttu-id="d61db-142">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d61db-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="d61db-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-143">bootManagerVersion</span></span>|<span data-ttu-id="d61db-144">String</span><span class="sxs-lookup"><span data-stu-id="d61db-144">String</span></span>|<span data-ttu-id="d61db-145">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="d61db-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="d61db-147">String</span><span class="sxs-lookup"><span data-stu-id="d61db-147">String</span></span>|<span data-ttu-id="d61db-148">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="d61db-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="d61db-149">secureBoot</span></span>|<span data-ttu-id="d61db-150">String</span><span class="sxs-lookup"><span data-stu-id="d61db-150">String</span></span>|<span data-ttu-id="d61db-151">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="d61db-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="d61db-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="d61db-152">bootDebugging</span></span>|<span data-ttu-id="d61db-153">String</span><span class="sxs-lookup"><span data-stu-id="d61db-153">String</span></span>|<span data-ttu-id="d61db-154">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="d61db-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="d61db-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="d61db-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="d61db-156">String</span><span class="sxs-lookup"><span data-stu-id="d61db-156">String</span></span>|<span data-ttu-id="d61db-157">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="d61db-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="d61db-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="d61db-158">codeIntegrity</span></span>|<span data-ttu-id="d61db-159">String</span><span class="sxs-lookup"><span data-stu-id="d61db-159">String</span></span>| <span data-ttu-id="d61db-160">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="d61db-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="d61db-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="d61db-161">testSigning</span></span>|<span data-ttu-id="d61db-162">String</span><span class="sxs-lookup"><span data-stu-id="d61db-162">String</span></span>|<span data-ttu-id="d61db-163">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="d61db-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="d61db-164">safeMode</span></span>|<span data-ttu-id="d61db-165">String</span><span class="sxs-lookup"><span data-stu-id="d61db-165">String</span></span>|<span data-ttu-id="d61db-166">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="d61db-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="d61db-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="d61db-167">windowsPE</span></span>|<span data-ttu-id="d61db-168">String</span><span class="sxs-lookup"><span data-stu-id="d61db-168">String</span></span>|<span data-ttu-id="d61db-169">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="d61db-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="d61db-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="d61db-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="d61db-171">String</span><span class="sxs-lookup"><span data-stu-id="d61db-171">String</span></span>|<span data-ttu-id="d61db-172">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="d61db-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="d61db-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="d61db-173">virtualSecureMode</span></span>|<span data-ttu-id="d61db-174">String</span><span class="sxs-lookup"><span data-stu-id="d61db-174">String</span></span>|<span data-ttu-id="d61db-175">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="d61db-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="d61db-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d61db-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="d61db-177">String</span><span class="sxs-lookup"><span data-stu-id="d61db-177">String</span></span>|<span data-ttu-id="d61db-178">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="d61db-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="d61db-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="d61db-180">String</span><span class="sxs-lookup"><span data-stu-id="d61db-180">String</span></span>|<span data-ttu-id="d61db-181">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d61db-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="d61db-183">String</span><span class="sxs-lookup"><span data-stu-id="d61db-183">String</span></span>|<span data-ttu-id="d61db-184">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d61db-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="d61db-185">tpmVersion</span></span>|<span data-ttu-id="d61db-186">String</span><span class="sxs-lookup"><span data-stu-id="d61db-186">String</span></span>|<span data-ttu-id="d61db-187">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="d61db-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="d61db-188">pcr0</span></span>|<span data-ttu-id="d61db-189">String</span><span class="sxs-lookup"><span data-stu-id="d61db-189">String</span></span>|<span data-ttu-id="d61db-190">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="d61db-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="d61db-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="d61db-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="d61db-192">String</span><span class="sxs-lookup"><span data-stu-id="d61db-192">String</span></span>|<span data-ttu-id="d61db-193">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="d61db-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="d61db-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="d61db-195">String</span><span class="sxs-lookup"><span data-stu-id="d61db-195">String</span></span>|<span data-ttu-id="d61db-196">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="d61db-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="d61db-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="d61db-197">bootRevisionListInfo</span></span>|<span data-ttu-id="d61db-198">String</span><span class="sxs-lookup"><span data-stu-id="d61db-198">String</span></span>|<span data-ttu-id="d61db-199">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d61db-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="d61db-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="d61db-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="d61db-201">String</span><span class="sxs-lookup"><span data-stu-id="d61db-201">String</span></span>|<span data-ttu-id="d61db-202">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d61db-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="d61db-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="d61db-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="d61db-204">String</span><span class="sxs-lookup"><span data-stu-id="d61db-204">String</span></span>|<span data-ttu-id="d61db-205">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="d61db-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="d61db-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="d61db-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="d61db-207">String</span><span class="sxs-lookup"><span data-stu-id="d61db-207">String</span></span>|<span data-ttu-id="d61db-208">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="d61db-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="d61db-209">Отношения</span><span class="sxs-lookup"><span data-stu-id="d61db-209">Relationships</span></span>
<span data-ttu-id="d61db-210">Нет</span><span class="sxs-lookup"><span data-stu-id="d61db-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61db-211">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d61db-211">JSON Representation</span></span>
<span data-ttu-id="d61db-212">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d61db-212">Here is a JSON representation of the resource.</span></span>
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







