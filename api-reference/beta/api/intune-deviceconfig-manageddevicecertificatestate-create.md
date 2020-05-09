---
title: Создание Манажеддевицецертификатестате
description: Создание нового объекта Манажеддевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 914285da1e6934df509c43e53d5e99cb0acbd24d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177844"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="c373f-103">Создание Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="c373f-103">Create managedDeviceCertificateState</span></span>

<span data-ttu-id="c373f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c373f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c373f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c373f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c373f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c373f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c373f-107">Создание нового объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="c373f-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c373f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c373f-108">Prerequisites</span></span>
<span data-ttu-id="c373f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c373f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c373f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c373f-111">Permission type</span></span>|<span data-ttu-id="c373f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c373f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c373f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c373f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c373f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c373f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c373f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c373f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c373f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c373f-116">Not supported.</span></span>|
|<span data-ttu-id="c373f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c373f-117">Application</span></span>|<span data-ttu-id="c373f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c373f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c373f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c373f-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="c373f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c373f-120">Request headers</span></span>
|<span data-ttu-id="c373f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c373f-121">Header</span></span>|<span data-ttu-id="c373f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c373f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c373f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c373f-123">Authorization</span></span>|<span data-ttu-id="c373f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c373f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c373f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c373f-125">Accept</span></span>|<span data-ttu-id="c373f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c373f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c373f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c373f-127">Request body</span></span>
<span data-ttu-id="c373f-128">В тексте запроса добавьте представление объекта Манажеддевицецертификатестате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c373f-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="c373f-129">В следующей таблице приведены свойства, необходимые при создании Манажеддевицецертификатестате.</span><span class="sxs-lookup"><span data-stu-id="c373f-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="c373f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c373f-130">Property</span></span>|<span data-ttu-id="c373f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c373f-131">Type</span></span>|<span data-ttu-id="c373f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c373f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c373f-133">id</span><span class="sxs-lookup"><span data-stu-id="c373f-133">id</span></span>|<span data-ttu-id="c373f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-134">String</span></span>|<span data-ttu-id="c373f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c373f-135">Key of the entity.</span></span>|
|<span data-ttu-id="c373f-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c373f-136">devicePlatform</span></span>|[<span data-ttu-id="c373f-137">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="c373f-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="c373f-138">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="c373f-138">Device platform.</span></span> <span data-ttu-id="c373f-139">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c373f-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="c373f-140">цертификатекэйусаже</span><span class="sxs-lookup"><span data-stu-id="c373f-140">certificateKeyUsage</span></span>|[<span data-ttu-id="c373f-141">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="c373f-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c373f-142">Использование ключа.</span><span class="sxs-lookup"><span data-stu-id="c373f-142">Key usage.</span></span> <span data-ttu-id="c373f-143">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c373f-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c373f-144">цертификатевалидитипериодунитс</span><span class="sxs-lookup"><span data-stu-id="c373f-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="c373f-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c373f-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c373f-146">Единицы срока действия.</span><span class="sxs-lookup"><span data-stu-id="c373f-146">Validity period units.</span></span> <span data-ttu-id="c373f-147">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c373f-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c373f-148">цертификатеиссуанцестате</span><span class="sxs-lookup"><span data-stu-id="c373f-148">certificateIssuanceState</span></span>|[<span data-ttu-id="c373f-149">цертификатеиссуанцестатес</span><span class="sxs-lookup"><span data-stu-id="c373f-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="c373f-150">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="c373f-150">Issuance State.</span></span> <span data-ttu-id="c373f-151">Возможные `unknown`значения:, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested`,,,,,,, `enrollmentSucceeded`,,,,,,,,,,,,,,,,,,. `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending`</span><span class="sxs-lookup"><span data-stu-id="c373f-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="c373f-152">цертификатекэйсторажепровидер</span><span class="sxs-lookup"><span data-stu-id="c373f-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="c373f-153">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="c373f-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c373f-154">Поставщик хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="c373f-154">Key Storage Provider.</span></span> <span data-ttu-id="c373f-155">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c373f-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c373f-156">цертификатесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="c373f-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="c373f-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c373f-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c373f-158">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="c373f-158">Subject name format.</span></span> <span data-ttu-id="c373f-159">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c373f-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c373f-160">цертификатесубжекталтернативенамеформат</span><span class="sxs-lookup"><span data-stu-id="c373f-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="c373f-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c373f-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c373f-162">Формат альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="c373f-162">Subject alternative name format.</span></span> <span data-ttu-id="c373f-163">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c373f-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c373f-164">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="c373f-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="c373f-165">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="c373f-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="c373f-166">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="c373f-166">Revoke status.</span></span> <span data-ttu-id="c373f-167">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="c373f-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="c373f-168">цертификатепрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="c373f-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="c373f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-169">String</span></span>|<span data-ttu-id="c373f-170">Отображаемое имя профиля сертификата</span><span class="sxs-lookup"><span data-stu-id="c373f-170">Certificate profile display name</span></span>|
|<span data-ttu-id="c373f-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c373f-171">deviceDisplayName</span></span>|<span data-ttu-id="c373f-172">String</span><span class="sxs-lookup"><span data-stu-id="c373f-172">String</span></span>|<span data-ttu-id="c373f-173">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="c373f-173">Device display name</span></span>|
|<span data-ttu-id="c373f-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c373f-174">userDisplayName</span></span>|<span data-ttu-id="c373f-175">String</span><span class="sxs-lookup"><span data-stu-id="c373f-175">String</span></span>|<span data-ttu-id="c373f-176">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="c373f-176">User display name</span></span>|
|<span data-ttu-id="c373f-177">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="c373f-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="c373f-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c373f-178">DateTimeOffset</span></span>|<span data-ttu-id="c373f-179">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="c373f-179">Certificate expiry date</span></span>|
|<span data-ttu-id="c373f-180">цертификателастиссуанцестатечанжеддатетиме</span><span class="sxs-lookup"><span data-stu-id="c373f-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="c373f-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c373f-181">DateTimeOffset</span></span>|<span data-ttu-id="c373f-182">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="c373f-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="c373f-183">ластцертификатестатечанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="c373f-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="c373f-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c373f-184">DateTimeOffset</span></span>|<span data-ttu-id="c373f-185">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="c373f-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="c373f-186">цертификатеиссуер</span><span class="sxs-lookup"><span data-stu-id="c373f-186">certificateIssuer</span></span>|<span data-ttu-id="c373f-187">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-187">String</span></span>|<span data-ttu-id="c373f-188">Издатель</span><span class="sxs-lookup"><span data-stu-id="c373f-188">Issuer</span></span>|
|<span data-ttu-id="c373f-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="c373f-189">certificateThumbprint</span></span>|<span data-ttu-id="c373f-190">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-190">String</span></span>|<span data-ttu-id="c373f-191">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="c373f-191">Thumbprint</span></span>|
|<span data-ttu-id="c373f-192">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="c373f-192">certificateSerialNumber</span></span>|<span data-ttu-id="c373f-193">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-193">String</span></span>|<span data-ttu-id="c373f-194">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="c373f-194">Serial number</span></span>|
|<span data-ttu-id="c373f-195">цертификатекэйленгс</span><span class="sxs-lookup"><span data-stu-id="c373f-195">certificateKeyLength</span></span>|<span data-ttu-id="c373f-196">Int32</span><span class="sxs-lookup"><span data-stu-id="c373f-196">Int32</span></span>|<span data-ttu-id="c373f-197">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="c373f-197">Key length</span></span>|
|<span data-ttu-id="c373f-198">цертификатинханцедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="c373f-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="c373f-199">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-199">String</span></span>|<span data-ttu-id="c373f-200">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="c373f-200">Extended key usage</span></span>|
|<span data-ttu-id="c373f-201">цертификатевалидитипериод</span><span class="sxs-lookup"><span data-stu-id="c373f-201">certificateValidityPeriod</span></span>|<span data-ttu-id="c373f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c373f-202">Int32</span></span>|<span data-ttu-id="c373f-203">Срок действия</span><span class="sxs-lookup"><span data-stu-id="c373f-203">Validity period</span></span>|
|<span data-ttu-id="c373f-204">цертификатесубжектнамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="c373f-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="c373f-205">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-205">String</span></span>|<span data-ttu-id="c373f-206">Строка формата имени субъекта для пользовательских форматов имен субъектов</span><span class="sxs-lookup"><span data-stu-id="c373f-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="c373f-207">цертификатесубжекталтернативенамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="c373f-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c373f-208">Строка</span><span class="sxs-lookup"><span data-stu-id="c373f-208">String</span></span>|<span data-ttu-id="c373f-209">Строка формата альтернативного имени субъекта для пользовательских форматов</span><span class="sxs-lookup"><span data-stu-id="c373f-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="c373f-210">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="c373f-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="c373f-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c373f-211">DateTimeOffset</span></span>|<span data-ttu-id="c373f-212">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="c373f-212">Issuance date</span></span>|
|<span data-ttu-id="c373f-213">цертификатирроркоде</span><span class="sxs-lookup"><span data-stu-id="c373f-213">certificateErrorCode</span></span>|<span data-ttu-id="c373f-214">Int32</span><span class="sxs-lookup"><span data-stu-id="c373f-214">Int32</span></span>|<span data-ttu-id="c373f-215">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="c373f-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="c373f-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="c373f-216">Response</span></span>
<span data-ttu-id="c373f-217">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c373f-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c373f-218">Пример</span><span class="sxs-lookup"><span data-stu-id="c373f-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="c373f-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="c373f-219">Request</span></span>
<span data-ttu-id="c373f-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c373f-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c373f-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="c373f-221">Response</span></span>
<span data-ttu-id="c373f-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c373f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



