---
title: Обновление windowsPhone81SCEPCertificateProfile
description: Обновление свойств объекта windowsPhone81SCEPCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d6b4ea37d470dc94c0a0b186017afd7eb85352f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42733464"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="51487-103">Обновление windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="51487-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="51487-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51487-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51487-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51487-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51487-106">Обновление свойств объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="51487-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51487-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51487-107">Prerequisites</span></span>
<span data-ttu-id="51487-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51487-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51487-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51487-110">Permission type</span></span>|<span data-ttu-id="51487-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51487-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51487-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51487-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51487-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51487-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51487-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51487-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51487-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51487-115">Not supported.</span></span>|
|<span data-ttu-id="51487-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="51487-116">Application</span></span>|<span data-ttu-id="51487-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51487-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51487-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51487-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="51487-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51487-119">Request headers</span></span>
|<span data-ttu-id="51487-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51487-120">Header</span></span>|<span data-ttu-id="51487-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51487-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51487-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51487-122">Authorization</span></span>|<span data-ttu-id="51487-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51487-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51487-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51487-124">Accept</span></span>|<span data-ttu-id="51487-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51487-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51487-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51487-126">Request body</span></span>
<span data-ttu-id="51487-127">В тексте запроса добавьте представление объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51487-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="51487-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="51487-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="51487-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51487-129">Property</span></span>|<span data-ttu-id="51487-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51487-130">Type</span></span>|<span data-ttu-id="51487-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51487-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51487-132">id</span><span class="sxs-lookup"><span data-stu-id="51487-132">id</span></span>|<span data-ttu-id="51487-133">String</span><span class="sxs-lookup"><span data-stu-id="51487-133">String</span></span>|<span data-ttu-id="51487-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51487-134">Key of the entity.</span></span> <span data-ttu-id="51487-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51487-136">lastModifiedDateTime</span></span>|<span data-ttu-id="51487-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51487-137">DateTimeOffset</span></span>|<span data-ttu-id="51487-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="51487-138">DateTime the object was last modified.</span></span> <span data-ttu-id="51487-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51487-140">roleScopeTagIds</span></span>|<span data-ttu-id="51487-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51487-141">String collection</span></span>|<span data-ttu-id="51487-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="51487-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51487-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="51487-144">supportsScopeTags</span></span>|<span data-ttu-id="51487-145">Логический</span><span class="sxs-lookup"><span data-stu-id="51487-145">Boolean</span></span>|<span data-ttu-id="51487-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="51487-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51487-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="51487-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51487-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="51487-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51487-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51487-149">This property is read-only.</span></span> <span data-ttu-id="51487-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51487-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="51487-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51487-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="51487-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51487-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="51487-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51487-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="51487-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51487-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="51487-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51487-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="51487-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51487-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="51487-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51487-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="51487-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="51487-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="51487-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51487-163">createdDateTime</span></span>|<span data-ttu-id="51487-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51487-164">DateTimeOffset</span></span>|<span data-ttu-id="51487-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="51487-165">DateTime the object was created.</span></span> <span data-ttu-id="51487-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-167">description</span><span class="sxs-lookup"><span data-stu-id="51487-167">description</span></span>|<span data-ttu-id="51487-168">String</span><span class="sxs-lookup"><span data-stu-id="51487-168">String</span></span>|<span data-ttu-id="51487-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51487-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51487-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-171">displayName</span><span class="sxs-lookup"><span data-stu-id="51487-171">displayName</span></span>|<span data-ttu-id="51487-172">Строка</span><span class="sxs-lookup"><span data-stu-id="51487-172">String</span></span>|<span data-ttu-id="51487-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51487-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51487-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-175">version</span><span class="sxs-lookup"><span data-stu-id="51487-175">version</span></span>|<span data-ttu-id="51487-176">Int32</span><span class="sxs-lookup"><span data-stu-id="51487-176">Int32</span></span>|<span data-ttu-id="51487-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51487-177">Version of the device configuration.</span></span> <span data-ttu-id="51487-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51487-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51487-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="51487-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="51487-180">Int32</span><span class="sxs-lookup"><span data-stu-id="51487-180">Int32</span></span>|<span data-ttu-id="51487-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="51487-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="51487-182">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="51487-182">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="51487-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="51487-183">keyStorageProvider</span></span>|[<span data-ttu-id="51487-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="51487-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="51487-185">Поставщик хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="51487-185">Key Storage Provider (KSP).</span></span> <span data-ttu-id="51487-186">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="51487-186">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="51487-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="51487-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="51487-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="51487-188">subjectNameFormat</span></span>|[<span data-ttu-id="51487-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="51487-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="51487-190">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="51487-190">Certificate Subject Name Format.</span></span> <span data-ttu-id="51487-191">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="51487-191">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="51487-192">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="51487-192">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="51487-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="51487-193">subjectAlternativeNameType</span></span>|[<span data-ttu-id="51487-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="51487-194">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="51487-195">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="51487-195">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="51487-196">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="51487-196">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="51487-197">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="51487-197">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="51487-198">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="51487-198">certificateValidityPeriodValue</span></span>|<span data-ttu-id="51487-199">Int32</span><span class="sxs-lookup"><span data-stu-id="51487-199">Int32</span></span>|<span data-ttu-id="51487-200">Значение периода Валидтий для сертификата.</span><span class="sxs-lookup"><span data-stu-id="51487-200">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="51487-201">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="51487-201">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="51487-202">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="51487-202">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="51487-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="51487-203">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="51487-204">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="51487-204">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="51487-205">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="51487-205">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="51487-206">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="51487-206">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="51487-207">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="51487-207">extendedKeyUsages</span></span>|<span data-ttu-id="51487-208">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="51487-208">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="51487-209">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="51487-209">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="51487-210">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="51487-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="51487-211">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="51487-211">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="51487-212">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="51487-212">scepServerUrls</span></span>|<span data-ttu-id="51487-213">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="51487-213">String collection</span></span>|<span data-ttu-id="51487-214">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="51487-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="51487-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="51487-215">subjectNameFormatString</span></span>|<span data-ttu-id="51487-216">String</span><span class="sxs-lookup"><span data-stu-id="51487-216">String</span></span>|<span data-ttu-id="51487-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="51487-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="51487-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="51487-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="51487-219">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="51487-219">keyUsage</span></span>|[<span data-ttu-id="51487-220">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="51487-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="51487-221">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="51487-221">SCEP Key Usage.</span></span> <span data-ttu-id="51487-222">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="51487-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="51487-223">keySize</span><span class="sxs-lookup"><span data-stu-id="51487-223">keySize</span></span>|[<span data-ttu-id="51487-224">keySize</span><span class="sxs-lookup"><span data-stu-id="51487-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="51487-225">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="51487-225">SCEP Key Size.</span></span> <span data-ttu-id="51487-226">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="51487-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="51487-227">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="51487-227">hashAlgorithm</span></span>|[<span data-ttu-id="51487-228">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="51487-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="51487-229">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="51487-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="51487-230">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="51487-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="51487-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="51487-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="51487-232">String</span><span class="sxs-lookup"><span data-stu-id="51487-232">String</span></span>|<span data-ttu-id="51487-233">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="51487-233">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="51487-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="51487-234">Response</span></span>
<span data-ttu-id="51487-235">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51487-235">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51487-236">Пример</span><span class="sxs-lookup"><span data-stu-id="51487-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="51487-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="51487-237">Request</span></span>
<span data-ttu-id="51487-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51487-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="51487-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="51487-239">Response</span></span>
<span data-ttu-id="51487-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51487-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




