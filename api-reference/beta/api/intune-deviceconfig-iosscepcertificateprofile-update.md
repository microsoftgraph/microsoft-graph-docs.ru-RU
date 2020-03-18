---
title: Обновление iosScepCertificateProfile
description: Обновление свойств объекта iosScepCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa2a2db3a79a23f4030dd4e668b882f0e343e09e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42749517"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="b5543-103">Обновление iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b5543-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="b5543-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5543-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5543-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5543-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5543-106">Обновление свойств объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b5543-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5543-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b5543-107">Prerequisites</span></span>
<span data-ttu-id="b5543-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5543-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5543-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5543-110">Permission type</span></span>|<span data-ttu-id="b5543-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5543-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5543-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5543-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5543-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5543-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5543-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5543-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5543-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5543-115">Not supported.</span></span>|
|<span data-ttu-id="b5543-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b5543-116">Application</span></span>|<span data-ttu-id="b5543-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5543-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5543-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5543-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5543-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5543-119">Request headers</span></span>
|<span data-ttu-id="b5543-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5543-120">Header</span></span>|<span data-ttu-id="b5543-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b5543-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5543-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5543-122">Authorization</span></span>|<span data-ttu-id="b5543-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5543-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5543-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b5543-124">Accept</span></span>|<span data-ttu-id="b5543-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5543-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5543-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5543-126">Request body</span></span>
<span data-ttu-id="b5543-127">В тексте запроса добавьте представление объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5543-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="b5543-128">В следующей таблице приведены свойства, необходимые при создании [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="b5543-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5543-129">Property</span></span>|<span data-ttu-id="b5543-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b5543-130">Type</span></span>|<span data-ttu-id="b5543-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b5543-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5543-132">id</span><span class="sxs-lookup"><span data-stu-id="b5543-132">id</span></span>|<span data-ttu-id="b5543-133">String</span><span class="sxs-lookup"><span data-stu-id="b5543-133">String</span></span>|<span data-ttu-id="b5543-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b5543-134">Key of the entity.</span></span> <span data-ttu-id="b5543-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5543-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b5543-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5543-137">DateTimeOffset</span></span>|<span data-ttu-id="b5543-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b5543-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b5543-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5543-140">roleScopeTagIds</span></span>|<span data-ttu-id="b5543-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5543-141">String collection</span></span>|<span data-ttu-id="b5543-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b5543-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5543-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b5543-144">supportsScopeTags</span></span>|<span data-ttu-id="b5543-145">Логический</span><span class="sxs-lookup"><span data-stu-id="b5543-145">Boolean</span></span>|<span data-ttu-id="b5543-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b5543-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5543-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b5543-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5543-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b5543-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5543-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5543-149">This property is read-only.</span></span> <span data-ttu-id="b5543-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5543-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5543-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5543-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5543-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5543-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5543-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5543-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5543-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5543-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5543-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5543-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5543-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5543-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5543-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5543-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5543-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b5543-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5543-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5543-163">createdDateTime</span></span>|<span data-ttu-id="b5543-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5543-164">DateTimeOffset</span></span>|<span data-ttu-id="b5543-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b5543-165">DateTime the object was created.</span></span> <span data-ttu-id="b5543-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-167">description</span><span class="sxs-lookup"><span data-stu-id="b5543-167">description</span></span>|<span data-ttu-id="b5543-168">String</span><span class="sxs-lookup"><span data-stu-id="b5543-168">String</span></span>|<span data-ttu-id="b5543-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5543-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5543-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b5543-171">displayName</span></span>|<span data-ttu-id="b5543-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b5543-172">String</span></span>|<span data-ttu-id="b5543-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5543-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5543-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-175">version</span><span class="sxs-lookup"><span data-stu-id="b5543-175">version</span></span>|<span data-ttu-id="b5543-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b5543-176">Int32</span></span>|<span data-ttu-id="b5543-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b5543-177">Version of the device configuration.</span></span> <span data-ttu-id="b5543-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5543-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="b5543-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="b5543-180">Int32</span><span class="sxs-lookup"><span data-stu-id="b5543-180">Int32</span></span>|<span data-ttu-id="b5543-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="b5543-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b5543-182">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b5543-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b5543-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b5543-183">subjectNameFormat</span></span>|[<span data-ttu-id="b5543-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="b5543-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="b5543-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b5543-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="b5543-186">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b5543-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="b5543-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="b5543-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b5543-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b5543-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b5543-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b5543-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="b5543-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="b5543-191">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b5543-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b5543-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b5543-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b5543-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b5543-194">Int32</span><span class="sxs-lookup"><span data-stu-id="b5543-194">Int32</span></span>|<span data-ttu-id="b5543-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b5543-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="b5543-196">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b5543-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b5543-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b5543-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b5543-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b5543-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b5543-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="b5543-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="b5543-200">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b5543-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="b5543-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b5543-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b5543-202">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="b5543-202">scepServerUrls</span></span>|<span data-ttu-id="b5543-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b5543-203">String collection</span></span>|<span data-ttu-id="b5543-204">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="b5543-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="b5543-205">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="b5543-205">subjectNameFormatString</span></span>|<span data-ttu-id="b5543-206">String</span><span class="sxs-lookup"><span data-stu-id="b5543-206">String</span></span>|<span data-ttu-id="b5543-207">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="b5543-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b5543-208">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="b5543-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b5543-209">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="b5543-209">keyUsage</span></span>|[<span data-ttu-id="b5543-210">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="b5543-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="b5543-211">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="b5543-211">SCEP Key Usage.</span></span> <span data-ttu-id="b5543-212">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b5543-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b5543-213">keySize</span><span class="sxs-lookup"><span data-stu-id="b5543-213">keySize</span></span>|[<span data-ttu-id="b5543-214">keySize</span><span class="sxs-lookup"><span data-stu-id="b5543-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="b5543-215">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="b5543-215">SCEP Key Size.</span></span> <span data-ttu-id="b5543-216">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="b5543-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="b5543-217">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="b5543-217">extendedKeyUsages</span></span>|<span data-ttu-id="b5543-218">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b5543-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b5543-219">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="b5543-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b5543-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b5543-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b5543-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b5543-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b5543-222">String</span><span class="sxs-lookup"><span data-stu-id="b5543-222">String</span></span>|<span data-ttu-id="b5543-223">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="b5543-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b5543-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b5543-224">certificateStore</span></span>|[<span data-ttu-id="b5543-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b5543-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="b5543-226">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="b5543-226">Target store certificate.</span></span> <span data-ttu-id="b5543-227">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="b5543-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="b5543-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="b5543-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="b5543-229">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="b5543-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="b5543-230">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="b5543-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="b5543-231">Переменная OnPremisesUserPrincipalName также поддерживает и другие, описанные здесь: https://go.microsoft.com/fwlink/?LinkId=2027630.</span><span class="sxs-lookup"><span data-stu-id="b5543-231">The OnPremisesUserPrincipalName variable is support as well as others documented here: https://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="b5543-232">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b5543-232">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b5543-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5543-233">Response</span></span>
<span data-ttu-id="b5543-234">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5543-234">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5543-235">Пример</span><span class="sxs-lookup"><span data-stu-id="b5543-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5543-236">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5543-236">Request</span></span>
<span data-ttu-id="b5543-237">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5543-237">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5543-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5543-238">Response</span></span>
<span data-ttu-id="b5543-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5543-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




