---
title: Создание windows10PkcsCertificateProfile
description: Создание нового объекта windows10PkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f4a33bd1b8190a135d26765578ea3f330de8e0e5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36345003"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="22472-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="22472-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="22472-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22472-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22472-106">Создание нового объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="22472-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22472-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22472-107">Prerequisites</span></span>
<span data-ttu-id="22472-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22472-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22472-110">Permission type</span></span>|<span data-ttu-id="22472-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22472-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22472-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22472-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22472-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22472-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22472-115">Not supported.</span></span>|
|<span data-ttu-id="22472-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22472-116">Application</span></span>|<span data-ttu-id="22472-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22472-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22472-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22472-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22472-119">Request headers</span></span>
|<span data-ttu-id="22472-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22472-120">Header</span></span>|<span data-ttu-id="22472-121">Значение</span><span class="sxs-lookup"><span data-stu-id="22472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22472-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22472-122">Authorization</span></span>|<span data-ttu-id="22472-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22472-124">Accept</span><span class="sxs-lookup"><span data-stu-id="22472-124">Accept</span></span>|<span data-ttu-id="22472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22472-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="22472-126">Request body</span></span>
<span data-ttu-id="22472-127">В тексте запроса добавьте представление объекта windows10PkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22472-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="22472-128">В следующей таблице приведены свойства, необходимые при создании windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="22472-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="22472-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="22472-129">Property</span></span>|<span data-ttu-id="22472-130">Тип</span><span class="sxs-lookup"><span data-stu-id="22472-130">Type</span></span>|<span data-ttu-id="22472-131">Описание</span><span class="sxs-lookup"><span data-stu-id="22472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22472-132">id</span><span class="sxs-lookup"><span data-stu-id="22472-132">id</span></span>|<span data-ttu-id="22472-133">String</span><span class="sxs-lookup"><span data-stu-id="22472-133">String</span></span>|<span data-ttu-id="22472-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22472-134">Key of the entity.</span></span> <span data-ttu-id="22472-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22472-136">lastModifiedDateTime</span></span>|<span data-ttu-id="22472-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22472-137">DateTimeOffset</span></span>|<span data-ttu-id="22472-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="22472-138">DateTime the object was last modified.</span></span> <span data-ttu-id="22472-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22472-140">roleScopeTagIds</span></span>|<span data-ttu-id="22472-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="22472-141">String collection</span></span>|<span data-ttu-id="22472-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="22472-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22472-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="22472-144">supportsScopeTags</span></span>|<span data-ttu-id="22472-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="22472-145">Boolean</span></span>|<span data-ttu-id="22472-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="22472-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22472-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="22472-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22472-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="22472-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22472-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22472-149">This property is read-only.</span></span> <span data-ttu-id="22472-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22472-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22472-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22472-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22472-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22472-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22472-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22472-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22472-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22472-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22472-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22472-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22472-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="22472-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22472-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="22472-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22472-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22472-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22472-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22472-163">createdDateTime</span></span>|<span data-ttu-id="22472-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22472-164">DateTimeOffset</span></span>|<span data-ttu-id="22472-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="22472-165">DateTime the object was created.</span></span> <span data-ttu-id="22472-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-167">description</span><span class="sxs-lookup"><span data-stu-id="22472-167">description</span></span>|<span data-ttu-id="22472-168">String</span><span class="sxs-lookup"><span data-stu-id="22472-168">String</span></span>|<span data-ttu-id="22472-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22472-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22472-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-171">displayName</span><span class="sxs-lookup"><span data-stu-id="22472-171">displayName</span></span>|<span data-ttu-id="22472-172">Строка</span><span class="sxs-lookup"><span data-stu-id="22472-172">String</span></span>|<span data-ttu-id="22472-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22472-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22472-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-175">version</span><span class="sxs-lookup"><span data-stu-id="22472-175">version</span></span>|<span data-ttu-id="22472-176">Int32</span><span class="sxs-lookup"><span data-stu-id="22472-176">Int32</span></span>|<span data-ttu-id="22472-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22472-177">Version of the device configuration.</span></span> <span data-ttu-id="22472-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22472-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22472-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="22472-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="22472-180">Int32</span><span class="sxs-lookup"><span data-stu-id="22472-180">Int32</span></span>|<span data-ttu-id="22472-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="22472-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="22472-182">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="22472-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="22472-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="22472-183">keyStorageProvider</span></span>|[<span data-ttu-id="22472-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="22472-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="22472-185">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22472-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="22472-186">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="22472-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="22472-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="22472-187">subjectNameFormat</span></span>|[<span data-ttu-id="22472-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="22472-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="22472-189">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22472-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="22472-190">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="22472-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="22472-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="22472-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="22472-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="22472-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="22472-193">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22472-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="22472-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="22472-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="22472-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="22472-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="22472-196">Int32</span><span class="sxs-lookup"><span data-stu-id="22472-196">Int32</span></span>|<span data-ttu-id="22472-197">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="22472-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="22472-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="22472-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="22472-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="22472-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="22472-200">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="22472-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="22472-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="22472-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="22472-202">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="22472-202">certificationAuthority</span></span>|<span data-ttu-id="22472-203">String</span><span class="sxs-lookup"><span data-stu-id="22472-203">String</span></span>|<span data-ttu-id="22472-204">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="22472-204">PKCS Certification Authority</span></span>|
|<span data-ttu-id="22472-205">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="22472-205">certificationAuthorityName</span></span>|<span data-ttu-id="22472-206">String</span><span class="sxs-lookup"><span data-stu-id="22472-206">String</span></span>|<span data-ttu-id="22472-207">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="22472-207">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="22472-208">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="22472-208">certificateTemplateName</span></span>|<span data-ttu-id="22472-209">String</span><span class="sxs-lookup"><span data-stu-id="22472-209">String</span></span>|<span data-ttu-id="22472-210">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="22472-210">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="22472-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="22472-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="22472-212">String</span><span class="sxs-lookup"><span data-stu-id="22472-212">String</span></span>|<span data-ttu-id="22472-213">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="22472-213">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="22472-214">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="22472-214">extendedKeyUsages</span></span>|<span data-ttu-id="22472-215">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="22472-215">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="22472-216">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="22472-216">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="22472-217">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="22472-217">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="22472-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="22472-218">Response</span></span>
<span data-ttu-id="22472-219">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="22472-219">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22472-220">Пример</span><span class="sxs-lookup"><span data-stu-id="22472-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="22472-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="22472-221">Request</span></span>
<span data-ttu-id="22472-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22472-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1784

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="22472-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="22472-223">Response</span></span>
<span data-ttu-id="22472-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22472-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1956

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```






