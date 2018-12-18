---
title: Обновление managedDeviceCertificateState
description: Обновление свойства объекта managedDeviceCertificateState.
author: tfitzmac
ms.openlocfilehash: 14c73bf219d8a568f8df0c4c55e3a1e3d0516abd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350171"
---
# <a name="update-manageddevicecertificatestate"></a><span data-ttu-id="81d27-103">Обновление managedDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="81d27-103">Update managedDeviceCertificateState</span></span>

> <span data-ttu-id="81d27-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81d27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81d27-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81d27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81d27-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81d27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81d27-107">Обновление свойства объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="81d27-107">Update the properties of a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81d27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81d27-108">Prerequisites</span></span>
<span data-ttu-id="81d27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81d27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81d27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81d27-111">Permission type</span></span>|<span data-ttu-id="81d27-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81d27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81d27-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81d27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="81d27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81d27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81d27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81d27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81d27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81d27-116">Not supported.</span></span>|
|<span data-ttu-id="81d27-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81d27-117">Application</span></span>|<span data-ttu-id="81d27-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81d27-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81d27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81d27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
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

## <a name="request-headers"></a><span data-ttu-id="81d27-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81d27-120">Request headers</span></span>
|<span data-ttu-id="81d27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81d27-121">Header</span></span>|<span data-ttu-id="81d27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81d27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81d27-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81d27-123">Authorization</span></span>|<span data-ttu-id="81d27-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="81d27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81d27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="81d27-125">Accept</span></span>|<span data-ttu-id="81d27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="81d27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81d27-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81d27-127">Request body</span></span>
<span data-ttu-id="81d27-128">В тексте запроса укажите представление JSON для объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .</span><span class="sxs-lookup"><span data-stu-id="81d27-128">In the request body, supply a JSON representation for the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

<span data-ttu-id="81d27-129">В следующей таблице показаны свойства, которые необходимы для создания [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span><span class="sxs-lookup"><span data-stu-id="81d27-129">The following table shows the properties that are required when you create the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).</span></span>

