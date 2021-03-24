---
title: Обновление iosScepCertificateProfile
description: Обновление свойств объекта iosScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 48bda5974ac7368309e2d7724a350005125c8450
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131479"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="42f60-103">Обновление iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="42f60-103">Update iosScepCertificateProfile</span></span>

<span data-ttu-id="42f60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42f60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42f60-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42f60-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42f60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42f60-107">Обновление свойств объекта [iosScepCertificateProfile.](../resources/intune-deviceconfig-iosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-107">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42f60-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="42f60-108">Prerequisites</span></span>
<span data-ttu-id="42f60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42f60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42f60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42f60-111">Permission type</span></span>|<span data-ttu-id="42f60-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42f60-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42f60-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42f60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42f60-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f60-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42f60-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42f60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42f60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42f60-116">Not supported.</span></span>|
|<span data-ttu-id="42f60-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="42f60-117">Application</span></span>|<span data-ttu-id="42f60-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42f60-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42f60-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42f60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="42f60-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42f60-120">Request headers</span></span>
|<span data-ttu-id="42f60-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42f60-121">Header</span></span>|<span data-ttu-id="42f60-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42f60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42f60-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="42f60-123">Authorization</span></span>|<span data-ttu-id="42f60-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42f60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42f60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42f60-125">Accept</span></span>|<span data-ttu-id="42f60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42f60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42f60-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42f60-127">Request body</span></span>
<span data-ttu-id="42f60-128">В теле запроса поставляем представление JSON для [объекта iosScepCertificateProfile.](../resources/intune-deviceconfig-iosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-128">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="42f60-129">В следующей таблице показаны свойства, необходимые при создании [iosScepCertificateProfile.](../resources/intune-deviceconfig-iosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-129">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="42f60-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42f60-130">Property</span></span>|<span data-ttu-id="42f60-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42f60-131">Type</span></span>|<span data-ttu-id="42f60-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42f60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42f60-133">id</span><span class="sxs-lookup"><span data-stu-id="42f60-133">id</span></span>|<span data-ttu-id="42f60-134">Строка</span><span class="sxs-lookup"><span data-stu-id="42f60-134">String</span></span>|<span data-ttu-id="42f60-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42f60-135">Key of the entity.</span></span> <span data-ttu-id="42f60-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42f60-137">lastModifiedDateTime</span></span>|<span data-ttu-id="42f60-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42f60-138">DateTimeOffset</span></span>|<span data-ttu-id="42f60-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42f60-139">DateTime the object was last modified.</span></span> <span data-ttu-id="42f60-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42f60-141">roleScopeTagIds</span></span>|<span data-ttu-id="42f60-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42f60-142">String collection</span></span>|<span data-ttu-id="42f60-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="42f60-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42f60-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="42f60-145">supportsScopeTags</span></span>|<span data-ttu-id="42f60-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="42f60-146">Boolean</span></span>|<span data-ttu-id="42f60-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="42f60-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42f60-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="42f60-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42f60-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="42f60-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42f60-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42f60-150">This property is read-only.</span></span> <span data-ttu-id="42f60-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42f60-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="42f60-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42f60-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="42f60-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42f60-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="42f60-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42f60-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="42f60-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42f60-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="42f60-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42f60-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="42f60-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42f60-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="42f60-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42f60-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="42f60-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42f60-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="42f60-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42f60-164">createdDateTime</span></span>|<span data-ttu-id="42f60-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42f60-165">DateTimeOffset</span></span>|<span data-ttu-id="42f60-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="42f60-166">DateTime the object was created.</span></span> <span data-ttu-id="42f60-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-168">description</span><span class="sxs-lookup"><span data-stu-id="42f60-168">description</span></span>|<span data-ttu-id="42f60-169">Строка</span><span class="sxs-lookup"><span data-stu-id="42f60-169">String</span></span>|<span data-ttu-id="42f60-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f60-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42f60-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-172">displayName</span><span class="sxs-lookup"><span data-stu-id="42f60-172">displayName</span></span>|<span data-ttu-id="42f60-173">Строка</span><span class="sxs-lookup"><span data-stu-id="42f60-173">String</span></span>|<span data-ttu-id="42f60-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f60-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42f60-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-176">version</span><span class="sxs-lookup"><span data-stu-id="42f60-176">version</span></span>|<span data-ttu-id="42f60-177">Int32</span><span class="sxs-lookup"><span data-stu-id="42f60-177">Int32</span></span>|<span data-ttu-id="42f60-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42f60-178">Version of the device configuration.</span></span> <span data-ttu-id="42f60-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42f60-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="42f60-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="42f60-181">Int32</span><span class="sxs-lookup"><span data-stu-id="42f60-181">Int32</span></span>|<span data-ttu-id="42f60-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="42f60-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="42f60-183">Допустимые значения от 1 до 99, унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="42f60-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="42f60-184">subjectNameFormat</span></span>|[<span data-ttu-id="42f60-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="42f60-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="42f60-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="42f60-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="42f60-187">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="42f60-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="42f60-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="42f60-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="42f60-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="42f60-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="42f60-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="42f60-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="42f60-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="42f60-192">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="42f60-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="42f60-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="42f60-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="42f60-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="42f60-195">Int32</span><span class="sxs-lookup"><span data-stu-id="42f60-195">Int32</span></span>|<span data-ttu-id="42f60-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="42f60-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="42f60-197">Унаследованный от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="42f60-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="42f60-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="42f60-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="42f60-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="42f60-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="42f60-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="42f60-201">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="42f60-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="42f60-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="42f60-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="42f60-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="42f60-203">scepServerUrls</span></span>|<span data-ttu-id="42f60-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42f60-204">String collection</span></span>|<span data-ttu-id="42f60-205">URL-адрес сервера SCEP Server (s).</span><span class="sxs-lookup"><span data-stu-id="42f60-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="42f60-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="42f60-206">subjectNameFormatString</span></span>|<span data-ttu-id="42f60-207">Строка</span><span class="sxs-lookup"><span data-stu-id="42f60-207">String</span></span>|<span data-ttu-id="42f60-208">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="42f60-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="42f60-209">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="42f60-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="42f60-210">keyUsage</span><span class="sxs-lookup"><span data-stu-id="42f60-210">keyUsage</span></span>|[<span data-ttu-id="42f60-211">keyUsages</span><span class="sxs-lookup"><span data-stu-id="42f60-211">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="42f60-212">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="42f60-212">SCEP Key Usage.</span></span> <span data-ttu-id="42f60-213">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="42f60-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="42f60-214">keySize</span><span class="sxs-lookup"><span data-stu-id="42f60-214">keySize</span></span>|[<span data-ttu-id="42f60-215">keySize</span><span class="sxs-lookup"><span data-stu-id="42f60-215">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="42f60-216">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="42f60-216">SCEP Key Size.</span></span> <span data-ttu-id="42f60-217">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="42f60-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="42f60-218">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="42f60-218">extendedKeyUsages</span></span>|<span data-ttu-id="42f60-219">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-219">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="42f60-220">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="42f60-220">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="42f60-221">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="42f60-221">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="42f60-222">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="42f60-222">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="42f60-223">Строка</span><span class="sxs-lookup"><span data-stu-id="42f60-223">String</span></span>|<span data-ttu-id="42f60-224">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="42f60-224">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="42f60-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="42f60-225">certificateStore</span></span>|[<span data-ttu-id="42f60-226">certificateStore</span><span class="sxs-lookup"><span data-stu-id="42f60-226">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="42f60-227">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="42f60-227">Target store certificate.</span></span> <span data-ttu-id="42f60-228">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="42f60-228">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="42f60-229">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="42f60-229">customSubjectAlternativeNames</span></span>|<span data-ttu-id="42f60-230">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="42f60-230">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="42f60-231">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="42f60-231">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="42f60-232">Переменная OnPremisesUserPrincipalName является поддержкой, а также другими, задокументированными здесь: https://go.microsoft.com/fwlink/?LinkId=2027630 .</span><span class="sxs-lookup"><span data-stu-id="42f60-232">The OnPremisesUserPrincipalName variable is support as well as others documented here: https://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="42f60-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="42f60-233">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="42f60-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="42f60-234">Response</span></span>
<span data-ttu-id="42f60-235">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42f60-235">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42f60-236">Пример</span><span class="sxs-lookup"><span data-stu-id="42f60-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="42f60-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="42f60-237">Request</span></span>
<span data-ttu-id="42f60-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42f60-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="42f60-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="42f60-239">Response</span></span>
<span data-ttu-id="42f60-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42f60-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




