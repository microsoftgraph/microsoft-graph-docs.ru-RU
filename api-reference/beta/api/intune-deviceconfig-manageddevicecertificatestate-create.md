---
title: Создание managedDeviceCertificateState
description: Создайте новый объект managedDeviceCertificateState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: abdf3fd3948efd592f7e6dffbb3b524189b78bff
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666333"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="68e61-103">Создание managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="68e61-103">Create managedDeviceCertificateState</span></span>

<span data-ttu-id="68e61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68e61-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68e61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68e61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68e61-107">Создайте новый [объект managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)</span><span class="sxs-lookup"><span data-stu-id="68e61-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68e61-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68e61-108">Prerequisites</span></span>
<span data-ttu-id="68e61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68e61-111">Permission type</span></span>|<span data-ttu-id="68e61-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68e61-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68e61-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68e61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68e61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68e61-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68e61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68e61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68e61-116">Not supported.</span></span>|
|<span data-ttu-id="68e61-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="68e61-117">Application</span></span>|<span data-ttu-id="68e61-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e61-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68e61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68e61-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates
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

## <a name="request-headers"></a><span data-ttu-id="68e61-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68e61-120">Request headers</span></span>
|<span data-ttu-id="68e61-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68e61-121">Header</span></span>|<span data-ttu-id="68e61-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68e61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68e61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68e61-123">Authorization</span></span>|<span data-ttu-id="68e61-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68e61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68e61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68e61-125">Accept</span></span>|<span data-ttu-id="68e61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68e61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68e61-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68e61-127">Request body</span></span>
<span data-ttu-id="68e61-128">В теле запроса поставляем представление JSON для объекта managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="68e61-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="68e61-129">В следующей таблице показаны свойства, необходимые при создании managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="68e61-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="68e61-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68e61-130">Property</span></span>|<span data-ttu-id="68e61-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68e61-131">Type</span></span>|<span data-ttu-id="68e61-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68e61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68e61-133">id</span><span class="sxs-lookup"><span data-stu-id="68e61-133">id</span></span>|<span data-ttu-id="68e61-134">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-134">String</span></span>|<span data-ttu-id="68e61-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68e61-135">Key of the entity.</span></span>|
|<span data-ttu-id="68e61-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="68e61-136">devicePlatform</span></span>|[<span data-ttu-id="68e61-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="68e61-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="68e61-138">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="68e61-138">Device platform.</span></span> <span data-ttu-id="68e61-139">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.</span><span class="sxs-lookup"><span data-stu-id="68e61-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.</span></span>|
|<span data-ttu-id="68e61-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="68e61-140">certificateKeyUsage</span></span>|[<span data-ttu-id="68e61-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="68e61-141">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="68e61-142">Использование ключей.</span><span class="sxs-lookup"><span data-stu-id="68e61-142">Key usage.</span></span> <span data-ttu-id="68e61-143">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="68e61-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="68e61-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="68e61-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="68e61-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="68e61-145">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="68e61-146">Единицы периода действия.</span><span class="sxs-lookup"><span data-stu-id="68e61-146">Validity period units.</span></span> <span data-ttu-id="68e61-147">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="68e61-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="68e61-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="68e61-148">certificateIssuanceState</span></span>|[<span data-ttu-id="68e61-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="68e61-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="68e61-150">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="68e61-150">Issuance State.</span></span> <span data-ttu-id="68e61-151">Возможные значения: `unknown` `challengeIssued` , , `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` , `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` .</span><span class="sxs-lookup"><span data-stu-id="68e61-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="68e61-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="68e61-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="68e61-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="68e61-153">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="68e61-154">Ключевой служба хранилища поставщик.</span><span class="sxs-lookup"><span data-stu-id="68e61-154">Key Storage Provider.</span></span> <span data-ttu-id="68e61-155">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="68e61-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="68e61-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="68e61-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="68e61-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="68e61-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="68e61-158">Формат имен субъекта.</span><span class="sxs-lookup"><span data-stu-id="68e61-158">Subject name format.</span></span> <span data-ttu-id="68e61-159">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="68e61-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="68e61-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="68e61-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="68e61-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="68e61-161">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="68e61-162">Тема альтернативного формата имен.</span><span class="sxs-lookup"><span data-stu-id="68e61-162">Subject alternative name format.</span></span> <span data-ttu-id="68e61-163">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="68e61-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="68e61-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="68e61-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="68e61-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="68e61-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="68e61-166">Отзови статус.</span><span class="sxs-lookup"><span data-stu-id="68e61-166">Revoke status.</span></span> <span data-ttu-id="68e61-167">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="68e61-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="68e61-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="68e61-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="68e61-169">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-169">String</span></span>|<span data-ttu-id="68e61-170">Имя отображения профиля сертификата</span><span class="sxs-lookup"><span data-stu-id="68e61-170">Certificate profile display name</span></span>|
|<span data-ttu-id="68e61-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="68e61-171">deviceDisplayName</span></span>|<span data-ttu-id="68e61-172">String</span><span class="sxs-lookup"><span data-stu-id="68e61-172">String</span></span>|<span data-ttu-id="68e61-173">Имя отображения устройства</span><span class="sxs-lookup"><span data-stu-id="68e61-173">Device display name</span></span>|
|<span data-ttu-id="68e61-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="68e61-174">userDisplayName</span></span>|<span data-ttu-id="68e61-175">String</span><span class="sxs-lookup"><span data-stu-id="68e61-175">String</span></span>|<span data-ttu-id="68e61-176">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="68e61-176">User display name</span></span>|
|<span data-ttu-id="68e61-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="68e61-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="68e61-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e61-178">DateTimeOffset</span></span>|<span data-ttu-id="68e61-179">Дата истечения срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="68e61-179">Certificate expiry date</span></span>|
|<span data-ttu-id="68e61-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="68e61-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="68e61-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e61-181">DateTimeOffset</span></span>|<span data-ttu-id="68e61-182">Изменение состояния последнего сертификата</span><span class="sxs-lookup"><span data-stu-id="68e61-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="68e61-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="68e61-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="68e61-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e61-184">DateTimeOffset</span></span>|<span data-ttu-id="68e61-185">Изменение состояния последнего сертификата</span><span class="sxs-lookup"><span data-stu-id="68e61-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="68e61-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="68e61-186">certificateIssuer</span></span>|<span data-ttu-id="68e61-187">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-187">String</span></span>|<span data-ttu-id="68e61-188">Издатель</span><span class="sxs-lookup"><span data-stu-id="68e61-188">Issuer</span></span>|
|<span data-ttu-id="68e61-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="68e61-189">certificateThumbprint</span></span>|<span data-ttu-id="68e61-190">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-190">String</span></span>|<span data-ttu-id="68e61-191">Thumbprint</span><span class="sxs-lookup"><span data-stu-id="68e61-191">Thumbprint</span></span>|
|<span data-ttu-id="68e61-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="68e61-192">certificateSerialNumber</span></span>|<span data-ttu-id="68e61-193">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-193">String</span></span>|<span data-ttu-id="68e61-194">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="68e61-194">Serial number</span></span>|
|<span data-ttu-id="68e61-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="68e61-195">certificateKeyLength</span></span>|<span data-ttu-id="68e61-196">Int32</span><span class="sxs-lookup"><span data-stu-id="68e61-196">Int32</span></span>|<span data-ttu-id="68e61-197">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="68e61-197">Key length</span></span>|
|<span data-ttu-id="68e61-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="68e61-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="68e61-199">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-199">String</span></span>|<span data-ttu-id="68e61-200">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="68e61-200">Extended key usage</span></span>|
|<span data-ttu-id="68e61-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="68e61-201">certificateValidityPeriod</span></span>|<span data-ttu-id="68e61-202">Int32</span><span class="sxs-lookup"><span data-stu-id="68e61-202">Int32</span></span>|<span data-ttu-id="68e61-203">Срок действия</span><span class="sxs-lookup"><span data-stu-id="68e61-203">Validity period</span></span>|
|<span data-ttu-id="68e61-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="68e61-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="68e61-205">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-205">String</span></span>|<span data-ttu-id="68e61-206">Строка формата subject name для пользовательских форматов имен субъекта</span><span class="sxs-lookup"><span data-stu-id="68e61-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="68e61-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="68e61-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="68e61-208">Строка</span><span class="sxs-lookup"><span data-stu-id="68e61-208">String</span></span>|<span data-ttu-id="68e61-209">Строка альтернативного формата имен для настраиваемого формата</span><span class="sxs-lookup"><span data-stu-id="68e61-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="68e61-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="68e61-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="68e61-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68e61-211">DateTimeOffset</span></span>|<span data-ttu-id="68e61-212">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="68e61-212">Issuance date</span></span>|
|<span data-ttu-id="68e61-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="68e61-213">certificateErrorCode</span></span>|<span data-ttu-id="68e61-214">Int32</span><span class="sxs-lookup"><span data-stu-id="68e61-214">Int32</span></span>|<span data-ttu-id="68e61-215">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="68e61-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="68e61-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e61-216">Response</span></span>
<span data-ttu-id="68e61-217">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68e61-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e61-218">Пример</span><span class="sxs-lookup"><span data-stu-id="68e61-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="68e61-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="68e61-219">Request</span></span>
<span data-ttu-id="68e61-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68e61-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68e61-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="68e61-221">Response</span></span>
<span data-ttu-id="68e61-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68e61-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




