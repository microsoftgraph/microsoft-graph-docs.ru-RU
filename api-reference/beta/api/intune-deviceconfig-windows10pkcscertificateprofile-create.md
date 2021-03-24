---
title: Создание windows10PkcsCertificateProfile
description: Создайте новый объект Windows10PkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cab742e45413a038b4ddfa79e662ce6993675323
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127538"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="96387-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="96387-103">Create windows10PkcsCertificateProfile</span></span>

<span data-ttu-id="96387-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96387-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96387-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96387-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96387-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="96387-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96387-107">Создайте [новый объект Windows10PkcsCertificateProfile.](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="96387-107">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96387-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="96387-108">Prerequisites</span></span>
<span data-ttu-id="96387-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96387-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96387-111">Permission type</span></span>|<span data-ttu-id="96387-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96387-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96387-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96387-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96387-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96387-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96387-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96387-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96387-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96387-116">Not supported.</span></span>|
|<span data-ttu-id="96387-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="96387-117">Application</span></span>|<span data-ttu-id="96387-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96387-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96387-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96387-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96387-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="96387-120">Request headers</span></span>
|<span data-ttu-id="96387-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96387-121">Header</span></span>|<span data-ttu-id="96387-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96387-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96387-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96387-123">Authorization</span></span>|<span data-ttu-id="96387-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96387-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96387-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96387-125">Accept</span></span>|<span data-ttu-id="96387-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96387-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96387-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96387-127">Request body</span></span>
<span data-ttu-id="96387-128">В теле запроса поставляем представление JSON для объекта Windows10PkkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="96387-128">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="96387-129">В следующей таблице показаны свойства, необходимые при создании windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="96387-129">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="96387-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="96387-130">Property</span></span>|<span data-ttu-id="96387-131">Тип</span><span class="sxs-lookup"><span data-stu-id="96387-131">Type</span></span>|<span data-ttu-id="96387-132">Описание</span><span class="sxs-lookup"><span data-stu-id="96387-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96387-133">id</span><span class="sxs-lookup"><span data-stu-id="96387-133">id</span></span>|<span data-ttu-id="96387-134">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-134">String</span></span>|<span data-ttu-id="96387-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="96387-135">Key of the entity.</span></span> <span data-ttu-id="96387-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96387-137">lastModifiedDateTime</span></span>|<span data-ttu-id="96387-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96387-138">DateTimeOffset</span></span>|<span data-ttu-id="96387-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="96387-139">DateTime the object was last modified.</span></span> <span data-ttu-id="96387-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="96387-141">roleScopeTagIds</span></span>|<span data-ttu-id="96387-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="96387-142">String collection</span></span>|<span data-ttu-id="96387-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="96387-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="96387-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="96387-145">supportsScopeTags</span></span>|<span data-ttu-id="96387-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="96387-146">Boolean</span></span>|<span data-ttu-id="96387-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="96387-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="96387-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="96387-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="96387-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="96387-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="96387-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96387-150">This property is read-only.</span></span> <span data-ttu-id="96387-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96387-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="96387-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="96387-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="96387-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96387-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="96387-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96387-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="96387-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="96387-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="96387-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96387-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="96387-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="96387-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="96387-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="96387-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="96387-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="96387-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="96387-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96387-164">createdDateTime</span></span>|<span data-ttu-id="96387-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96387-165">DateTimeOffset</span></span>|<span data-ttu-id="96387-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="96387-166">DateTime the object was created.</span></span> <span data-ttu-id="96387-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-168">description</span><span class="sxs-lookup"><span data-stu-id="96387-168">description</span></span>|<span data-ttu-id="96387-169">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-169">String</span></span>|<span data-ttu-id="96387-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96387-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96387-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-172">displayName</span><span class="sxs-lookup"><span data-stu-id="96387-172">displayName</span></span>|<span data-ttu-id="96387-173">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-173">String</span></span>|<span data-ttu-id="96387-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96387-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96387-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-176">version</span><span class="sxs-lookup"><span data-stu-id="96387-176">version</span></span>|<span data-ttu-id="96387-177">Int32</span><span class="sxs-lookup"><span data-stu-id="96387-177">Int32</span></span>|<span data-ttu-id="96387-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="96387-178">Version of the device configuration.</span></span> <span data-ttu-id="96387-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="96387-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96387-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="96387-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="96387-181">Int32</span><span class="sxs-lookup"><span data-stu-id="96387-181">Int32</span></span>|<span data-ttu-id="96387-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="96387-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="96387-183">Допустимые значения от 1 до 99, унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="96387-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="96387-184">keyStorageProvider</span></span>|[<span data-ttu-id="96387-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="96387-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="96387-186">Поставщик ключей для хранения данных (KSP), унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="96387-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="96387-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="96387-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="96387-188">subjectNameFormat</span></span>|[<span data-ttu-id="96387-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="96387-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="96387-190">Формат имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="96387-191">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="96387-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="96387-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="96387-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="96387-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="96387-193">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="96387-194">Тип альтернативного имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="96387-195">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="96387-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="96387-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="96387-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="96387-197">Int32</span><span class="sxs-lookup"><span data-stu-id="96387-197">Int32</span></span>|<span data-ttu-id="96387-198">Значение для периода действия сертификата, унаследованной от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="96387-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="96387-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="96387-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="96387-200">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="96387-201">Масштабировать период действия сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="96387-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="96387-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="96387-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="96387-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="96387-203">certificationAuthority</span></span>|<span data-ttu-id="96387-204">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-204">String</span></span>|<span data-ttu-id="96387-205">Сертификационный орган PKCS</span><span class="sxs-lookup"><span data-stu-id="96387-205">PKCS Certification Authority</span></span>|
|<span data-ttu-id="96387-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="96387-206">certificationAuthorityName</span></span>|<span data-ttu-id="96387-207">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-207">String</span></span>|<span data-ttu-id="96387-208">Имя органа сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="96387-208">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="96387-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="96387-209">certificateTemplateName</span></span>|<span data-ttu-id="96387-210">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-210">String</span></span>|<span data-ttu-id="96387-211">Имя шаблона шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="96387-211">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="96387-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="96387-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="96387-213">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-213">String</span></span>|<span data-ttu-id="96387-214">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="96387-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="96387-215">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="96387-215">extendedKeyUsages</span></span>|<span data-ttu-id="96387-216">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="96387-216">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="96387-217">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="96387-217">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="96387-218">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="96387-218">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="96387-219">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="96387-219">subjectNameFormatString</span></span>|<span data-ttu-id="96387-220">Строка</span><span class="sxs-lookup"><span data-stu-id="96387-220">String</span></span>|<span data-ttu-id="96387-221">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="96387-221">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="96387-222">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="96387-222">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="96387-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="96387-223">certificateStore</span></span>|[<span data-ttu-id="96387-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="96387-224">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="96387-225">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="96387-225">Target store certificate.</span></span> <span data-ttu-id="96387-226">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="96387-226">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="96387-227">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="96387-227">customSubjectAlternativeNames</span></span>|<span data-ttu-id="96387-228">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="96387-228">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="96387-229">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="96387-229">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="96387-230">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="96387-230">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="96387-231">Ответ</span><span class="sxs-lookup"><span data-stu-id="96387-231">Response</span></span>
<span data-ttu-id="96387-232">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект Windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="96387-232">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96387-233">Пример</span><span class="sxs-lookup"><span data-stu-id="96387-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="96387-234">Запрос</span><span class="sxs-lookup"><span data-stu-id="96387-234">Request</span></span>
<span data-ttu-id="96387-235">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96387-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2074

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
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="96387-236">Отклик</span><span class="sxs-lookup"><span data-stu-id="96387-236">Response</span></span>
<span data-ttu-id="96387-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="96387-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2246

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
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




