---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2a4ab6f846b5172ca91f191f32392b915df116e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030809"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="09627-103">Тип ресурса deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="09627-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="09627-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09627-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09627-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="09627-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="09627-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="09627-106">Properties</span></span>
|<span data-ttu-id="09627-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="09627-107">Property</span></span>|<span data-ttu-id="09627-108">Тип</span><span class="sxs-lookup"><span data-stu-id="09627-108">Type</span></span>|<span data-ttu-id="09627-109">Описание</span><span class="sxs-lookup"><span data-stu-id="09627-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09627-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="09627-110">lastUpdateDateTime</span></span>|<span data-ttu-id="09627-111">String</span><span class="sxs-lookup"><span data-stu-id="09627-111">String</span></span>|<span data-ttu-id="09627-112">Метка времени последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="09627-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="09627-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="09627-113">contentNamespaceUrl</span></span>|<span data-ttu-id="09627-114">String</span><span class="sxs-lookup"><span data-stu-id="09627-114">String</span></span>|<span data-ttu-id="09627-115">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="09627-115">The DHA report version.</span></span> <span data-ttu-id="09627-116">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="09627-116">(Namespace version)</span></span>|
|<span data-ttu-id="09627-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="09627-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="09627-118">String</span><span class="sxs-lookup"><span data-stu-id="09627-118">String</span></span>|<span data-ttu-id="09627-119">Версия отчета DHA</span><span class="sxs-lookup"><span data-stu-id="09627-119">The DHA report version.</span></span> <span data-ttu-id="09627-120">(версия пространства имен).</span><span class="sxs-lookup"><span data-stu-id="09627-120">(Namespace version)</span></span>|
|<span data-ttu-id="09627-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="09627-121">contentVersion</span></span>|<span data-ttu-id="09627-122">String</span><span class="sxs-lookup"><span data-stu-id="09627-122">String</span></span>|<span data-ttu-id="09627-123">Версия схемы состояния HealthAttestation.</span><span class="sxs-lookup"><span data-stu-id="09627-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="09627-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="09627-124">issuedDateTime</span></span>|<span data-ttu-id="09627-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09627-125">DateTimeOffset</span></span>|<span data-ttu-id="09627-126">Дата и время оценки устройства или его публикации для MDM.</span><span class="sxs-lookup"><span data-stu-id="09627-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="09627-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="09627-127">attestationIdentityKey</span></span>|<span data-ttu-id="09627-128">String</span><span class="sxs-lookup"><span data-stu-id="09627-128">String</span></span>|<span data-ttu-id="09627-129">Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).</span><span class="sxs-lookup"><span data-stu-id="09627-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="09627-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="09627-130">resetCount</span></span>|<span data-ttu-id="09627-131">Int64</span><span class="sxs-lookup"><span data-stu-id="09627-131">Int64</span></span>|<span data-ttu-id="09627-132">Количество переходов компьютера в режим гибернации или возобновлений его работы.</span><span class="sxs-lookup"><span data-stu-id="09627-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="09627-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="09627-133">restartCount</span></span>|<span data-ttu-id="09627-134">Int64</span><span class="sxs-lookup"><span data-stu-id="09627-134">Int64</span></span>|<span data-ttu-id="09627-135">Количество перезапусков компьютера.</span><span class="sxs-lookup"><span data-stu-id="09627-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="09627-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="09627-136">dataExcutionPolicy</span></span>|<span data-ttu-id="09627-137">String</span><span class="sxs-lookup"><span data-stu-id="09627-137">String</span></span>|<span data-ttu-id="09627-138">Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти.</span><span class="sxs-lookup"><span data-stu-id="09627-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="09627-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="09627-139">bitLockerStatus</span></span>|<span data-ttu-id="09627-140">String</span><span class="sxs-lookup"><span data-stu-id="09627-140">String</span></span>|<span data-ttu-id="09627-141">Включение или выключение шифрования диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="09627-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="09627-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="09627-142">bootManagerVersion</span></span>|<span data-ttu-id="09627-143">String</span><span class="sxs-lookup"><span data-stu-id="09627-143">String</span></span>|<span data-ttu-id="09627-144">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="09627-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="09627-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="09627-146">String</span><span class="sxs-lookup"><span data-stu-id="09627-146">String</span></span>|<span data-ttu-id="09627-147">Версия диспетчера загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="09627-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="09627-148">secureBoot</span></span>|<span data-ttu-id="09627-149">String</span><span class="sxs-lookup"><span data-stu-id="09627-149">String</span></span>|<span data-ttu-id="09627-150">Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.</span><span class="sxs-lookup"><span data-stu-id="09627-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="09627-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="09627-151">bootDebugging</span></span>|<span data-ttu-id="09627-152">String</span><span class="sxs-lookup"><span data-stu-id="09627-152">String</span></span>|<span data-ttu-id="09627-153">Если включено свойство bootDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="09627-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="09627-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="09627-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="09627-155">String</span><span class="sxs-lookup"><span data-stu-id="09627-155">String</span></span>|<span data-ttu-id="09627-156">Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.</span><span class="sxs-lookup"><span data-stu-id="09627-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="09627-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="09627-157">codeIntegrity</span></span>|<span data-ttu-id="09627-158">String</span><span class="sxs-lookup"><span data-stu-id="09627-158">String</span></span>| <span data-ttu-id="09627-159">Если включена целостность кода, выполняется только код, который прошел проверку на целостность.</span><span class="sxs-lookup"><span data-stu-id="09627-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="09627-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="09627-160">testSigning</span></span>|<span data-ttu-id="09627-161">String</span><span class="sxs-lookup"><span data-stu-id="09627-161">String</span></span>|<span data-ttu-id="09627-162">Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="09627-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="09627-163">safeMode</span></span>|<span data-ttu-id="09627-164">String</span><span class="sxs-lookup"><span data-stu-id="09627-164">String</span></span>|<span data-ttu-id="09627-165">Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.</span><span class="sxs-lookup"><span data-stu-id="09627-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="09627-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="09627-166">windowsPE</span></span>|<span data-ttu-id="09627-167">String</span><span class="sxs-lookup"><span data-stu-id="09627-167">String</span></span>|<span data-ttu-id="09627-168">Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.</span><span class="sxs-lookup"><span data-stu-id="09627-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="09627-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="09627-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="09627-170">String</span><span class="sxs-lookup"><span data-stu-id="09627-170">String</span></span>|<span data-ttu-id="09627-171">Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.</span><span class="sxs-lookup"><span data-stu-id="09627-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="09627-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="09627-172">virtualSecureMode</span></span>|<span data-ttu-id="09627-173">String</span><span class="sxs-lookup"><span data-stu-id="09627-173">String</span></span>|<span data-ttu-id="09627-174">VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.</span><span class="sxs-lookup"><span data-stu-id="09627-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="09627-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="09627-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="09627-176">String</span><span class="sxs-lookup"><span data-stu-id="09627-176">String</span></span>|<span data-ttu-id="09627-177">Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).</span><span class="sxs-lookup"><span data-stu-id="09627-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="09627-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="09627-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="09627-179">String</span><span class="sxs-lookup"><span data-stu-id="09627-179">String</span></span>|<span data-ttu-id="09627-180">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="09627-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="09627-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="09627-182">String</span><span class="sxs-lookup"><span data-stu-id="09627-182">String</span></span>|<span data-ttu-id="09627-183">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="09627-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="09627-184">tpmVersion</span></span>|<span data-ttu-id="09627-185">String</span><span class="sxs-lookup"><span data-stu-id="09627-185">String</span></span>|<span data-ttu-id="09627-186">Номер версии системы безопасности для приложения загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="09627-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="09627-187">pcr0</span></span>|<span data-ttu-id="09627-188">String</span><span class="sxs-lookup"><span data-stu-id="09627-188">String</span></span>|<span data-ttu-id="09627-189">Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]</span><span class="sxs-lookup"><span data-stu-id="09627-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="09627-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="09627-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="09627-191">String</span><span class="sxs-lookup"><span data-stu-id="09627-191">String</span></span>|<span data-ttu-id="09627-192">Отпечаток пользовательской политики настройки безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="09627-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="09627-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="09627-194">String</span><span class="sxs-lookup"><span data-stu-id="09627-194">String</span></span>|<span data-ttu-id="09627-195">Политика целостности кода, которая управляет безопасностью среды загрузки.</span><span class="sxs-lookup"><span data-stu-id="09627-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="09627-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="09627-196">bootRevisionListInfo</span></span>|<span data-ttu-id="09627-197">String</span><span class="sxs-lookup"><span data-stu-id="09627-197">String</span></span>|<span data-ttu-id="09627-198">Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="09627-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="09627-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="09627-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="09627-200">String</span><span class="sxs-lookup"><span data-stu-id="09627-200">String</span></span>|<span data-ttu-id="09627-201">Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.</span><span class="sxs-lookup"><span data-stu-id="09627-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="09627-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="09627-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="09627-203">String</span><span class="sxs-lookup"><span data-stu-id="09627-203">String</span></span>|<span data-ttu-id="09627-204">Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.</span><span class="sxs-lookup"><span data-stu-id="09627-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="09627-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="09627-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="09627-206">String</span><span class="sxs-lookup"><span data-stu-id="09627-206">String</span></span>|<span data-ttu-id="09627-207">Этот атрибут указывает, поддерживается ли DHA для устройства.</span><span class="sxs-lookup"><span data-stu-id="09627-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="09627-208">Отношения</span><span class="sxs-lookup"><span data-stu-id="09627-208">Relationships</span></span>
<span data-ttu-id="09627-209">Нет</span><span class="sxs-lookup"><span data-stu-id="09627-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09627-210">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09627-210">JSON Representation</span></span>
<span data-ttu-id="09627-211">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09627-211">Here is a JSON representation of the resource.</span></span>
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



