---
title: Создание windows10ImportedPFXCertificateProfile
description: Создание нового объекта windows10ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 917a1a4d54878a82b068678193df4a6c40389327
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345143"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="c0231-103">Создание windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c0231-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="c0231-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0231-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0231-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0231-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0231-106">Создание нового объекта [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c0231-106">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0231-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c0231-107">Prerequisites</span></span>
<span data-ttu-id="c0231-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0231-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0231-110">Permission type</span></span>|<span data-ttu-id="c0231-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0231-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0231-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0231-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c0231-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0231-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c0231-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0231-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0231-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0231-115">Not supported.</span></span>|
|<span data-ttu-id="c0231-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0231-116">Application</span></span>|<span data-ttu-id="c0231-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0231-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0231-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0231-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0231-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0231-119">Request headers</span></span>
|<span data-ttu-id="c0231-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0231-120">Header</span></span>|<span data-ttu-id="c0231-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c0231-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0231-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0231-122">Authorization</span></span>|<span data-ttu-id="c0231-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0231-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0231-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c0231-124">Accept</span></span>|<span data-ttu-id="c0231-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c0231-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0231-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0231-126">Request body</span></span>
<span data-ttu-id="c0231-127">В тексте запроса добавьте представление объекта windows10ImportedPFXCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0231-127">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="c0231-128">В следующей таблице приведены свойства, необходимые при создании windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c0231-128">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="c0231-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0231-129">Property</span></span>|<span data-ttu-id="c0231-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c0231-130">Type</span></span>|<span data-ttu-id="c0231-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c0231-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0231-132">id</span><span class="sxs-lookup"><span data-stu-id="c0231-132">id</span></span>|<span data-ttu-id="c0231-133">String</span><span class="sxs-lookup"><span data-stu-id="c0231-133">String</span></span>|<span data-ttu-id="c0231-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c0231-134">Key of the entity.</span></span> <span data-ttu-id="c0231-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0231-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c0231-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0231-137">DateTimeOffset</span></span>|<span data-ttu-id="c0231-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c0231-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c0231-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c0231-140">roleScopeTagIds</span></span>|<span data-ttu-id="c0231-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c0231-141">String collection</span></span>|<span data-ttu-id="c0231-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c0231-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c0231-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c0231-144">supportsScopeTags</span></span>|<span data-ttu-id="c0231-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0231-145">Boolean</span></span>|<span data-ttu-id="c0231-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c0231-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c0231-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c0231-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c0231-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c0231-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c0231-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0231-149">This property is read-only.</span></span> <span data-ttu-id="c0231-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0231-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c0231-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c0231-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c0231-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c0231-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c0231-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0231-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c0231-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c0231-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c0231-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c0231-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c0231-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c0231-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c0231-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c0231-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c0231-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c0231-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c0231-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0231-163">createdDateTime</span></span>|<span data-ttu-id="c0231-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0231-164">DateTimeOffset</span></span>|<span data-ttu-id="c0231-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c0231-165">DateTime the object was created.</span></span> <span data-ttu-id="c0231-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-167">description</span><span class="sxs-lookup"><span data-stu-id="c0231-167">description</span></span>|<span data-ttu-id="c0231-168">String</span><span class="sxs-lookup"><span data-stu-id="c0231-168">String</span></span>|<span data-ttu-id="c0231-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0231-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c0231-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c0231-171">displayName</span></span>|<span data-ttu-id="c0231-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c0231-172">String</span></span>|<span data-ttu-id="c0231-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0231-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c0231-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-175">version</span><span class="sxs-lookup"><span data-stu-id="c0231-175">version</span></span>|<span data-ttu-id="c0231-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c0231-176">Int32</span></span>|<span data-ttu-id="c0231-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c0231-177">Version of the device configuration.</span></span> <span data-ttu-id="c0231-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c0231-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c0231-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c0231-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c0231-180">Int32</span></span>|<span data-ttu-id="c0231-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c0231-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c0231-182">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c0231-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c0231-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="c0231-183">keyStorageProvider</span></span>|[<span data-ttu-id="c0231-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="c0231-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c0231-185">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c0231-186">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c0231-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c0231-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c0231-187">subjectNameFormat</span></span>|[<span data-ttu-id="c0231-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c0231-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c0231-189">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c0231-190">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c0231-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c0231-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c0231-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c0231-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c0231-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c0231-193">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c0231-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c0231-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c0231-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c0231-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c0231-196">Int32</span><span class="sxs-lookup"><span data-stu-id="c0231-196">Int32</span></span>|<span data-ttu-id="c0231-197">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c0231-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c0231-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c0231-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c0231-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c0231-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c0231-200">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c0231-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c0231-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c0231-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c0231-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c0231-202">intendedPurpose</span></span>|[<span data-ttu-id="c0231-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c0231-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c0231-204">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c0231-204">Not yet documented.</span></span> <span data-ttu-id="c0231-205">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="c0231-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c0231-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0231-206">Response</span></span>
<span data-ttu-id="c0231-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0231-207">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0231-208">Пример</span><span class="sxs-lookup"><span data-stu-id="c0231-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0231-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0231-209">Request</span></span>
<span data-ttu-id="c0231-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0231-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1359

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="c0231-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0231-211">Response</span></span>
<span data-ttu-id="c0231-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0231-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1531

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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






