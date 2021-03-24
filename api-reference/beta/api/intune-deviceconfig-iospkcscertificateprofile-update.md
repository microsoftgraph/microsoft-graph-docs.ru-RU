---
title: Обновление iosPkcsCertificateProfile
description: Обновление свойств объекта iosPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 555a329f6f36144969627ff5803127310254a610
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147786"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="ce43d-103">Обновление iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ce43d-103">Update iosPkcsCertificateProfile</span></span>

<span data-ttu-id="ce43d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce43d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce43d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce43d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce43d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce43d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce43d-107">Обновление свойств объекта [iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce43d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce43d-108">Prerequisites</span></span>
<span data-ttu-id="ce43d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce43d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce43d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce43d-111">Permission type</span></span>|<span data-ttu-id="ce43d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce43d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce43d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce43d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce43d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce43d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce43d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce43d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce43d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce43d-116">Not supported.</span></span>|
|<span data-ttu-id="ce43d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ce43d-117">Application</span></span>|<span data-ttu-id="ce43d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce43d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce43d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce43d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ce43d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce43d-120">Request headers</span></span>
|<span data-ttu-id="ce43d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce43d-121">Header</span></span>|<span data-ttu-id="ce43d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce43d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce43d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce43d-123">Authorization</span></span>|<span data-ttu-id="ce43d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce43d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce43d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce43d-125">Accept</span></span>|<span data-ttu-id="ce43d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce43d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce43d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce43d-127">Request body</span></span>
<span data-ttu-id="ce43d-128">В теле запроса поставляем представление JSON для [объекта iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="ce43d-129">В следующей таблице показаны свойства, необходимые при создании [iosPkcsCertificateProfile.](../resources/intune-deviceconfig-iospkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="ce43d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce43d-130">Property</span></span>|<span data-ttu-id="ce43d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce43d-131">Type</span></span>|<span data-ttu-id="ce43d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce43d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce43d-133">id</span><span class="sxs-lookup"><span data-stu-id="ce43d-133">id</span></span>|<span data-ttu-id="ce43d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-134">String</span></span>|<span data-ttu-id="ce43d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce43d-135">Key of the entity.</span></span> <span data-ttu-id="ce43d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce43d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce43d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce43d-138">DateTimeOffset</span></span>|<span data-ttu-id="ce43d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ce43d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce43d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce43d-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce43d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce43d-142">String collection</span></span>|<span data-ttu-id="ce43d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ce43d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce43d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce43d-145">supportsScopeTags</span></span>|<span data-ttu-id="ce43d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce43d-146">Boolean</span></span>|<span data-ttu-id="ce43d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ce43d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce43d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ce43d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce43d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ce43d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce43d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce43d-150">This property is read-only.</span></span> <span data-ttu-id="ce43d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce43d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce43d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce43d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce43d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce43d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce43d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce43d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce43d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce43d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce43d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce43d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce43d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce43d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce43d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce43d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce43d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ce43d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce43d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce43d-164">createdDateTime</span></span>|<span data-ttu-id="ce43d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce43d-165">DateTimeOffset</span></span>|<span data-ttu-id="ce43d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ce43d-166">DateTime the object was created.</span></span> <span data-ttu-id="ce43d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-168">description</span><span class="sxs-lookup"><span data-stu-id="ce43d-168">description</span></span>|<span data-ttu-id="ce43d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-169">String</span></span>|<span data-ttu-id="ce43d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce43d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce43d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ce43d-172">displayName</span></span>|<span data-ttu-id="ce43d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-173">String</span></span>|<span data-ttu-id="ce43d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce43d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce43d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-176">version</span><span class="sxs-lookup"><span data-stu-id="ce43d-176">version</span></span>|<span data-ttu-id="ce43d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ce43d-177">Int32</span></span>|<span data-ttu-id="ce43d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ce43d-178">Version of the device configuration.</span></span> <span data-ttu-id="ce43d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce43d-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="ce43d-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="ce43d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="ce43d-181">Int32</span></span>|<span data-ttu-id="ce43d-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce43d-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ce43d-183">Допустимые значения от 1 до 99, унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce43d-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce43d-184">subjectNameFormat</span></span>|[<span data-ttu-id="ce43d-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ce43d-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="ce43d-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce43d-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="ce43d-187">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ce43d-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="ce43d-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="ce43d-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce43d-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ce43d-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ce43d-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="ce43d-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce43d-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="ce43d-192">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ce43d-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="ce43d-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="ce43d-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ce43d-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ce43d-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ce43d-195">Int32</span></span>|<span data-ttu-id="ce43d-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce43d-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ce43d-197">Унаследованный от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ce43d-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce43d-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ce43d-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ce43d-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="ce43d-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ce43d-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ce43d-201">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ce43d-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ce43d-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ce43d-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ce43d-203">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="ce43d-203">certificationAuthority</span></span>|<span data-ttu-id="ce43d-204">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-204">String</span></span>|<span data-ttu-id="ce43d-205">Сертификационный орган PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce43d-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="ce43d-206">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="ce43d-206">certificationAuthorityName</span></span>|<span data-ttu-id="ce43d-207">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-207">String</span></span>|<span data-ttu-id="ce43d-208">Имя органа сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce43d-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="ce43d-209">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="ce43d-209">certificateTemplateName</span></span>|<span data-ttu-id="ce43d-210">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-210">String</span></span>|<span data-ttu-id="ce43d-211">Имя шаблона шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="ce43d-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="ce43d-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ce43d-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ce43d-213">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-213">String</span></span>|<span data-ttu-id="ce43d-214">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="ce43d-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ce43d-215">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ce43d-215">subjectNameFormatString</span></span>|<span data-ttu-id="ce43d-216">Строка</span><span class="sxs-lookup"><span data-stu-id="ce43d-216">String</span></span>|<span data-ttu-id="ce43d-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="ce43d-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ce43d-218">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="ce43d-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ce43d-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ce43d-219">certificateStore</span></span>|[<span data-ttu-id="ce43d-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ce43d-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="ce43d-221">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="ce43d-221">Target store certificate.</span></span> <span data-ttu-id="ce43d-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="ce43d-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ce43d-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ce43d-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ce43d-224">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="ce43d-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ce43d-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="ce43d-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ce43d-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ce43d-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ce43d-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce43d-227">Response</span></span>
<span data-ttu-id="ce43d-228">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce43d-228">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce43d-229">Пример</span><span class="sxs-lookup"><span data-stu-id="ce43d-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce43d-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce43d-230">Request</span></span>
<span data-ttu-id="ce43d-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce43d-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ce43d-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce43d-232">Response</span></span>
<span data-ttu-id="ce43d-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce43d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




