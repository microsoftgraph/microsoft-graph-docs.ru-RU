---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26070efb2247ef1fdfa60f45a985eb9223de923b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356963"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="0a561-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="0a561-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="0a561-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a561-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a561-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0a561-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0a561-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a561-106">Properties</span></span>
|<span data-ttu-id="0a561-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a561-107">Property</span></span>|<span data-ttu-id="0a561-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0a561-108">Type</span></span>|<span data-ttu-id="0a561-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0a561-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a561-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0a561-110">lastUpdateDateTime</span></span>|<span data-ttu-id="0a561-111">String</span><span class="sxs-lookup"><span data-stu-id="0a561-111">String</span></span>|<span data-ttu-id="0a561-112">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="0a561-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="0a561-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="0a561-113">contentNamespaceUrl</span></span>|<span data-ttu-id="0a561-114">String</span><span class="sxs-lookup"><span data-stu-id="0a561-114">String</span></span>|<span data-ttu-id="0a561-115">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="0a561-115">The DHA report version.</span></span> <span data-ttu-id="0a561-116">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="0a561-116">(Namespace version)</span></span>|
|<span data-ttu-id="0a561-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="0a561-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="0a561-118">String</span><span class="sxs-lookup"><span data-stu-id="0a561-118">String</span></span>|<span data-ttu-id="0a561-119">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="0a561-119">The DHA report version.</span></span> <span data-ttu-id="0a561-120">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="0a561-120">(Namespace version)</span></span>|
|<span data-ttu-id="0a561-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-121">contentVersion</span></span>|<span data-ttu-id="0a561-122">String</span><span class="sxs-lookup"><span data-stu-id="0a561-122">String</span></span>|<span data-ttu-id="0a561-123">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="0a561-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="0a561-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a561-124">issuedDateTime</span></span>|<span data-ttu-id="0a561-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a561-125">DateTimeOffset</span></span>|<span data-ttu-id="0a561-126">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="0a561-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="0a561-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="0a561-127">attestationIdentityKey</span></span>|<span data-ttu-id="0a561-128">String</span><span class="sxs-lookup"><span data-stu-id="0a561-128">String</span></span>|<span data-ttu-id="0a561-129">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="0a561-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="0a561-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="0a561-130">resetCount</span></span>|<span data-ttu-id="0a561-131">Int64</span><span class="sxs-lookup"><span data-stu-id="0a561-131">Int64</span></span>|<span data-ttu-id="0a561-132">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="0a561-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="0a561-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="0a561-133">restartCount</span></span>|<span data-ttu-id="0a561-134">Int64</span><span class="sxs-lookup"><span data-stu-id="0a561-134">Int64</span></span>|<span data-ttu-id="0a561-135">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="0a561-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="0a561-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="0a561-136">dataExcutionPolicy</span></span>|<span data-ttu-id="0a561-137">String</span><span class="sxs-lookup"><span data-stu-id="0a561-137">String</span></span>|<span data-ttu-id="0a561-138">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="0a561-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="0a561-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="0a561-139">bitLockerStatus</span></span>|<span data-ttu-id="0a561-140">String</span><span class="sxs-lookup"><span data-stu-id="0a561-140">String</span></span>|<span data-ttu-id="0a561-141">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="0a561-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="0a561-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-142">bootManagerVersion</span></span>|<span data-ttu-id="0a561-143">String</span><span class="sxs-lookup"><span data-stu-id="0a561-143">String</span></span>|<span data-ttu-id="0a561-144">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="0a561-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="0a561-146">String</span><span class="sxs-lookup"><span data-stu-id="0a561-146">String</span></span>|<span data-ttu-id="0a561-147">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="0a561-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="0a561-148">secureBoot</span></span>|<span data-ttu-id="0a561-149">String</span><span class="sxs-lookup"><span data-stu-id="0a561-149">String</span></span>|<span data-ttu-id="0a561-150">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="0a561-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="0a561-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="0a561-151">bootDebugging</span></span>|<span data-ttu-id="0a561-152">String</span><span class="sxs-lookup"><span data-stu-id="0a561-152">String</span></span>|<span data-ttu-id="0a561-153">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="0a561-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="0a561-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="0a561-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="0a561-155">String</span><span class="sxs-lookup"><span data-stu-id="0a561-155">String</span></span>|<span data-ttu-id="0a561-156">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="0a561-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="0a561-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="0a561-157">codeIntegrity</span></span>|<span data-ttu-id="0a561-158">String</span><span class="sxs-lookup"><span data-stu-id="0a561-158">String</span></span>| <span data-ttu-id="0a561-159">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="0a561-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="0a561-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="0a561-160">testSigning</span></span>|<span data-ttu-id="0a561-161">String</span><span class="sxs-lookup"><span data-stu-id="0a561-161">String</span></span>|<span data-ttu-id="0a561-162">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="0a561-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="0a561-163">safeMode</span></span>|<span data-ttu-id="0a561-164">String</span><span class="sxs-lookup"><span data-stu-id="0a561-164">String</span></span>|<span data-ttu-id="0a561-165">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="0a561-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="0a561-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="0a561-166">windowsPE</span></span>|<span data-ttu-id="0a561-167">String</span><span class="sxs-lookup"><span data-stu-id="0a561-167">String</span></span>|<span data-ttu-id="0a561-168">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="0a561-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="0a561-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="0a561-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="0a561-170">String</span><span class="sxs-lookup"><span data-stu-id="0a561-170">String</span></span>|<span data-ttu-id="0a561-171">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="0a561-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="0a561-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="0a561-172">virtualSecureMode</span></span>|<span data-ttu-id="0a561-173">String</span><span class="sxs-lookup"><span data-stu-id="0a561-173">String</span></span>|<span data-ttu-id="0a561-174">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="0a561-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="0a561-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0a561-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="0a561-176">String</span><span class="sxs-lookup"><span data-stu-id="0a561-176">String</span></span>|<span data-ttu-id="0a561-177">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="0a561-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="0a561-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="0a561-179">String</span><span class="sxs-lookup"><span data-stu-id="0a561-179">String</span></span>|<span data-ttu-id="0a561-180">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0a561-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="0a561-182">String</span><span class="sxs-lookup"><span data-stu-id="0a561-182">String</span></span>|<span data-ttu-id="0a561-183">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0a561-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="0a561-184">tpmVersion</span></span>|<span data-ttu-id="0a561-185">String</span><span class="sxs-lookup"><span data-stu-id="0a561-185">String</span></span>|<span data-ttu-id="0a561-186">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="0a561-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="0a561-187">pcr0</span></span>|<span data-ttu-id="0a561-188">String</span><span class="sxs-lookup"><span data-stu-id="0a561-188">String</span></span>|<span data-ttu-id="0a561-189">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="0a561-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="0a561-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="0a561-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="0a561-191">String</span><span class="sxs-lookup"><span data-stu-id="0a561-191">String</span></span>|<span data-ttu-id="0a561-192">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="0a561-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="0a561-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="0a561-194">String</span><span class="sxs-lookup"><span data-stu-id="0a561-194">String</span></span>|<span data-ttu-id="0a561-195">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="0a561-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="0a561-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="0a561-196">bootRevisionListInfo</span></span>|<span data-ttu-id="0a561-197">String</span><span class="sxs-lookup"><span data-stu-id="0a561-197">String</span></span>|<span data-ttu-id="0a561-198">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a561-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="0a561-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="0a561-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="0a561-200">String</span><span class="sxs-lookup"><span data-stu-id="0a561-200">String</span></span>|<span data-ttu-id="0a561-201">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="0a561-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="0a561-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="0a561-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="0a561-203">String</span><span class="sxs-lookup"><span data-stu-id="0a561-203">String</span></span>|<span data-ttu-id="0a561-204">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="0a561-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="0a561-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="0a561-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="0a561-206">String</span><span class="sxs-lookup"><span data-stu-id="0a561-206">String</span></span>|<span data-ttu-id="0a561-207">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="0a561-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a561-208">Связи</span><span class="sxs-lookup"><span data-stu-id="0a561-208">Relationships</span></span>
<span data-ttu-id="0a561-209">Нет</span><span class="sxs-lookup"><span data-stu-id="0a561-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a561-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a561-210">JSON Representation</span></span>
<span data-ttu-id="0a561-211">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a561-211">Here is a JSON representation of the resource.</span></span>
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




