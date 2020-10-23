---
title: Обновление Манажеддевицецертификатестате
description: Обновление свойств объекта Манажеддевицецертификатестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6d097573c8abdd7fee9f08b98aa5eaf8528deb62
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696911"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="b1e30-103">Обновление Манажеддевицецертификатестате</span><span class="sxs-lookup"><span data-stu-id="b1e30-103">Update managedDeviceCertificateState</span></span>

<span data-ttu-id="b1e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1e30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1e30-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1e30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1e30-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1e30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1e30-107">Обновление свойств объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="b1e30-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1e30-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b1e30-108">Prerequisites</span></span>
<span data-ttu-id="b1e30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1e30-111">Permission type</span></span>|<span data-ttu-id="b1e30-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1e30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1e30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1e30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1e30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1e30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1e30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1e30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1e30-116">Not supported.</span></span>|
|<span data-ttu-id="b1e30-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1e30-117">Application</span></span>|<span data-ttu-id="b1e30-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e30-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1e30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1e30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfilePkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="b1e30-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1e30-120">Request headers</span></span>
|<span data-ttu-id="b1e30-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1e30-121">Header</span></span>|<span data-ttu-id="b1e30-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b1e30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1e30-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1e30-123">Authorization</span></span>|<span data-ttu-id="b1e30-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1e30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1e30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1e30-125">Accept</span></span>|<span data-ttu-id="b1e30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1e30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1e30-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1e30-127">Request body</span></span>
<span data-ttu-id="b1e30-128">В тексте запроса добавьте представление объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1e30-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="b1e30-129">В следующей таблице приведены свойства, необходимые при создании [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="b1e30-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="b1e30-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1e30-130">Property</span></span>|<span data-ttu-id="b1e30-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b1e30-131">Type</span></span>|<span data-ttu-id="b1e30-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b1e30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1e30-133">id</span><span class="sxs-lookup"><span data-stu-id="b1e30-133">id</span></span>|<span data-ttu-id="b1e30-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-134">String</span></span>|<span data-ttu-id="b1e30-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1e30-135">Key of the entity.</span></span>|
|<span data-ttu-id="b1e30-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="b1e30-136">devicePlatform</span></span>|[<span data-ttu-id="b1e30-137">девицеплатформтипе</span><span class="sxs-lookup"><span data-stu-id="b1e30-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="b1e30-138">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="b1e30-138">Device platform.</span></span> <span data-ttu-id="b1e30-139">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="b1e30-140">цертификатекэйусаже</span><span class="sxs-lookup"><span data-stu-id="b1e30-140">certificateKeyUsage</span></span>|[<span data-ttu-id="b1e30-141">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="b1e30-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b1e30-142">Использование ключа.</span><span class="sxs-lookup"><span data-stu-id="b1e30-142">Key usage.</span></span> <span data-ttu-id="b1e30-143">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b1e30-144">цертификатевалидитипериодунитс</span><span class="sxs-lookup"><span data-stu-id="b1e30-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="b1e30-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b1e30-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b1e30-146">Единицы срока действия.</span><span class="sxs-lookup"><span data-stu-id="b1e30-146">Validity period units.</span></span> <span data-ttu-id="b1e30-147">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b1e30-148">цертификатеиссуанцестате</span><span class="sxs-lookup"><span data-stu-id="b1e30-148">certificateIssuanceState</span></span>|[<span data-ttu-id="b1e30-149">цертификатеиссуанцестатес</span><span class="sxs-lookup"><span data-stu-id="b1e30-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="b1e30-150">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="b1e30-150">Issuance State.</span></span> <span data-ttu-id="b1e30-151">Возможные значения:,,,,,,,,,,, `unknown` `challengeIssued` `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` , `enrollmentNotNeeded` , `revoked` , `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` ,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="b1e30-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="b1e30-152">цертификатекэйсторажепровидер</span><span class="sxs-lookup"><span data-stu-id="b1e30-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="b1e30-153">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="b1e30-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="b1e30-154">Поставщик хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="b1e30-154">Key Storage Provider.</span></span> <span data-ttu-id="b1e30-155">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b1e30-156">цертификатесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="b1e30-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="b1e30-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b1e30-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b1e30-158">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="b1e30-158">Subject name format.</span></span> <span data-ttu-id="b1e30-159">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b1e30-160">цертификатесубжекталтернативенамеформат</span><span class="sxs-lookup"><span data-stu-id="b1e30-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="b1e30-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b1e30-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b1e30-162">Формат альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="b1e30-162">Subject alternative name format.</span></span> <span data-ttu-id="b1e30-163">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="b1e30-164">цертификатеревокестатус</span><span class="sxs-lookup"><span data-stu-id="b1e30-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="b1e30-165">цертификатеревокатионстатус</span><span class="sxs-lookup"><span data-stu-id="b1e30-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="b1e30-166">Отзыв состояния.</span><span class="sxs-lookup"><span data-stu-id="b1e30-166">Revoke status.</span></span> <span data-ttu-id="b1e30-167">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="b1e30-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="b1e30-168">цертификатепрофиледисплайнаме</span><span class="sxs-lookup"><span data-stu-id="b1e30-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="b1e30-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-169">String</span></span>|<span data-ttu-id="b1e30-170">Отображаемое имя профиля сертификата</span><span class="sxs-lookup"><span data-stu-id="b1e30-170">Certificate profile display name</span></span>|
|<span data-ttu-id="b1e30-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1e30-171">deviceDisplayName</span></span>|<span data-ttu-id="b1e30-172">String</span><span class="sxs-lookup"><span data-stu-id="b1e30-172">String</span></span>|<span data-ttu-id="b1e30-173">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="b1e30-173">Device display name</span></span>|
|<span data-ttu-id="b1e30-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1e30-174">userDisplayName</span></span>|<span data-ttu-id="b1e30-175">String</span><span class="sxs-lookup"><span data-stu-id="b1e30-175">String</span></span>|<span data-ttu-id="b1e30-176">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="b1e30-176">User display name</span></span>|
|<span data-ttu-id="b1e30-177">цертификатикспиратиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b1e30-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="b1e30-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1e30-178">DateTimeOffset</span></span>|<span data-ttu-id="b1e30-179">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="b1e30-179">Certificate expiry date</span></span>|
|<span data-ttu-id="b1e30-180">цертификателастиссуанцестатечанжеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b1e30-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="b1e30-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1e30-181">DateTimeOffset</span></span>|<span data-ttu-id="b1e30-182">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="b1e30-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="b1e30-183">ластцертификатестатечанжедатетиме</span><span class="sxs-lookup"><span data-stu-id="b1e30-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="b1e30-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1e30-184">DateTimeOffset</span></span>|<span data-ttu-id="b1e30-185">Последнее изменение состояния выдачи сертификата</span><span class="sxs-lookup"><span data-stu-id="b1e30-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="b1e30-186">цертификатеиссуер</span><span class="sxs-lookup"><span data-stu-id="b1e30-186">certificateIssuer</span></span>|<span data-ttu-id="b1e30-187">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-187">String</span></span>|<span data-ttu-id="b1e30-188">Издатель</span><span class="sxs-lookup"><span data-stu-id="b1e30-188">Issuer</span></span>|
|<span data-ttu-id="b1e30-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="b1e30-189">certificateThumbprint</span></span>|<span data-ttu-id="b1e30-190">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-190">String</span></span>|<span data-ttu-id="b1e30-191">Thumbprint</span><span class="sxs-lookup"><span data-stu-id="b1e30-191">Thumbprint</span></span>|
|<span data-ttu-id="b1e30-192">цертификатесериалнумбер</span><span class="sxs-lookup"><span data-stu-id="b1e30-192">certificateSerialNumber</span></span>|<span data-ttu-id="b1e30-193">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-193">String</span></span>|<span data-ttu-id="b1e30-194">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="b1e30-194">Serial number</span></span>|
|<span data-ttu-id="b1e30-195">цертификатекэйленгс</span><span class="sxs-lookup"><span data-stu-id="b1e30-195">certificateKeyLength</span></span>|<span data-ttu-id="b1e30-196">Int32</span><span class="sxs-lookup"><span data-stu-id="b1e30-196">Int32</span></span>|<span data-ttu-id="b1e30-197">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="b1e30-197">Key length</span></span>|
|<span data-ttu-id="b1e30-198">цертификатинханцедкэйусаже</span><span class="sxs-lookup"><span data-stu-id="b1e30-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="b1e30-199">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-199">String</span></span>|<span data-ttu-id="b1e30-200">Расширенное использование ключа</span><span class="sxs-lookup"><span data-stu-id="b1e30-200">Extended key usage</span></span>|
|<span data-ttu-id="b1e30-201">цертификатевалидитипериод</span><span class="sxs-lookup"><span data-stu-id="b1e30-201">certificateValidityPeriod</span></span>|<span data-ttu-id="b1e30-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b1e30-202">Int32</span></span>|<span data-ttu-id="b1e30-203">Срок действия</span><span class="sxs-lookup"><span data-stu-id="b1e30-203">Validity period</span></span>|
|<span data-ttu-id="b1e30-204">цертификатесубжектнамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="b1e30-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="b1e30-205">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-205">String</span></span>|<span data-ttu-id="b1e30-206">Строка формата имени субъекта для пользовательских форматов имен субъектов</span><span class="sxs-lookup"><span data-stu-id="b1e30-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="b1e30-207">цертификатесубжекталтернативенамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="b1e30-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b1e30-208">Строка</span><span class="sxs-lookup"><span data-stu-id="b1e30-208">String</span></span>|<span data-ttu-id="b1e30-209">Строка формата альтернативного имени субъекта для пользовательских форматов</span><span class="sxs-lookup"><span data-stu-id="b1e30-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="b1e30-210">цертификатеиссуанцедатетиме</span><span class="sxs-lookup"><span data-stu-id="b1e30-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="b1e30-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1e30-211">DateTimeOffset</span></span>|<span data-ttu-id="b1e30-212">Дата выпуска</span><span class="sxs-lookup"><span data-stu-id="b1e30-212">Issuance date</span></span>|
|<span data-ttu-id="b1e30-213">цертификатирроркоде</span><span class="sxs-lookup"><span data-stu-id="b1e30-213">certificateErrorCode</span></span>|<span data-ttu-id="b1e30-214">Int32</span><span class="sxs-lookup"><span data-stu-id="b1e30-214">Int32</span></span>|<span data-ttu-id="b1e30-215">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="b1e30-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="b1e30-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1e30-216">Response</span></span>
<span data-ttu-id="b1e30-217">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e30-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1e30-218">Пример</span><span class="sxs-lookup"><span data-stu-id="b1e30-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1e30-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e30-219">Request</span></span>
<span data-ttu-id="b1e30-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e30-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1e30-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e30-221">Response</span></span>
<span data-ttu-id="b1e30-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1e30-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





