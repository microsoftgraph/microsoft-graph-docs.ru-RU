---
title: Создание iosPkcsCertificateProfile
description: Создайте новый объект iosPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6e310734eceaed295a4e602d126c86485ff5a12
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147835"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="8cc35-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8cc35-103">Create iosPkcsCertificateProfile</span></span>

<span data-ttu-id="8cc35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc35-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cc35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc35-107">Создайте новый [объект iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8cc35-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc35-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cc35-108">Prerequisites</span></span>
<span data-ttu-id="8cc35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cc35-111">Permission type</span></span>|<span data-ttu-id="8cc35-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cc35-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc35-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cc35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc35-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc35-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc35-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cc35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc35-116">Not supported.</span></span>|
|<span data-ttu-id="8cc35-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8cc35-117">Application</span></span>|<span data-ttu-id="8cc35-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc35-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc35-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cc35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8cc35-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8cc35-120">Request headers</span></span>
|<span data-ttu-id="8cc35-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cc35-121">Header</span></span>|<span data-ttu-id="8cc35-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cc35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc35-123">Authorization</span></span>|<span data-ttu-id="8cc35-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cc35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cc35-125">Accept</span></span>|<span data-ttu-id="8cc35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc35-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cc35-127">Request body</span></span>
<span data-ttu-id="8cc35-128">В теле запроса поставляем представление JSON для объекта iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8cc35-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="8cc35-129">В следующей таблице показаны свойства, необходимые при создании iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8cc35-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="8cc35-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc35-130">Property</span></span>|<span data-ttu-id="8cc35-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc35-131">Type</span></span>|<span data-ttu-id="8cc35-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc35-133">id</span><span class="sxs-lookup"><span data-stu-id="8cc35-133">id</span></span>|<span data-ttu-id="8cc35-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-134">String</span></span>|<span data-ttu-id="8cc35-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc35-135">Key of the entity.</span></span> <span data-ttu-id="8cc35-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc35-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc35-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc35-138">DateTimeOffset</span></span>|<span data-ttu-id="8cc35-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc35-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8cc35-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cc35-141">roleScopeTagIds</span></span>|<span data-ttu-id="8cc35-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8cc35-142">String collection</span></span>|<span data-ttu-id="8cc35-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="8cc35-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8cc35-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8cc35-145">supportsScopeTags</span></span>|<span data-ttu-id="8cc35-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc35-146">Boolean</span></span>|<span data-ttu-id="8cc35-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8cc35-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8cc35-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="8cc35-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8cc35-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8cc35-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8cc35-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cc35-150">This property is read-only.</span></span> <span data-ttu-id="8cc35-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8cc35-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8cc35-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8cc35-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8cc35-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8cc35-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8cc35-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8cc35-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8cc35-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8cc35-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8cc35-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8cc35-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8cc35-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8cc35-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8cc35-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8cc35-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8cc35-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8cc35-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8cc35-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc35-164">createdDateTime</span></span>|<span data-ttu-id="8cc35-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc35-165">DateTimeOffset</span></span>|<span data-ttu-id="8cc35-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8cc35-166">DateTime the object was created.</span></span> <span data-ttu-id="8cc35-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-168">description</span><span class="sxs-lookup"><span data-stu-id="8cc35-168">description</span></span>|<span data-ttu-id="8cc35-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-169">String</span></span>|<span data-ttu-id="8cc35-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc35-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8cc35-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc35-172">displayName</span></span>|<span data-ttu-id="8cc35-173">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-173">String</span></span>|<span data-ttu-id="8cc35-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc35-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8cc35-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-176">version</span><span class="sxs-lookup"><span data-stu-id="8cc35-176">version</span></span>|<span data-ttu-id="8cc35-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc35-177">Int32</span></span>|<span data-ttu-id="8cc35-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8cc35-178">Version of the device configuration.</span></span> <span data-ttu-id="8cc35-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8cc35-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8cc35-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="8cc35-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc35-181">Int32</span></span>|<span data-ttu-id="8cc35-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="8cc35-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8cc35-183">Допустимые значения от 1 до 99, унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8cc35-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8cc35-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8cc35-184">subjectNameFormat</span></span>|[<span data-ttu-id="8cc35-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8cc35-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="8cc35-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8cc35-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="8cc35-187">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8cc35-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="8cc35-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="8cc35-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8cc35-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8cc35-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8cc35-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="8cc35-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8cc35-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="8cc35-192">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8cc35-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="8cc35-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="8cc35-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8cc35-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8cc35-195">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc35-195">Int32</span></span>|<span data-ttu-id="8cc35-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8cc35-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8cc35-197">Унаследованный от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8cc35-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8cc35-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8cc35-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8cc35-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8cc35-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="8cc35-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8cc35-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8cc35-201">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8cc35-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8cc35-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8cc35-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8cc35-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="8cc35-203">certificationAuthority</span></span>|<span data-ttu-id="8cc35-204">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-204">String</span></span>|<span data-ttu-id="8cc35-205">Сертификационный орган PKCS.</span><span class="sxs-lookup"><span data-stu-id="8cc35-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="8cc35-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="8cc35-206">certificationAuthorityName</span></span>|<span data-ttu-id="8cc35-207">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-207">String</span></span>|<span data-ttu-id="8cc35-208">Имя органа сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="8cc35-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="8cc35-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="8cc35-209">certificateTemplateName</span></span>|<span data-ttu-id="8cc35-210">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-210">String</span></span>|<span data-ttu-id="8cc35-211">Имя шаблона шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="8cc35-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="8cc35-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8cc35-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8cc35-213">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-213">String</span></span>|<span data-ttu-id="8cc35-214">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="8cc35-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8cc35-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8cc35-215">subjectNameFormatString</span></span>|<span data-ttu-id="8cc35-216">Строка</span><span class="sxs-lookup"><span data-stu-id="8cc35-216">String</span></span>|<span data-ttu-id="8cc35-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="8cc35-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8cc35-218">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="8cc35-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8cc35-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8cc35-219">certificateStore</span></span>|[<span data-ttu-id="8cc35-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8cc35-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="8cc35-221">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="8cc35-221">Target store certificate.</span></span> <span data-ttu-id="8cc35-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="8cc35-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8cc35-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8cc35-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8cc35-224">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="8cc35-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8cc35-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="8cc35-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="8cc35-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8cc35-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc35-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="8cc35-227">Response</span></span>
<span data-ttu-id="8cc35-228">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8cc35-228">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc35-229">Пример</span><span class="sxs-lookup"><span data-stu-id="8cc35-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc35-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cc35-230">Request</span></span>
<span data-ttu-id="8cc35-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cc35-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1824

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="8cc35-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cc35-232">Response</span></span>
<span data-ttu-id="8cc35-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cc35-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1996

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