|<span data-ttu-id="81d27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="81d27-130">Property</span></span>|<span data-ttu-id="81d27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="81d27-131">Type</span></span>|<span data-ttu-id="81d27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="81d27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d27-133">id</span><span class="sxs-lookup"><span data-stu-id="81d27-133">id</span></span>|<span data-ttu-id="81d27-134">Строка</span><span class="sxs-lookup"><span data-stu-id="81d27-134">String</span></span>|<span data-ttu-id="81d27-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81d27-135">Key of the entity.</span></span>|
|<span data-ttu-id="81d27-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="81d27-136">devicePlatform</span></span>|[<span data-ttu-id="81d27-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="81d27-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="81d27-138">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="81d27-138">Device platform.</span></span> <span data-ttu-id="81d27-139">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="81d27-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="81d27-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="81d27-140">certificateKeyUsage</span></span>|[<span data-ttu-id="81d27-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="81d27-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="81d27-142">Использование ключей.</span><span class="sxs-lookup"><span data-stu-id="81d27-142">Key usage.</span></span> <span data-ttu-id="81d27-143">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="81d27-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="81d27-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="81d27-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="81d27-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="81d27-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="81d27-146">Действия подразделений.</span><span class="sxs-lookup"><span data-stu-id="81d27-146">Validity period units.</span></span> <span data-ttu-id="81d27-147">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="81d27-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="81d27-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="81d27-148">certificateIssuanceState</span></span>|[<span data-ttu-id="81d27-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="81d27-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="81d27-150">Состояние выдачи.</span><span class="sxs-lookup"><span data-stu-id="81d27-150">Issuance State.</span></span> <span data-ttu-id="81d27-151">Возможные значения: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="81d27-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="81d27-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="81d27-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="81d27-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="81d27-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="81d27-154">Поставщика хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="81d27-154">Key Storage Provider.</span></span> <span data-ttu-id="81d27-155">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="81d27-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="81d27-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81d27-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="81d27-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81d27-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="81d27-158">Формат имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="81d27-158">Subject name format.</span></span> <span data-ttu-id="81d27-159">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="81d27-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="81d27-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="81d27-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="81d27-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="81d27-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="81d27-162">Формат альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="81d27-162">Subject alternative name format.</span></span> <span data-ttu-id="81d27-163">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="81d27-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="81d27-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="81d27-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="81d27-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="81d27-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="81d27-166">Отмените состояние.</span><span class="sxs-lookup"><span data-stu-id="81d27-166">Revoke status.</span></span> <span data-ttu-id="81d27-167">Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.</span><span class="sxs-lookup"><span data-stu-id="81d27-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="81d27-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="81d27-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="81d27-169">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-169">String</span></span>|<span data-ttu-id="81d27-170">Отображаемое имя сертификата профилей</span><span class="sxs-lookup"><span data-stu-id="81d27-170">Certificate profile display name</span></span>|
|<span data-ttu-id="81d27-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="81d27-171">deviceDisplayName</span></span>|<span data-ttu-id="81d27-172">String</span><span class="sxs-lookup"><span data-stu-id="81d27-172">String</span></span>|<span data-ttu-id="81d27-173">Отображаемое имя устройства</span><span class="sxs-lookup"><span data-stu-id="81d27-173">Device display name</span></span>|
|<span data-ttu-id="81d27-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="81d27-174">userDisplayName</span></span>|<span data-ttu-id="81d27-175">String</span><span class="sxs-lookup"><span data-stu-id="81d27-175">String</span></span>|<span data-ttu-id="81d27-176">Отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="81d27-176">User display name</span></span>|
|<span data-ttu-id="81d27-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="81d27-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="81d27-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d27-178">DateTimeOffset</span></span>|<span data-ttu-id="81d27-179">Дата окончания срока действия сертификата</span><span class="sxs-lookup"><span data-stu-id="81d27-179">Certificate expiry date</span></span>|
|<span data-ttu-id="81d27-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="81d27-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="81d27-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d27-181">DateTimeOffset</span></span>|<span data-ttu-id="81d27-182">Последнее изменение состояния выдачи сертификатов</span><span class="sxs-lookup"><span data-stu-id="81d27-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="81d27-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="81d27-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="81d27-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d27-184">DateTimeOffset</span></span>|<span data-ttu-id="81d27-185">Последнее изменение состояния выдачи сертификатов</span><span class="sxs-lookup"><span data-stu-id="81d27-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="81d27-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="81d27-186">certificateIssuer</span></span>|<span data-ttu-id="81d27-187">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-187">String</span></span>|<span data-ttu-id="81d27-188">Издателя</span><span class="sxs-lookup"><span data-stu-id="81d27-188">Issuer</span></span>|
|<span data-ttu-id="81d27-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="81d27-189">certificateThumbprint</span></span>|<span data-ttu-id="81d27-190">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-190">String</span></span>|<span data-ttu-id="81d27-191">Отпечаток</span><span class="sxs-lookup"><span data-stu-id="81d27-191">Thumbprint</span></span>|
|<span data-ttu-id="81d27-192">серийный номер сертификата</span><span class="sxs-lookup"><span data-stu-id="81d27-192">certificateSerialNumber</span></span>|<span data-ttu-id="81d27-193">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-193">String</span></span>|<span data-ttu-id="81d27-194">Серийный номер</span><span class="sxs-lookup"><span data-stu-id="81d27-194">Serial number</span></span>|
|<span data-ttu-id="81d27-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="81d27-195">certificateKeyLength</span></span>|<span data-ttu-id="81d27-196">Int32</span><span class="sxs-lookup"><span data-stu-id="81d27-196">Int32</span></span>|<span data-ttu-id="81d27-197">Длина ключа</span><span class="sxs-lookup"><span data-stu-id="81d27-197">Key length</span></span>|
|<span data-ttu-id="81d27-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="81d27-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="81d27-199">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-199">String</span></span>|<span data-ttu-id="81d27-200">Расширенного использования ключа</span><span class="sxs-lookup"><span data-stu-id="81d27-200">Extended key usage</span></span>|
|<span data-ttu-id="81d27-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="81d27-201">certificateValidityPeriod</span></span>|<span data-ttu-id="81d27-202">Int32</span><span class="sxs-lookup"><span data-stu-id="81d27-202">Int32</span></span>|<span data-ttu-id="81d27-203">Срок действия</span><span class="sxs-lookup"><span data-stu-id="81d27-203">Validity period</span></span>|
|<span data-ttu-id="81d27-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="81d27-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="81d27-205">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-205">String</span></span>|<span data-ttu-id="81d27-206">Строку формата имени субъекта для форматов имя настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="81d27-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="81d27-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="81d27-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="81d27-208">String.</span><span class="sxs-lookup"><span data-stu-id="81d27-208">String</span></span>|<span data-ttu-id="81d27-209">Строку формата альтернативное имя субъекта для настраиваемых форматов</span><span class="sxs-lookup"><span data-stu-id="81d27-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="81d27-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="81d27-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="81d27-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81d27-211">DateTimeOffset</span></span>|<span data-ttu-id="81d27-212">Дата выдачи</span><span class="sxs-lookup"><span data-stu-id="81d27-212">Issuance date</span></span>|
|<span data-ttu-id="81d27-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="81d27-213">certificateErrorCode</span></span>|<span data-ttu-id="81d27-214">Int32</span><span class="sxs-lookup"><span data-stu-id="81d27-214">Int32</span></span>|<span data-ttu-id="81d27-215">Код ошибки</span><span class="sxs-lookup"><span data-stu-id="81d27-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="81d27-216">Ответ</span><span class="sxs-lookup"><span data-stu-id="81d27-216">Response</span></span>
<span data-ttu-id="81d27-217">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="81d27-217">If successful, this method returns a `200 OK` response code and an updated [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81d27-218">Пример</span><span class="sxs-lookup"><span data-stu-id="81d27-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="81d27-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="81d27-219">Request</span></span>
<span data-ttu-id="81d27-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81d27-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates/{managedDeviceCertificateStateId}
Content-type: application/json
Content-length: 1449

{
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

### <a name="response"></a><span data-ttu-id="81d27-221">Ответ</span><span class="sxs-lookup"><span data-stu-id="81d27-221">Response</span></span>
<span data-ttu-id="81d27-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="81d27-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





