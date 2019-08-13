---
title: Обновление windowsPhone81ImportedPFXCertificateProfile
description: Обновление свойств объекта windowsPhone81ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ea26f1ee210ad871a9f0e70dd6e145de2484e564
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313946"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="696ef-103">Обновление windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="696ef-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="696ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="696ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="696ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="696ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="696ef-106">Обновление свойств объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="696ef-106">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="696ef-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="696ef-107">Prerequisites</span></span>
<span data-ttu-id="696ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="696ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="696ef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="696ef-110">Permission type</span></span>|<span data-ttu-id="696ef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="696ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="696ef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="696ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="696ef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="696ef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="696ef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="696ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="696ef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="696ef-115">Not supported.</span></span>|
|<span data-ttu-id="696ef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="696ef-116">Application</span></span>|<span data-ttu-id="696ef-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="696ef-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="696ef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="696ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="696ef-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="696ef-119">Request headers</span></span>
|<span data-ttu-id="696ef-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="696ef-120">Header</span></span>|<span data-ttu-id="696ef-121">Значение</span><span class="sxs-lookup"><span data-stu-id="696ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="696ef-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="696ef-122">Authorization</span></span>|<span data-ttu-id="696ef-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="696ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="696ef-124">Accept</span><span class="sxs-lookup"><span data-stu-id="696ef-124">Accept</span></span>|<span data-ttu-id="696ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="696ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="696ef-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="696ef-126">Request body</span></span>
<span data-ttu-id="696ef-127">В тексте запроса добавьте представление объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="696ef-127">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="696ef-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-128">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="696ef-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="696ef-129">Property</span></span>|<span data-ttu-id="696ef-130">Тип</span><span class="sxs-lookup"><span data-stu-id="696ef-130">Type</span></span>|<span data-ttu-id="696ef-131">Описание</span><span class="sxs-lookup"><span data-stu-id="696ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="696ef-132">id</span><span class="sxs-lookup"><span data-stu-id="696ef-132">id</span></span>|<span data-ttu-id="696ef-133">String</span><span class="sxs-lookup"><span data-stu-id="696ef-133">String</span></span>|<span data-ttu-id="696ef-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="696ef-134">Key of the entity.</span></span> <span data-ttu-id="696ef-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="696ef-136">lastModifiedDateTime</span></span>|<span data-ttu-id="696ef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696ef-137">DateTimeOffset</span></span>|<span data-ttu-id="696ef-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="696ef-138">DateTime the object was last modified.</span></span> <span data-ttu-id="696ef-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="696ef-140">roleScopeTagIds</span></span>|<span data-ttu-id="696ef-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="696ef-141">String collection</span></span>|<span data-ttu-id="696ef-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="696ef-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="696ef-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="696ef-144">supportsScopeTags</span></span>|<span data-ttu-id="696ef-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="696ef-145">Boolean</span></span>|<span data-ttu-id="696ef-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="696ef-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="696ef-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="696ef-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="696ef-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="696ef-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="696ef-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="696ef-149">This property is read-only.</span></span> <span data-ttu-id="696ef-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="696ef-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="696ef-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="696ef-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="696ef-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="696ef-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="696ef-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="696ef-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="696ef-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="696ef-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="696ef-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="696ef-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="696ef-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="696ef-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="696ef-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="696ef-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="696ef-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="696ef-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="696ef-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="696ef-163">createdDateTime</span></span>|<span data-ttu-id="696ef-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="696ef-164">DateTimeOffset</span></span>|<span data-ttu-id="696ef-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="696ef-165">DateTime the object was created.</span></span> <span data-ttu-id="696ef-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-167">description</span><span class="sxs-lookup"><span data-stu-id="696ef-167">description</span></span>|<span data-ttu-id="696ef-168">String</span><span class="sxs-lookup"><span data-stu-id="696ef-168">String</span></span>|<span data-ttu-id="696ef-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="696ef-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="696ef-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-171">displayName</span><span class="sxs-lookup"><span data-stu-id="696ef-171">displayName</span></span>|<span data-ttu-id="696ef-172">Строка</span><span class="sxs-lookup"><span data-stu-id="696ef-172">String</span></span>|<span data-ttu-id="696ef-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="696ef-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="696ef-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-175">version</span><span class="sxs-lookup"><span data-stu-id="696ef-175">version</span></span>|<span data-ttu-id="696ef-176">Int32</span><span class="sxs-lookup"><span data-stu-id="696ef-176">Int32</span></span>|<span data-ttu-id="696ef-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="696ef-177">Version of the device configuration.</span></span> <span data-ttu-id="696ef-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="696ef-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="696ef-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="696ef-180">Int32</span><span class="sxs-lookup"><span data-stu-id="696ef-180">Int32</span></span>|<span data-ttu-id="696ef-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="696ef-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="696ef-182">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="696ef-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="696ef-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="696ef-183">keyStorageProvider</span></span>|[<span data-ttu-id="696ef-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="696ef-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="696ef-185">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="696ef-186">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="696ef-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="696ef-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="696ef-187">subjectNameFormat</span></span>|[<span data-ttu-id="696ef-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="696ef-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="696ef-189">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="696ef-190">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="696ef-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="696ef-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="696ef-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="696ef-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="696ef-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="696ef-193">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="696ef-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="696ef-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="696ef-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="696ef-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="696ef-196">Int32</span><span class="sxs-lookup"><span data-stu-id="696ef-196">Int32</span></span>|<span data-ttu-id="696ef-197">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="696ef-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="696ef-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="696ef-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="696ef-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="696ef-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="696ef-200">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="696ef-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="696ef-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="696ef-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="696ef-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="696ef-202">intendedPurpose</span></span>|[<span data-ttu-id="696ef-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="696ef-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="696ef-204">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="696ef-204">Not yet documented.</span></span> <span data-ttu-id="696ef-205">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="696ef-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="696ef-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="696ef-206">Response</span></span>
<span data-ttu-id="696ef-207">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="696ef-207">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="696ef-208">Пример</span><span class="sxs-lookup"><span data-stu-id="696ef-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="696ef-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="696ef-209">Request</span></span>
<span data-ttu-id="696ef-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="696ef-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="696ef-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="696ef-211">Response</span></span>
<span data-ttu-id="696ef-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="696ef-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
  "intendedPurpose": "smimeEncryption"
}
```






