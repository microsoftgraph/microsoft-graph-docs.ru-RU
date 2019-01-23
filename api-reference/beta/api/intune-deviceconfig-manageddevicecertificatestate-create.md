---
title: Создание managedDeviceCertificateState
description: Создание нового объекта managedDeviceCertificateState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8efc74f2f8abad4b659f41ac53d270af5dab2a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396317"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="e9d1a-103">Создание managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="e9d1a-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="e9d1a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9d1a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9d1a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9d1a-107">Создание нового объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="e9d1a-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9d1a-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e9d1a-108">Prerequisites</span></span>
<span data-ttu-id="e9d1a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9d1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e9d1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9d1a-111">Permission type</span></span>|<span data-ttu-id="e9d1a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9d1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9d1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9d1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9d1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9d1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9d1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9d1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9d1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-116">Not supported.</span></span>|
|<span data-ttu-id="e9d1a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9d1a-117">Application</span></span>|<span data-ttu-id="e9d1a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9d1a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9d1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="e9d1a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9d1a-120">Request headers</span></span>
|<span data-ttu-id="e9d1a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9d1a-121">Header</span></span>|<span data-ttu-id="e9d1a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9d1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9d1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9d1a-123">Authorization</span></span>|<span data-ttu-id="e9d1a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9d1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9d1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9d1a-125">Accept</span></span>|<span data-ttu-id="e9d1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9d1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9d1a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9d1a-127">Request body</span></span>
<span data-ttu-id="e9d1a-128">В тексте запроса укажите представление JSON для объекта managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="e9d1a-129">В следующей таблице показаны свойства, которые необходимы для создания managedDeviceCertificateState.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="e9d1a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9d1a-130">Property</span></span>|<span data-ttu-id="e9d1a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e9d1a-131">Type</span></span>|<span data-ttu-id="e9d1a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e9d1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9d1a-133">id</span><span class="sxs-lookup"><span data-stu-id="e9d1a-133">id</span></span>|<span data-ttu-id="e9d1a-134">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-134">String</span></span>|<span data-ttu-id="e9d1a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-135">Key of the entity.</span></span>|
|<span data-ttu-id="e9d1a-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="e9d1a-136">devicePlatform</span></span>|[<span data-ttu-id="e9d1a-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="e9d1a-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="e9d1a-138">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-138">Device platform.</span></span> <span data-ttu-id="e9d1a-139">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="e9d1a-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e9d1a-140">certificateKeyUsage</span></span>|[<span data-ttu-id="e9d1a-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="e9d1a-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e9d1a-142">Использование ключей.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-142">Key usage.</span></span> <span data-ttu-id="e9d1a-143">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e9d1a-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="e9d1a-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="e9d1a-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e9d1a-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e9d1a-146">Действия подразделений.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-146">Validity period units.</span></span> <span data-ttu-id="e9d1a-147">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e9d1a-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="e9d1a-148">certificateIssuanceState</span></span>|[<span data-ttu-id="e9d1a-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="e9d1a-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="e9d1a-150">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-150">Issuance State.</span></span> <span data-ttu-id="e9d1a-151">Возможные значения: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="e9d1a-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e9d1a-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="e9d1a-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="e9d1a-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e9d1a-154">Поставщика хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-154">Key Storage Provider.</span></span> <span data-ttu-id="e9d1a-155">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="e9d1a-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e9d1a-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="e9d1a-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e9d1a-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e9d1a-158">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-158">Subject name format.</span></span> <span data-ttu-id="e9d1a-159">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e9d1a-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="e9d1a-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="e9d1a-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e9d1a-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e9d1a-162">Формат альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-162">Subject alternative name format.</span></span> <span data-ttu-id="e9d1a-163">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e9d1a-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="e9d1a-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="e9d1a-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="e9d1a-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="e9d1a-166">Отмените состояние.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-166">Revoke status.</span></span> <span data-ttu-id="e9d1a-167">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="e9d1a-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="e9d1a-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="e9d1a-169">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-169">String</span></span>|<span data-ttu-id="e9d1a-170">Отображаемое имя сертификата профилей</span><span class="sxs-lookup"><span data-stu-id="e9d1a-170">Certificate profile display name</span></span>|
|<span data-ttu-id="e9d1a-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e9d1a-171">deviceDisplayName</span></span>|<span data-ttu-id="e9d1a-172">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-172">String</span></span>|<span data-ttu-id="e9d1a-173">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="e9d1a-173">Device display name</span></span>|
|<span data-ttu-id="e9d1a-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e9d1a-174">userDisplayName</span></span>|<span data-ttu-id="e9d1a-175">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-175">String</span></span>|<span data-ttu-id="e9d1a-176">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e9d1a-176">User display name</span></span>|
|<span data-ttu-id="e9d1a-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e9d1a-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="e9d1a-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9d1a-178">DateTimeOffset</span></span>|<span data-ttu-id="e9d1a-179">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="e9d1a-179">Certificate expiry date</span></span>|
|<span data-ttu-id="e9d1a-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9d1a-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="e9d1a-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9d1a-181">DateTimeOffset</span></span>|<span data-ttu-id="e9d1a-182">Последнее изменение состояния выдачи сертификатов</span><span class="sxs-lookup"><span data-stu-id="e9d1a-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e9d1a-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="e9d1a-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="e9d1a-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9d1a-184">DateTimeOffset</span></span>|<span data-ttu-id="e9d1a-185">Последнее изменение состояния выдачи сертификатов</span><span class="sxs-lookup"><span data-stu-id="e9d1a-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="e9d1a-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="e9d1a-186">certificateIssuer</span></span>|<span data-ttu-id="e9d1a-187">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-187">String</span></span>|<span data-ttu-id="e9d1a-188">Издателя</span><span class="sxs-lookup"><span data-stu-id="e9d1a-188">Issuer</span></span>|
|<span data-ttu-id="e9d1a-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="e9d1a-189">certificateThumbprint</span></span>|<span data-ttu-id="e9d1a-190">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-190">String</span></span>|<span data-ttu-id="e9d1a-191">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="e9d1a-191">Thumbprint</span></span>|
|<span data-ttu-id="e9d1a-192">серийный номер сертификата</span><span class="sxs-lookup"><span data-stu-id="e9d1a-192">certificateSerialNumber</span></span>|<span data-ttu-id="e9d1a-193">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-193">String</span></span>|<span data-ttu-id="e9d1a-194">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="e9d1a-194">Serial number</span></span>|
|<span data-ttu-id="e9d1a-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="e9d1a-195">certificateKeyLength</span></span>|<span data-ttu-id="e9d1a-196">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d1a-196">Int32</span></span>|<span data-ttu-id="e9d1a-197">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="e9d1a-197">Key length</span></span>|
|<span data-ttu-id="e9d1a-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e9d1a-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="e9d1a-199">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-199">String</span></span>|<span data-ttu-id="e9d1a-200">Расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="e9d1a-200">Extended key usage</span></span>|
|<span data-ttu-id="e9d1a-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="e9d1a-201">certificateValidityPeriod</span></span>|<span data-ttu-id="e9d1a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d1a-202">Int32</span></span>|<span data-ttu-id="e9d1a-203">Срок действия</span><span class="sxs-lookup"><span data-stu-id="e9d1a-203">Validity period</span></span>|
|<span data-ttu-id="e9d1a-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e9d1a-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="e9d1a-205">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-205">String</span></span>|<span data-ttu-id="e9d1a-206">Строку формата имени субъекта для форматов имя настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="e9d1a-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="e9d1a-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e9d1a-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e9d1a-208">String</span><span class="sxs-lookup"><span data-stu-id="e9d1a-208">String</span></span>|<span data-ttu-id="e9d1a-209">Строку формата альтернативное имя субъекта для настраиваемых форматов</span><span class="sxs-lookup"><span data-stu-id="e9d1a-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="e9d1a-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="e9d1a-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="e9d1a-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9d1a-211">DateTimeOffset</span></span>|<span data-ttu-id="e9d1a-212">Дата выдачи</span><span class="sxs-lookup"><span data-stu-id="e9d1a-212">Issuance date</span></span>|
|<span data-ttu-id="e9d1a-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="e9d1a-213">certificateErrorCode</span></span>|<span data-ttu-id="e9d1a-214">Int32</span><span class="sxs-lookup"><span data-stu-id="e9d1a-214">Int32</span></span>|<span data-ttu-id="e9d1a-215">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="e9d1a-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="e9d1a-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d1a-216">Response</span></span>
<span data-ttu-id="e9d1a-217">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9d1a-218">Пример</span><span class="sxs-lookup"><span data-stu-id="e9d1a-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9d1a-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9d1a-219">Request</span></span>
<span data-ttu-id="e9d1a-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9d1a-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d1a-221">Response</span></span>
<span data-ttu-id="e9d1a-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9d1a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




