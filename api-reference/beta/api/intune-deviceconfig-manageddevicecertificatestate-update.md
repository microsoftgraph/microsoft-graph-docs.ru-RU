---
title: Обновление Манажеддевицецертификатестате
description: Обновление свойств объекта Манажеддевицецертификатестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6c38cf87123e9c3f23cac3fb4eea457e7f6d597
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533371"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="820f7-103">Обновление Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="820f7-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="820f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="820f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="820f7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="820f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="820f7-106">Обновление свойств объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="820f7-106">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="820f7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="820f7-107">Prerequisites</span></span>
<span data-ttu-id="820f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="820f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="820f7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="820f7-110">Permission type</span></span>|<span data-ttu-id="820f7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="820f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="820f7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="820f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="820f7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820f7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="820f7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="820f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="820f7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="820f7-115">Not supported.</span></span>|
|<span data-ttu-id="820f7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="820f7-116">Application</span></span>|<span data-ttu-id="820f7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="820f7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="820f7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="820f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="820f7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="820f7-119">Request headers</span></span>
|<span data-ttu-id="820f7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="820f7-120">Header</span></span>|<span data-ttu-id="820f7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="820f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="820f7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="820f7-122">Authorization</span></span>|<span data-ttu-id="820f7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="820f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="820f7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="820f7-124">Accept</span></span>|<span data-ttu-id="820f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="820f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="820f7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="820f7-126">Request body</span></span>
<span data-ttu-id="820f7-127">В тексте запроса добавьте представление объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="820f7-127">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="820f7-128">В следующей таблице приведены свойства, необходимые при создании [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="820f7-128">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="820f7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="820f7-129">Property</span></span>|<span data-ttu-id="820f7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="820f7-130">Type</span></span>|<span data-ttu-id="820f7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="820f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="820f7-132">id</span><span class="sxs-lookup"><span data-stu-id="820f7-132">id</span></span>|<span data-ttu-id="820f7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="820f7-133">String</span></span>|<span data-ttu-id="820f7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="820f7-134">Key of the entity.</span></span>|
|<span data-ttu-id="820f7-135">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="820f7-135">devicePlatform</span></span>|[<span data-ttu-id="820f7-136">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="820f7-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="820f7-137">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="820f7-137">Device platform.</span></span> <span data-ttu-id="820f7-138">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="820f7-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="820f7-139">цертификатекэйусаже</span><span class="sxs-lookup"><span data-stu-id="820f7-139">certificateKeyUsage</span></span>|[<span data-ttu-id="820f7-140">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="820f7-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="820f7-141">Использование ключа.</span><span class="sxs-lookup"><span data-stu-id="820f7-141">Key usage.</span></span> <span data-ttu-id="820f7-142">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="820f7-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="820f7-143">цертификатевалидитипериодунитс</span><span class="sxs-lookup"><span data-stu-id="820f7-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="820f7-144">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="820f7-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="820f7-145">Единицы срока действия.</span><span class="sxs-lookup"><span data-stu-id="820f7-145">Validity period units.</span></span> <span data-ttu-id="820f7-146">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="820f7-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="820f7-147">цертификатеиссуанцестате</span><span class="sxs-lookup"><span data-stu-id="820f7-147">certificateIssuanceState</span></span>|[<span data-ttu-id="820f7-148">цертификатеиссуанцестатес</span><span class="sxs-lookup"><span data-stu-id="820f7-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="820f7-149">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="820f7-149">Issuance State.</span></span> <span data-ttu-id="820f7-150">Возможные значения: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `responsePending` `enrollmentSucceeded`,,,,,,,,,,,,,,,,,,,,, `issueFailed` `issuePending` `issued` `responseProcessingFailed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="820f7-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="820f7-151">цертификатекэйсторажепровидер</span><span class="sxs-lookup"><span data-stu-id="820f7-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="820f7-152">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="820f7-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="820f7-153">Поставщик хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="820f7-153">Key Storage Provider.</span></span> <span data-ttu-id="820f7-154">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="820f7-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="820f7-155">цертификатесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="820f7-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="820f7-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="820f7-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="820f7-157">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="820f7-157">Subject name format.</span></span> <span data-ttu-id="820f7-158">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="820f7-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="820f7-159">цертификатесубжекталтернативенамеформат</span><span class="sxs-lookup"><span data-stu-id="820f7-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="820f7-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="820f7-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="820f7-161">Формат альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="820f7-161">Subject alternative name format.</span></span> <span data-ttu-id="820f7-162">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="820f7-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="820f7-163">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="820f7-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="820f7-164">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="820f7-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="820f7-165">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="820f7-165">Revoke status.</span></span> <span data-ttu-id="820f7-166">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="820f7-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="820f7-167">цертификатепрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="820f7-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="820f7-168">String</span><span class="sxs-lookup"><span data-stu-id="820f7-168">String</span></span>|<span data-ttu-id="820f7-169">Отображаемое имя профиля сертификата</span><span class="sxs-lookup"><span data-stu-id="820f7-169">Certificate profile display name</span></span>|
|<span data-ttu-id="820f7-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="820f7-170">deviceDisplayName</span></span>|<span data-ttu-id="820f7-171">String</span><span class="sxs-lookup"><span data-stu-id="820f7-171">String</span></span>|<span data-ttu-id="820f7-172">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="820f7-172">Device display name</span></span>|
|<span data-ttu-id="820f7-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="820f7-173">userDisplayName</span></span>|<span data-ttu-id="820f7-174">String</span><span class="sxs-lookup"><span data-stu-id="820f7-174">String</span></span>|<span data-ttu-id="820f7-175">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="820f7-175">User display name</span></span>|
|<span data-ttu-id="820f7-176">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="820f7-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="820f7-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820f7-177">DateTimeOffset</span></span>|<span data-ttu-id="820f7-178">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="820f7-178">Certificate expiry date</span></span>|
|<span data-ttu-id="820f7-179">цертификателастиссуанцестатечанжеддатетиме</span><span class="sxs-lookup"><span data-stu-id="820f7-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="820f7-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820f7-180">DateTimeOffset</span></span>|<span data-ttu-id="820f7-181">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="820f7-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="820f7-182">ластцертификатестатечанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="820f7-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="820f7-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820f7-183">DateTimeOffset</span></span>|<span data-ttu-id="820f7-184">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="820f7-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="820f7-185">цертификатеиссуер</span><span class="sxs-lookup"><span data-stu-id="820f7-185">certificateIssuer</span></span>|<span data-ttu-id="820f7-186">String</span><span class="sxs-lookup"><span data-stu-id="820f7-186">String</span></span>|<span data-ttu-id="820f7-187">Издатель</span><span class="sxs-lookup"><span data-stu-id="820f7-187">Issuer</span></span>|
|<span data-ttu-id="820f7-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="820f7-188">certificateThumbprint</span></span>|<span data-ttu-id="820f7-189">String</span><span class="sxs-lookup"><span data-stu-id="820f7-189">String</span></span>|<span data-ttu-id="820f7-190">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="820f7-190">Thumbprint</span></span>|
|<span data-ttu-id="820f7-191">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="820f7-191">certificateSerialNumber</span></span>|<span data-ttu-id="820f7-192">String</span><span class="sxs-lookup"><span data-stu-id="820f7-192">String</span></span>|<span data-ttu-id="820f7-193">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="820f7-193">Serial number</span></span>|
|<span data-ttu-id="820f7-194">цертификатекэйленгс</span><span class="sxs-lookup"><span data-stu-id="820f7-194">certificateKeyLength</span></span>|<span data-ttu-id="820f7-195">Int32</span><span class="sxs-lookup"><span data-stu-id="820f7-195">Int32</span></span>|<span data-ttu-id="820f7-196">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="820f7-196">Key length</span></span>|
|<span data-ttu-id="820f7-197">цертификатинханцедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="820f7-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="820f7-198">String</span><span class="sxs-lookup"><span data-stu-id="820f7-198">String</span></span>|<span data-ttu-id="820f7-199">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="820f7-199">Extended key usage</span></span>|
|<span data-ttu-id="820f7-200">цертификатевалидитипериод</span><span class="sxs-lookup"><span data-stu-id="820f7-200">certificateValidityPeriod</span></span>|<span data-ttu-id="820f7-201">Int32</span><span class="sxs-lookup"><span data-stu-id="820f7-201">Int32</span></span>|<span data-ttu-id="820f7-202">Срок действия</span><span class="sxs-lookup"><span data-stu-id="820f7-202">Validity period</span></span>|
|<span data-ttu-id="820f7-203">цертификатесубжектнамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="820f7-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="820f7-204">String</span><span class="sxs-lookup"><span data-stu-id="820f7-204">String</span></span>|<span data-ttu-id="820f7-205">Строка формата имени субъекта для пользовательских форматов имен субъектов</span><span class="sxs-lookup"><span data-stu-id="820f7-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="820f7-206">цертификатесубжекталтернативенамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="820f7-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="820f7-207">String</span><span class="sxs-lookup"><span data-stu-id="820f7-207">String</span></span>|<span data-ttu-id="820f7-208">Строка формата альтернативного имени субъекта для пользовательских форматов</span><span class="sxs-lookup"><span data-stu-id="820f7-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="820f7-209">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="820f7-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="820f7-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="820f7-210">DateTimeOffset</span></span>|<span data-ttu-id="820f7-211">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="820f7-211">Issuance date</span></span>|
|<span data-ttu-id="820f7-212">цертификатирроркоде</span><span class="sxs-lookup"><span data-stu-id="820f7-212">certificateErrorCode</span></span>|<span data-ttu-id="820f7-213">Int32</span><span class="sxs-lookup"><span data-stu-id="820f7-213">Int32</span></span>|<span data-ttu-id="820f7-214">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="820f7-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="820f7-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="820f7-215">Response</span></span>
<span data-ttu-id="820f7-216">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="820f7-216">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="820f7-217">Пример</span><span class="sxs-lookup"><span data-stu-id="820f7-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="820f7-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="820f7-218">Request</span></span>
<span data-ttu-id="820f7-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="820f7-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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

### <a name="response"></a><span data-ttu-id="820f7-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="820f7-220">Response</span></span>
<span data-ttu-id="820f7-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="820f7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






