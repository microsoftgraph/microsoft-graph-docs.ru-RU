---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f43fee985ca760cfe3323f55ce79aaa043d9bd9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260063"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="547c7-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="547c7-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="547c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="547c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="547c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="547c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="547c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="547c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="547c7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="547c7-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="547c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="547c7-108">Properties</span></span>
|<span data-ttu-id="547c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="547c7-109">Property</span></span>|<span data-ttu-id="547c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="547c7-110">Type</span></span>|<span data-ttu-id="547c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="547c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="547c7-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="547c7-112">lastUpdateDateTime</span></span>|<span data-ttu-id="547c7-113">String</span><span class="sxs-lookup"><span data-stu-id="547c7-113">String</span></span>|<span data-ttu-id="547c7-114">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="547c7-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="547c7-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="547c7-115">contentNamespaceUrl</span></span>|<span data-ttu-id="547c7-116">String</span><span class="sxs-lookup"><span data-stu-id="547c7-116">String</span></span>|<span data-ttu-id="547c7-117">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="547c7-117">The DHA report version.</span></span> <span data-ttu-id="547c7-118">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="547c7-118">(Namespace version)</span></span>|
|<span data-ttu-id="547c7-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="547c7-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="547c7-120">String</span><span class="sxs-lookup"><span data-stu-id="547c7-120">String</span></span>|<span data-ttu-id="547c7-121">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="547c7-121">The DHA report version.</span></span> <span data-ttu-id="547c7-122">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="547c7-122">(Namespace version)</span></span>|
|<span data-ttu-id="547c7-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-123">contentVersion</span></span>|<span data-ttu-id="547c7-124">String</span><span class="sxs-lookup"><span data-stu-id="547c7-124">String</span></span>|<span data-ttu-id="547c7-125">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="547c7-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="547c7-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="547c7-126">issuedDateTime</span></span>|<span data-ttu-id="547c7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="547c7-127">DateTimeOffset</span></span>|<span data-ttu-id="547c7-128">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="547c7-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="547c7-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="547c7-129">attestationIdentityKey</span></span>|<span data-ttu-id="547c7-130">String</span><span class="sxs-lookup"><span data-stu-id="547c7-130">String</span></span>|<span data-ttu-id="547c7-131">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="547c7-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="547c7-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="547c7-132">resetCount</span></span>|<span data-ttu-id="547c7-133">Int64</span><span class="sxs-lookup"><span data-stu-id="547c7-133">Int64</span></span>|<span data-ttu-id="547c7-134">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="547c7-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="547c7-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="547c7-135">restartCount</span></span>|<span data-ttu-id="547c7-136">Int64</span><span class="sxs-lookup"><span data-stu-id="547c7-136">Int64</span></span>|<span data-ttu-id="547c7-137">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="547c7-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="547c7-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="547c7-138">dataExcutionPolicy</span></span>|<span data-ttu-id="547c7-139">String</span><span class="sxs-lookup"><span data-stu-id="547c7-139">String</span></span>|<span data-ttu-id="547c7-140">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="547c7-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="547c7-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="547c7-141">bitLockerStatus</span></span>|<span data-ttu-id="547c7-142">String</span><span class="sxs-lookup"><span data-stu-id="547c7-142">String</span></span>|<span data-ttu-id="547c7-143">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="547c7-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="547c7-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-144">bootManagerVersion</span></span>|<span data-ttu-id="547c7-145">String</span><span class="sxs-lookup"><span data-stu-id="547c7-145">String</span></span>|<span data-ttu-id="547c7-146">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="547c7-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="547c7-148">String</span><span class="sxs-lookup"><span data-stu-id="547c7-148">String</span></span>|<span data-ttu-id="547c7-149">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="547c7-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="547c7-150">secureBoot</span></span>|<span data-ttu-id="547c7-151">String</span><span class="sxs-lookup"><span data-stu-id="547c7-151">String</span></span>|<span data-ttu-id="547c7-152">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="547c7-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="547c7-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="547c7-153">bootDebugging</span></span>|<span data-ttu-id="547c7-154">String</span><span class="sxs-lookup"><span data-stu-id="547c7-154">String</span></span>|<span data-ttu-id="547c7-155">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="547c7-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="547c7-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="547c7-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="547c7-157">String</span><span class="sxs-lookup"><span data-stu-id="547c7-157">String</span></span>|<span data-ttu-id="547c7-158">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="547c7-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="547c7-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="547c7-159">codeIntegrity</span></span>|<span data-ttu-id="547c7-160">String</span><span class="sxs-lookup"><span data-stu-id="547c7-160">String</span></span>| <span data-ttu-id="547c7-161">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="547c7-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="547c7-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="547c7-162">testSigning</span></span>|<span data-ttu-id="547c7-163">String</span><span class="sxs-lookup"><span data-stu-id="547c7-163">String</span></span>|<span data-ttu-id="547c7-164">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="547c7-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="547c7-165">safeMode</span></span>|<span data-ttu-id="547c7-166">String</span><span class="sxs-lookup"><span data-stu-id="547c7-166">String</span></span>|<span data-ttu-id="547c7-167">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="547c7-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="547c7-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="547c7-168">windowsPE</span></span>|<span data-ttu-id="547c7-169">String</span><span class="sxs-lookup"><span data-stu-id="547c7-169">String</span></span>|<span data-ttu-id="547c7-170">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="547c7-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="547c7-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="547c7-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="547c7-172">String</span><span class="sxs-lookup"><span data-stu-id="547c7-172">String</span></span>|<span data-ttu-id="547c7-173">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="547c7-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="547c7-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="547c7-174">virtualSecureMode</span></span>|<span data-ttu-id="547c7-175">String</span><span class="sxs-lookup"><span data-stu-id="547c7-175">String</span></span>|<span data-ttu-id="547c7-176">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="547c7-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="547c7-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="547c7-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="547c7-178">String</span><span class="sxs-lookup"><span data-stu-id="547c7-178">String</span></span>|<span data-ttu-id="547c7-179">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="547c7-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="547c7-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="547c7-181">String</span><span class="sxs-lookup"><span data-stu-id="547c7-181">String</span></span>|<span data-ttu-id="547c7-182">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="547c7-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="547c7-184">String</span><span class="sxs-lookup"><span data-stu-id="547c7-184">String</span></span>|<span data-ttu-id="547c7-185">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="547c7-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="547c7-186">tpmVersion</span></span>|<span data-ttu-id="547c7-187">String</span><span class="sxs-lookup"><span data-stu-id="547c7-187">String</span></span>|<span data-ttu-id="547c7-188">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="547c7-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="547c7-189">pcr0</span></span>|<span data-ttu-id="547c7-190">String</span><span class="sxs-lookup"><span data-stu-id="547c7-190">String</span></span>|<span data-ttu-id="547c7-191">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="547c7-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="547c7-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="547c7-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="547c7-193">String</span><span class="sxs-lookup"><span data-stu-id="547c7-193">String</span></span>|<span data-ttu-id="547c7-194">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="547c7-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="547c7-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="547c7-196">String</span><span class="sxs-lookup"><span data-stu-id="547c7-196">String</span></span>|<span data-ttu-id="547c7-197">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="547c7-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="547c7-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="547c7-198">bootRevisionListInfo</span></span>|<span data-ttu-id="547c7-199">String</span><span class="sxs-lookup"><span data-stu-id="547c7-199">String</span></span>|<span data-ttu-id="547c7-200">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="547c7-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="547c7-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="547c7-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="547c7-202">String</span><span class="sxs-lookup"><span data-stu-id="547c7-202">String</span></span>|<span data-ttu-id="547c7-203">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="547c7-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="547c7-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="547c7-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="547c7-205">String</span><span class="sxs-lookup"><span data-stu-id="547c7-205">String</span></span>|<span data-ttu-id="547c7-206">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="547c7-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="547c7-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="547c7-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="547c7-208">String</span><span class="sxs-lookup"><span data-stu-id="547c7-208">String</span></span>|<span data-ttu-id="547c7-209">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="547c7-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="547c7-210">Связи</span><span class="sxs-lookup"><span data-stu-id="547c7-210">Relationships</span></span>
<span data-ttu-id="547c7-211">Нет</span><span class="sxs-lookup"><span data-stu-id="547c7-211">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="547c7-212">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="547c7-212">JSON Representation</span></span>
<span data-ttu-id="547c7-213">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="547c7-213">Here is a JSON representation of the resource.</span></span>
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




