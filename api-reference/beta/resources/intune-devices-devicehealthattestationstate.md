---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a38fb9959e555dfd24796273c6acd29ff869ab4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320761"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="50a9a-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="50a9a-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="50a9a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50a9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50a9a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50a9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50a9a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="50a9a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="50a9a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50a9a-107">Properties</span></span>
|<span data-ttu-id="50a9a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50a9a-108">Property</span></span>|<span data-ttu-id="50a9a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50a9a-109">Type</span></span>|<span data-ttu-id="50a9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50a9a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a9a-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="50a9a-111">lastUpdateDateTime</span></span>|<span data-ttu-id="50a9a-112">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-112">String</span></span>|<span data-ttu-id="50a9a-113">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="50a9a-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="50a9a-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="50a9a-114">contentNamespaceUrl</span></span>|<span data-ttu-id="50a9a-115">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-115">String</span></span>|<span data-ttu-id="50a9a-116">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="50a9a-116">The DHA report version.</span></span> <span data-ttu-id="50a9a-117">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="50a9a-117">(Namespace version)</span></span>|
|<span data-ttu-id="50a9a-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="50a9a-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="50a9a-119">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-119">String</span></span>|<span data-ttu-id="50a9a-120">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="50a9a-120">The DHA report version.</span></span> <span data-ttu-id="50a9a-121">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="50a9a-121">(Namespace version)</span></span>|
|<span data-ttu-id="50a9a-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-122">contentVersion</span></span>|<span data-ttu-id="50a9a-123">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-123">String</span></span>|<span data-ttu-id="50a9a-124">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="50a9a-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="50a9a-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="50a9a-125">issuedDateTime</span></span>|<span data-ttu-id="50a9a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50a9a-126">DateTimeOffset</span></span>|<span data-ttu-id="50a9a-127">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="50a9a-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="50a9a-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="50a9a-128">attestationIdentityKey</span></span>|<span data-ttu-id="50a9a-129">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-129">String</span></span>|<span data-ttu-id="50a9a-130">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="50a9a-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="50a9a-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="50a9a-131">resetCount</span></span>|<span data-ttu-id="50a9a-132">Int64</span><span class="sxs-lookup"><span data-stu-id="50a9a-132">Int64</span></span>|<span data-ttu-id="50a9a-133">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="50a9a-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="50a9a-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="50a9a-134">restartCount</span></span>|<span data-ttu-id="50a9a-135">Int64</span><span class="sxs-lookup"><span data-stu-id="50a9a-135">Int64</span></span>|<span data-ttu-id="50a9a-136">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="50a9a-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="50a9a-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="50a9a-137">dataExcutionPolicy</span></span>|<span data-ttu-id="50a9a-138">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-138">String</span></span>|<span data-ttu-id="50a9a-139">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="50a9a-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="50a9a-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="50a9a-140">bitLockerStatus</span></span>|<span data-ttu-id="50a9a-141">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-141">String</span></span>|<span data-ttu-id="50a9a-142">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="50a9a-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="50a9a-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-143">bootManagerVersion</span></span>|<span data-ttu-id="50a9a-144">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-144">String</span></span>|<span data-ttu-id="50a9a-145">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="50a9a-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="50a9a-147">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-147">String</span></span>|<span data-ttu-id="50a9a-148">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="50a9a-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="50a9a-149">secureBoot</span></span>|<span data-ttu-id="50a9a-150">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-150">String</span></span>|<span data-ttu-id="50a9a-151">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="50a9a-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="50a9a-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="50a9a-152">bootDebugging</span></span>|<span data-ttu-id="50a9a-153">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-153">String</span></span>|<span data-ttu-id="50a9a-154">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="50a9a-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="50a9a-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="50a9a-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="50a9a-156">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-156">String</span></span>|<span data-ttu-id="50a9a-157">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="50a9a-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="50a9a-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="50a9a-158">codeIntegrity</span></span>|<span data-ttu-id="50a9a-159">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-159">String</span></span>| <span data-ttu-id="50a9a-160">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="50a9a-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="50a9a-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="50a9a-161">testSigning</span></span>|<span data-ttu-id="50a9a-162">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-162">String</span></span>|<span data-ttu-id="50a9a-163">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="50a9a-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="50a9a-164">safeMode</span></span>|<span data-ttu-id="50a9a-165">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-165">String</span></span>|<span data-ttu-id="50a9a-166">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="50a9a-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="50a9a-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="50a9a-167">windowsPE</span></span>|<span data-ttu-id="50a9a-168">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-168">String</span></span>|<span data-ttu-id="50a9a-169">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="50a9a-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="50a9a-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="50a9a-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="50a9a-171">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-171">String</span></span>|<span data-ttu-id="50a9a-172">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="50a9a-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="50a9a-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="50a9a-173">virtualSecureMode</span></span>|<span data-ttu-id="50a9a-174">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-174">String</span></span>|<span data-ttu-id="50a9a-175">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="50a9a-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="50a9a-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="50a9a-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="50a9a-177">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-177">String</span></span>|<span data-ttu-id="50a9a-178">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="50a9a-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="50a9a-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="50a9a-180">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-180">String</span></span>|<span data-ttu-id="50a9a-181">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="50a9a-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="50a9a-183">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-183">String</span></span>|<span data-ttu-id="50a9a-184">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="50a9a-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="50a9a-185">tpmVersion</span></span>|<span data-ttu-id="50a9a-186">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-186">String</span></span>|<span data-ttu-id="50a9a-187">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="50a9a-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="50a9a-188">pcr0</span></span>|<span data-ttu-id="50a9a-189">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-189">String</span></span>|<span data-ttu-id="50a9a-190">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="50a9a-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="50a9a-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="50a9a-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="50a9a-192">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-192">String</span></span>|<span data-ttu-id="50a9a-193">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="50a9a-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="50a9a-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="50a9a-195">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-195">String</span></span>|<span data-ttu-id="50a9a-196">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="50a9a-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="50a9a-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="50a9a-197">bootRevisionListInfo</span></span>|<span data-ttu-id="50a9a-198">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-198">String</span></span>|<span data-ttu-id="50a9a-199">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="50a9a-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="50a9a-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="50a9a-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="50a9a-201">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-201">String</span></span>|<span data-ttu-id="50a9a-202">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="50a9a-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="50a9a-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="50a9a-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="50a9a-204">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-204">String</span></span>|<span data-ttu-id="50a9a-205">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="50a9a-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="50a9a-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="50a9a-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="50a9a-207">String</span><span class="sxs-lookup"><span data-stu-id="50a9a-207">String</span></span>|<span data-ttu-id="50a9a-208">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="50a9a-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="50a9a-209">Отношения</span><span class="sxs-lookup"><span data-stu-id="50a9a-209">Relationships</span></span>
<span data-ttu-id="50a9a-210">Нет</span><span class="sxs-lookup"><span data-stu-id="50a9a-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50a9a-211">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50a9a-211">JSON Representation</span></span>
<span data-ttu-id="50a9a-212">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50a9a-212">Here is a JSON representation of the resource.</span></span>
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



