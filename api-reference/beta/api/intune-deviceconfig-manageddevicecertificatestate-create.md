---
title: Создание Манажеддевицецертификатестате
description: Создание нового объекта Манажеддевицецертификатестате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcacd051950270ba26088e2433128086f9fc2d42
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42743347"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="7a2ed-103">Создание Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="7a2ed-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="7a2ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a2ed-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a2ed-106">Создание нового объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="7a2ed-106">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a2ed-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a2ed-107">Prerequisites</span></span>
<span data-ttu-id="7a2ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a2ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a2ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a2ed-110">Permission type</span></span>|<span data-ttu-id="7a2ed-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a2ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a2ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a2ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a2ed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a2ed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a2ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a2ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a2ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-115">Not supported.</span></span>|
|<span data-ttu-id="7a2ed-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7a2ed-116">Application</span></span>|<span data-ttu-id="7a2ed-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a2ed-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a2ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a2ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="7a2ed-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7a2ed-119">Request headers</span></span>
|<span data-ttu-id="7a2ed-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a2ed-120">Header</span></span>|<span data-ttu-id="7a2ed-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7a2ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a2ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a2ed-122">Authorization</span></span>|<span data-ttu-id="7a2ed-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a2ed-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7a2ed-124">Accept</span></span>|<span data-ttu-id="7a2ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7a2ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a2ed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a2ed-126">Request body</span></span>
<span data-ttu-id="7a2ed-127">В тексте запроса добавьте представление объекта Манажеддевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-127">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="7a2ed-128">В следующей таблице приведены свойства, необходимые при создании Манажеддевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-128">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="7a2ed-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a2ed-129">Property</span></span>|<span data-ttu-id="7a2ed-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7a2ed-130">Type</span></span>|<span data-ttu-id="7a2ed-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7a2ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a2ed-132">id</span><span class="sxs-lookup"><span data-stu-id="7a2ed-132">id</span></span>|<span data-ttu-id="7a2ed-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7a2ed-133">String</span></span>|<span data-ttu-id="7a2ed-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-134">Key of the entity.</span></span>|
|<span data-ttu-id="7a2ed-135">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="7a2ed-135">devicePlatform</span></span>|[<span data-ttu-id="7a2ed-136">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="7a2ed-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="7a2ed-137">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-137">Device platform.</span></span> <span data-ttu-id="7a2ed-138">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="7a2ed-139">цертификатекэйусаже</span><span class="sxs-lookup"><span data-stu-id="7a2ed-139">certificateKeyUsage</span></span>|[<span data-ttu-id="7a2ed-140">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="7a2ed-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7a2ed-141">Использование ключа.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-141">Key usage.</span></span> <span data-ttu-id="7a2ed-142">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7a2ed-143">цертификатевалидитипериодунитс</span><span class="sxs-lookup"><span data-stu-id="7a2ed-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="7a2ed-144">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7a2ed-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7a2ed-145">Единицы срока действия.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-145">Validity period units.</span></span> <span data-ttu-id="7a2ed-146">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7a2ed-147">цертификатеиссуанцестате</span><span class="sxs-lookup"><span data-stu-id="7a2ed-147">certificateIssuanceState</span></span>|[<span data-ttu-id="7a2ed-148">цертификатеиссуанцестатес</span><span class="sxs-lookup"><span data-stu-id="7a2ed-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="7a2ed-149">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-149">Issuance State.</span></span> <span data-ttu-id="7a2ed-150">Возможные `unknown`значения:, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested`,,,,,,, `enrollmentSucceeded`,,,,,,,,,,,,,,,,,,. `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending`</span><span class="sxs-lookup"><span data-stu-id="7a2ed-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="7a2ed-151">цертификатекэйсторажепровидер</span><span class="sxs-lookup"><span data-stu-id="7a2ed-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="7a2ed-152">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="7a2ed-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="7a2ed-153">Поставщик хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-153">Key Storage Provider.</span></span> <span data-ttu-id="7a2ed-154">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="7a2ed-155">цертификатесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="7a2ed-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="7a2ed-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7a2ed-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="7a2ed-157">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-157">Subject name format.</span></span> <span data-ttu-id="7a2ed-158">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="7a2ed-159">цертификатесубжекталтернативенамеформат</span><span class="sxs-lookup"><span data-stu-id="7a2ed-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="7a2ed-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7a2ed-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7a2ed-161">Формат альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-161">Subject alternative name format.</span></span> <span data-ttu-id="7a2ed-162">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7a2ed-163">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="7a2ed-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="7a2ed-164">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="7a2ed-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="7a2ed-165">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-165">Revoke status.</span></span> <span data-ttu-id="7a2ed-166">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="7a2ed-167">цертификатепрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="7a2ed-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="7a2ed-168">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-168">String</span></span>|<span data-ttu-id="7a2ed-169">Отображаемое имя профиля сертификата</span><span class="sxs-lookup"><span data-stu-id="7a2ed-169">Certificate profile display name</span></span>|
|<span data-ttu-id="7a2ed-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7a2ed-170">deviceDisplayName</span></span>|<span data-ttu-id="7a2ed-171">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-171">String</span></span>|<span data-ttu-id="7a2ed-172">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="7a2ed-172">Device display name</span></span>|
|<span data-ttu-id="7a2ed-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7a2ed-173">userDisplayName</span></span>|<span data-ttu-id="7a2ed-174">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-174">String</span></span>|<span data-ttu-id="7a2ed-175">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="7a2ed-175">User display name</span></span>|
|<span data-ttu-id="7a2ed-176">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="7a2ed-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="7a2ed-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a2ed-177">DateTimeOffset</span></span>|<span data-ttu-id="7a2ed-178">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="7a2ed-178">Certificate expiry date</span></span>|
|<span data-ttu-id="7a2ed-179">цертификателастиссуанцестатечанжеддатетиме</span><span class="sxs-lookup"><span data-stu-id="7a2ed-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="7a2ed-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a2ed-180">DateTimeOffset</span></span>|<span data-ttu-id="7a2ed-181">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="7a2ed-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="7a2ed-182">ластцертификатестатечанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="7a2ed-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="7a2ed-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a2ed-183">DateTimeOffset</span></span>|<span data-ttu-id="7a2ed-184">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="7a2ed-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="7a2ed-185">цертификатеиссуер</span><span class="sxs-lookup"><span data-stu-id="7a2ed-185">certificateIssuer</span></span>|<span data-ttu-id="7a2ed-186">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-186">String</span></span>|<span data-ttu-id="7a2ed-187">Издатель</span><span class="sxs-lookup"><span data-stu-id="7a2ed-187">Issuer</span></span>|
|<span data-ttu-id="7a2ed-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="7a2ed-188">certificateThumbprint</span></span>|<span data-ttu-id="7a2ed-189">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-189">String</span></span>|<span data-ttu-id="7a2ed-190">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="7a2ed-190">Thumbprint</span></span>|
|<span data-ttu-id="7a2ed-191">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="7a2ed-191">certificateSerialNumber</span></span>|<span data-ttu-id="7a2ed-192">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-192">String</span></span>|<span data-ttu-id="7a2ed-193">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="7a2ed-193">Serial number</span></span>|
|<span data-ttu-id="7a2ed-194">цертификатекэйленгс</span><span class="sxs-lookup"><span data-stu-id="7a2ed-194">certificateKeyLength</span></span>|<span data-ttu-id="7a2ed-195">Int32</span><span class="sxs-lookup"><span data-stu-id="7a2ed-195">Int32</span></span>|<span data-ttu-id="7a2ed-196">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="7a2ed-196">Key length</span></span>|
|<span data-ttu-id="7a2ed-197">цертификатинханцедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="7a2ed-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="7a2ed-198">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-198">String</span></span>|<span data-ttu-id="7a2ed-199">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="7a2ed-199">Extended key usage</span></span>|
|<span data-ttu-id="7a2ed-200">цертификатевалидитипериод</span><span class="sxs-lookup"><span data-stu-id="7a2ed-200">certificateValidityPeriod</span></span>|<span data-ttu-id="7a2ed-201">Int32</span><span class="sxs-lookup"><span data-stu-id="7a2ed-201">Int32</span></span>|<span data-ttu-id="7a2ed-202">Срок действия</span><span class="sxs-lookup"><span data-stu-id="7a2ed-202">Validity period</span></span>|
|<span data-ttu-id="7a2ed-203">цертификатесубжектнамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="7a2ed-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="7a2ed-204">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-204">String</span></span>|<span data-ttu-id="7a2ed-205">Строка формата имени субъекта для пользовательских форматов имен субъектов</span><span class="sxs-lookup"><span data-stu-id="7a2ed-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="7a2ed-206">цертификатесубжекталтернативенамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="7a2ed-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7a2ed-207">String</span><span class="sxs-lookup"><span data-stu-id="7a2ed-207">String</span></span>|<span data-ttu-id="7a2ed-208">Строка формата альтернативного имени субъекта для пользовательских форматов</span><span class="sxs-lookup"><span data-stu-id="7a2ed-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="7a2ed-209">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="7a2ed-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="7a2ed-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a2ed-210">DateTimeOffset</span></span>|<span data-ttu-id="7a2ed-211">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="7a2ed-211">Issuance date</span></span>|
|<span data-ttu-id="7a2ed-212">цертификатирроркоде</span><span class="sxs-lookup"><span data-stu-id="7a2ed-212">certificateErrorCode</span></span>|<span data-ttu-id="7a2ed-213">Int32</span><span class="sxs-lookup"><span data-stu-id="7a2ed-213">Int32</span></span>|<span data-ttu-id="7a2ed-214">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="7a2ed-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="7a2ed-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a2ed-215">Response</span></span>
<span data-ttu-id="7a2ed-216">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-216">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a2ed-217">Пример</span><span class="sxs-lookup"><span data-stu-id="7a2ed-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a2ed-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a2ed-218">Request</span></span>
<span data-ttu-id="7a2ed-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1517

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```

### <a name="response"></a><span data-ttu-id="7a2ed-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a2ed-220">Response</span></span>
<span data-ttu-id="7a2ed-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a2ed-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1566

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```




