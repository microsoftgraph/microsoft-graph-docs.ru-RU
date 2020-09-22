---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a4e9b7e916f33bc6c472c5c90bd440a246f7016
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091203"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="492b2-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="492b2-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="492b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="492b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="492b2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="492b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="492b2-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="492b2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="492b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="492b2-107">Properties</span></span>
|<span data-ttu-id="492b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="492b2-108">Property</span></span>|<span data-ttu-id="492b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="492b2-109">Type</span></span>|<span data-ttu-id="492b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="492b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="492b2-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="492b2-111">lastUpdateDateTime</span></span>|<span data-ttu-id="492b2-112">String</span><span class="sxs-lookup"><span data-stu-id="492b2-112">String</span></span>|<span data-ttu-id="492b2-113">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="492b2-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="492b2-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="492b2-114">contentNamespaceUrl</span></span>|<span data-ttu-id="492b2-115">String</span><span class="sxs-lookup"><span data-stu-id="492b2-115">String</span></span>|<span data-ttu-id="492b2-116">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="492b2-116">The DHA report version.</span></span> <span data-ttu-id="492b2-117">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="492b2-117">(Namespace version)</span></span>|
|<span data-ttu-id="492b2-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="492b2-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="492b2-119">String</span><span class="sxs-lookup"><span data-stu-id="492b2-119">String</span></span>|<span data-ttu-id="492b2-120">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="492b2-120">The DHA report version.</span></span> <span data-ttu-id="492b2-121">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="492b2-121">(Namespace version)</span></span>|
|<span data-ttu-id="492b2-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-122">contentVersion</span></span>|<span data-ttu-id="492b2-123">String</span><span class="sxs-lookup"><span data-stu-id="492b2-123">String</span></span>|<span data-ttu-id="492b2-124">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="492b2-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="492b2-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="492b2-125">issuedDateTime</span></span>|<span data-ttu-id="492b2-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="492b2-126">DateTimeOffset</span></span>|<span data-ttu-id="492b2-127">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="492b2-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="492b2-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="492b2-128">attestationIdentityKey</span></span>|<span data-ttu-id="492b2-129">String</span><span class="sxs-lookup"><span data-stu-id="492b2-129">String</span></span>|<span data-ttu-id="492b2-130">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="492b2-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="492b2-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="492b2-131">resetCount</span></span>|<span data-ttu-id="492b2-132">Int64</span><span class="sxs-lookup"><span data-stu-id="492b2-132">Int64</span></span>|<span data-ttu-id="492b2-133">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="492b2-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="492b2-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="492b2-134">restartCount</span></span>|<span data-ttu-id="492b2-135">Int64</span><span class="sxs-lookup"><span data-stu-id="492b2-135">Int64</span></span>|<span data-ttu-id="492b2-136">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="492b2-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="492b2-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="492b2-137">dataExcutionPolicy</span></span>|<span data-ttu-id="492b2-138">String</span><span class="sxs-lookup"><span data-stu-id="492b2-138">String</span></span>|<span data-ttu-id="492b2-139">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="492b2-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="492b2-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="492b2-140">bitLockerStatus</span></span>|<span data-ttu-id="492b2-141">String</span><span class="sxs-lookup"><span data-stu-id="492b2-141">String</span></span>|<span data-ttu-id="492b2-142">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="492b2-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="492b2-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-143">bootManagerVersion</span></span>|<span data-ttu-id="492b2-144">String</span><span class="sxs-lookup"><span data-stu-id="492b2-144">String</span></span>|<span data-ttu-id="492b2-145">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="492b2-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="492b2-147">String</span><span class="sxs-lookup"><span data-stu-id="492b2-147">String</span></span>|<span data-ttu-id="492b2-148">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="492b2-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="492b2-149">secureBoot</span></span>|<span data-ttu-id="492b2-150">String</span><span class="sxs-lookup"><span data-stu-id="492b2-150">String</span></span>|<span data-ttu-id="492b2-151">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="492b2-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="492b2-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="492b2-152">bootDebugging</span></span>|<span data-ttu-id="492b2-153">String</span><span class="sxs-lookup"><span data-stu-id="492b2-153">String</span></span>|<span data-ttu-id="492b2-154">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="492b2-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="492b2-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="492b2-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="492b2-156">String</span><span class="sxs-lookup"><span data-stu-id="492b2-156">String</span></span>|<span data-ttu-id="492b2-157">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="492b2-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="492b2-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="492b2-158">codeIntegrity</span></span>|<span data-ttu-id="492b2-159">String</span><span class="sxs-lookup"><span data-stu-id="492b2-159">String</span></span>| <span data-ttu-id="492b2-160">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="492b2-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="492b2-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="492b2-161">testSigning</span></span>|<span data-ttu-id="492b2-162">String</span><span class="sxs-lookup"><span data-stu-id="492b2-162">String</span></span>|<span data-ttu-id="492b2-163">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="492b2-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="492b2-164">safeMode</span></span>|<span data-ttu-id="492b2-165">String</span><span class="sxs-lookup"><span data-stu-id="492b2-165">String</span></span>|<span data-ttu-id="492b2-166">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="492b2-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="492b2-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="492b2-167">windowsPE</span></span>|<span data-ttu-id="492b2-168">String</span><span class="sxs-lookup"><span data-stu-id="492b2-168">String</span></span>|<span data-ttu-id="492b2-169">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="492b2-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="492b2-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="492b2-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="492b2-171">String</span><span class="sxs-lookup"><span data-stu-id="492b2-171">String</span></span>|<span data-ttu-id="492b2-172">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="492b2-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="492b2-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="492b2-173">virtualSecureMode</span></span>|<span data-ttu-id="492b2-174">String</span><span class="sxs-lookup"><span data-stu-id="492b2-174">String</span></span>|<span data-ttu-id="492b2-175">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="492b2-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="492b2-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="492b2-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="492b2-177">String</span><span class="sxs-lookup"><span data-stu-id="492b2-177">String</span></span>|<span data-ttu-id="492b2-178">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="492b2-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="492b2-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="492b2-180">String</span><span class="sxs-lookup"><span data-stu-id="492b2-180">String</span></span>|<span data-ttu-id="492b2-181">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="492b2-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="492b2-183">String</span><span class="sxs-lookup"><span data-stu-id="492b2-183">String</span></span>|<span data-ttu-id="492b2-184">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="492b2-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="492b2-185">tpmVersion</span></span>|<span data-ttu-id="492b2-186">String</span><span class="sxs-lookup"><span data-stu-id="492b2-186">String</span></span>|<span data-ttu-id="492b2-187">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="492b2-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="492b2-188">pcr0</span></span>|<span data-ttu-id="492b2-189">String</span><span class="sxs-lookup"><span data-stu-id="492b2-189">String</span></span>|<span data-ttu-id="492b2-190">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="492b2-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="492b2-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="492b2-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="492b2-192">String</span><span class="sxs-lookup"><span data-stu-id="492b2-192">String</span></span>|<span data-ttu-id="492b2-193">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="492b2-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="492b2-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="492b2-195">String</span><span class="sxs-lookup"><span data-stu-id="492b2-195">String</span></span>|<span data-ttu-id="492b2-196">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="492b2-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="492b2-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="492b2-197">bootRevisionListInfo</span></span>|<span data-ttu-id="492b2-198">String</span><span class="sxs-lookup"><span data-stu-id="492b2-198">String</span></span>|<span data-ttu-id="492b2-199">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="492b2-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="492b2-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="492b2-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="492b2-201">String</span><span class="sxs-lookup"><span data-stu-id="492b2-201">String</span></span>|<span data-ttu-id="492b2-202">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="492b2-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="492b2-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="492b2-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="492b2-204">String</span><span class="sxs-lookup"><span data-stu-id="492b2-204">String</span></span>|<span data-ttu-id="492b2-205">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="492b2-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="492b2-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="492b2-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="492b2-207">String</span><span class="sxs-lookup"><span data-stu-id="492b2-207">String</span></span>|<span data-ttu-id="492b2-208">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="492b2-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="492b2-209">Связи</span><span class="sxs-lookup"><span data-stu-id="492b2-209">Relationships</span></span>
<span data-ttu-id="492b2-210">Нет</span><span class="sxs-lookup"><span data-stu-id="492b2-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="492b2-211">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="492b2-211">JSON Representation</span></span>
<span data-ttu-id="492b2-212">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="492b2-212">Here is a JSON representation of the resource.</span></span>
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









