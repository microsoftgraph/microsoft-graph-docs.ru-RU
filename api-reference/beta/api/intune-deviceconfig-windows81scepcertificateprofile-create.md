---
title: Создание windows81SCEPCertificateProfile
description: Создание нового объекта windows81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8710f522bcc93bbcf453ed312977b60f3fb1ca13
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947052"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="bde24-103">Создание windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="bde24-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="bde24-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bde24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bde24-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bde24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bde24-106">Создание нового объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bde24-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bde24-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bde24-107">Prerequisites</span></span>
<span data-ttu-id="bde24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bde24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bde24-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bde24-110">Permission type</span></span>|<span data-ttu-id="bde24-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bde24-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bde24-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bde24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bde24-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bde24-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bde24-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bde24-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bde24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bde24-115">Not supported.</span></span>|
|<span data-ttu-id="bde24-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bde24-116">Application</span></span>|<span data-ttu-id="bde24-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bde24-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bde24-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bde24-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bde24-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bde24-119">Request headers</span></span>
|<span data-ttu-id="bde24-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bde24-120">Header</span></span>|<span data-ttu-id="bde24-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bde24-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bde24-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bde24-122">Authorization</span></span>|<span data-ttu-id="bde24-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bde24-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bde24-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bde24-124">Accept</span></span>|<span data-ttu-id="bde24-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bde24-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bde24-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bde24-126">Request body</span></span>
<span data-ttu-id="bde24-127">В тексте запроса добавьте представление объекта windows81SCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bde24-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="bde24-128">В следующей таблице приведены свойства, необходимые при создании windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="bde24-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="bde24-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bde24-129">Property</span></span>|<span data-ttu-id="bde24-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bde24-130">Type</span></span>|<span data-ttu-id="bde24-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bde24-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bde24-132">id</span><span class="sxs-lookup"><span data-stu-id="bde24-132">id</span></span>|<span data-ttu-id="bde24-133">String</span><span class="sxs-lookup"><span data-stu-id="bde24-133">String</span></span>|<span data-ttu-id="bde24-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bde24-134">Key of the entity.</span></span> <span data-ttu-id="bde24-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bde24-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bde24-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bde24-137">DateTimeOffset</span></span>|<span data-ttu-id="bde24-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bde24-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bde24-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bde24-140">roleScopeTagIds</span></span>|<span data-ttu-id="bde24-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bde24-141">String collection</span></span>|<span data-ttu-id="bde24-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bde24-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bde24-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bde24-144">supportsScopeTags</span></span>|<span data-ttu-id="bde24-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bde24-145">Boolean</span></span>|<span data-ttu-id="bde24-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bde24-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bde24-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bde24-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bde24-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bde24-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bde24-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bde24-149">This property is read-only.</span></span> <span data-ttu-id="bde24-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bde24-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bde24-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bde24-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bde24-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bde24-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bde24-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bde24-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bde24-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bde24-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bde24-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bde24-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bde24-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bde24-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bde24-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bde24-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bde24-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="bde24-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bde24-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bde24-163">createdDateTime</span></span>|<span data-ttu-id="bde24-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bde24-164">DateTimeOffset</span></span>|<span data-ttu-id="bde24-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bde24-165">DateTime the object was created.</span></span> <span data-ttu-id="bde24-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-167">description</span><span class="sxs-lookup"><span data-stu-id="bde24-167">description</span></span>|<span data-ttu-id="bde24-168">String</span><span class="sxs-lookup"><span data-stu-id="bde24-168">String</span></span>|<span data-ttu-id="bde24-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bde24-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bde24-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-171">displayName</span><span class="sxs-lookup"><span data-stu-id="bde24-171">displayName</span></span>|<span data-ttu-id="bde24-172">Строка</span><span class="sxs-lookup"><span data-stu-id="bde24-172">String</span></span>|<span data-ttu-id="bde24-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bde24-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bde24-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-175">version</span><span class="sxs-lookup"><span data-stu-id="bde24-175">version</span></span>|<span data-ttu-id="bde24-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bde24-176">Int32</span></span>|<span data-ttu-id="bde24-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bde24-177">Version of the device configuration.</span></span> <span data-ttu-id="bde24-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bde24-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="bde24-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="bde24-180">Int32</span><span class="sxs-lookup"><span data-stu-id="bde24-180">Int32</span></span>|<span data-ttu-id="bde24-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="bde24-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="bde24-182">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bde24-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="bde24-183">keyStorageProvider</span></span>|[<span data-ttu-id="bde24-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="bde24-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="bde24-185">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bde24-186">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="bde24-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="bde24-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bde24-187">subjectNameFormat</span></span>|[<span data-ttu-id="bde24-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="bde24-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="bde24-189">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bde24-190">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="bde24-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="bde24-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bde24-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="bde24-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bde24-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bde24-193">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bde24-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="bde24-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bde24-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="bde24-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="bde24-196">Int32</span><span class="sxs-lookup"><span data-stu-id="bde24-196">Int32</span></span>|<span data-ttu-id="bde24-197">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="bde24-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bde24-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="bde24-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="bde24-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="bde24-200">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="bde24-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="bde24-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="bde24-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="bde24-202">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="bde24-202">extendedKeyUsages</span></span>|<span data-ttu-id="bde24-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="bde24-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="bde24-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="bde24-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bde24-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bde24-206">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-206">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="bde24-207">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="bde24-207">customSubjectAlternativeNames</span></span>|<span data-ttu-id="bde24-208">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-208">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="bde24-209">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="bde24-209">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="bde24-210">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bde24-210">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bde24-211">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="bde24-211">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="bde24-212">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="bde24-212">scepServerUrls</span></span>|<span data-ttu-id="bde24-213">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bde24-213">String collection</span></span>|<span data-ttu-id="bde24-214">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="bde24-214">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="bde24-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="bde24-215">subjectNameFormatString</span></span>|<span data-ttu-id="bde24-216">Строка</span><span class="sxs-lookup"><span data-stu-id="bde24-216">String</span></span>|<span data-ttu-id="bde24-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="bde24-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="bde24-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="bde24-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="bde24-219">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="bde24-219">keyUsage</span></span>|[<span data-ttu-id="bde24-220">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="bde24-220">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="bde24-221">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="bde24-221">SCEP Key Usage.</span></span> <span data-ttu-id="bde24-222">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="bde24-222">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="bde24-223">keySize</span><span class="sxs-lookup"><span data-stu-id="bde24-223">keySize</span></span>|[<span data-ttu-id="bde24-224">keySize</span><span class="sxs-lookup"><span data-stu-id="bde24-224">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="bde24-225">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="bde24-225">SCEP Key Size.</span></span> <span data-ttu-id="bde24-226">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="bde24-226">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="bde24-227">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="bde24-227">hashAlgorithm</span></span>|[<span data-ttu-id="bde24-228">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="bde24-228">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="bde24-229">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="bde24-229">SCEP Hash Algorithm.</span></span> <span data-ttu-id="bde24-230">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="bde24-230">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="bde24-231">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="bde24-231">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="bde24-232">Строка</span><span class="sxs-lookup"><span data-stu-id="bde24-232">String</span></span>|<span data-ttu-id="bde24-233">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="bde24-233">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="bde24-234">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bde24-234">certificateStore</span></span>|[<span data-ttu-id="bde24-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="bde24-235">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="bde24-236">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde24-236">Target store certificate.</span></span> <span data-ttu-id="bde24-237">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="bde24-237">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="bde24-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="bde24-238">Response</span></span>
<span data-ttu-id="bde24-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bde24-239">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bde24-240">Пример</span><span class="sxs-lookup"><span data-stu-id="bde24-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="bde24-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="bde24-241">Request</span></span>
<span data-ttu-id="bde24-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bde24-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="bde24-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="bde24-243">Response</span></span>
<span data-ttu-id="bde24-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bde24-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```





