---
title: Обновление Макоспкксцертификатепрофиле
description: Обновление свойств объекта Макоспкксцертификатепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fe9272d6722d8d5f73f9c3670c468987646cda8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42745200"
---
# <a name="update-macospkcscertificateprofile"></a><span data-ttu-id="9291e-103">Обновление Макоспкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="9291e-103">Update macOSPkcsCertificateProfile</span></span>

> <span data-ttu-id="9291e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9291e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9291e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9291e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9291e-106">Обновление свойств объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9291e-106">Update the properties of a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9291e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9291e-107">Prerequisites</span></span>
<span data-ttu-id="9291e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9291e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9291e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9291e-110">Permission type</span></span>|<span data-ttu-id="9291e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9291e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9291e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9291e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9291e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9291e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9291e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9291e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9291e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9291e-115">Not supported.</span></span>|
|<span data-ttu-id="9291e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9291e-116">Application</span></span>|<span data-ttu-id="9291e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9291e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9291e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9291e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9291e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9291e-119">Request headers</span></span>
|<span data-ttu-id="9291e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9291e-120">Header</span></span>|<span data-ttu-id="9291e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9291e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9291e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9291e-122">Authorization</span></span>|<span data-ttu-id="9291e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9291e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9291e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9291e-124">Accept</span></span>|<span data-ttu-id="9291e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9291e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9291e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9291e-126">Request body</span></span>
<span data-ttu-id="9291e-127">В тексте запроса добавьте представление объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9291e-127">In the request body, supply a JSON representation for the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="9291e-128">В следующей таблице приведены свойства, необходимые при создании [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-128">The following table shows the properties that are required when you create the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="9291e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9291e-129">Property</span></span>|<span data-ttu-id="9291e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9291e-130">Type</span></span>|<span data-ttu-id="9291e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9291e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9291e-132">id</span><span class="sxs-lookup"><span data-stu-id="9291e-132">id</span></span>|<span data-ttu-id="9291e-133">String</span><span class="sxs-lookup"><span data-stu-id="9291e-133">String</span></span>|<span data-ttu-id="9291e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-134">Key of the entity.</span></span> <span data-ttu-id="9291e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9291e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9291e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9291e-137">DateTimeOffset</span></span>|<span data-ttu-id="9291e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9291e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9291e-140">roleScopeTagIds</span></span>|<span data-ttu-id="9291e-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9291e-141">String collection</span></span>|<span data-ttu-id="9291e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9291e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9291e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9291e-144">supportsScopeTags</span></span>|<span data-ttu-id="9291e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="9291e-145">Boolean</span></span>|<span data-ttu-id="9291e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9291e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9291e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9291e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9291e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9291e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9291e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9291e-149">This property is read-only.</span></span> <span data-ttu-id="9291e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9291e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9291e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9291e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9291e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9291e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9291e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9291e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9291e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9291e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9291e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9291e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9291e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9291e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9291e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9291e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9291e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9291e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9291e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9291e-163">createdDateTime</span></span>|<span data-ttu-id="9291e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9291e-164">DateTimeOffset</span></span>|<span data-ttu-id="9291e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-165">DateTime the object was created.</span></span> <span data-ttu-id="9291e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-167">description</span><span class="sxs-lookup"><span data-stu-id="9291e-167">description</span></span>|<span data-ttu-id="9291e-168">String</span><span class="sxs-lookup"><span data-stu-id="9291e-168">String</span></span>|<span data-ttu-id="9291e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9291e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9291e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9291e-171">displayName</span></span>|<span data-ttu-id="9291e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9291e-172">String</span></span>|<span data-ttu-id="9291e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9291e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9291e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-175">version</span><span class="sxs-lookup"><span data-stu-id="9291e-175">version</span></span>|<span data-ttu-id="9291e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9291e-176">Int32</span></span>|<span data-ttu-id="9291e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9291e-177">Version of the device configuration.</span></span> <span data-ttu-id="9291e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9291e-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="9291e-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="9291e-180">Int32</span><span class="sxs-lookup"><span data-stu-id="9291e-180">Int32</span></span>|<span data-ttu-id="9291e-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="9291e-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="9291e-182">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9291e-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9291e-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="9291e-183">subjectNameFormat</span></span>|[<span data-ttu-id="9291e-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="9291e-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="9291e-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="9291e-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="9291e-186">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="9291e-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="9291e-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="9291e-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9291e-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="9291e-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="9291e-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="9291e-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="9291e-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="9291e-191">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="9291e-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="9291e-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="9291e-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="9291e-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="9291e-194">Int32</span><span class="sxs-lookup"><span data-stu-id="9291e-194">Int32</span></span>|<span data-ttu-id="9291e-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9291e-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="9291e-196">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="9291e-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="9291e-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9291e-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="9291e-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="9291e-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="9291e-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="9291e-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="9291e-200">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="9291e-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="9291e-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="9291e-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="9291e-202">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="9291e-202">certificationAuthority</span></span>|<span data-ttu-id="9291e-203">String</span><span class="sxs-lookup"><span data-stu-id="9291e-203">String</span></span>|<span data-ttu-id="9291e-204">Полное доменное имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="9291e-204">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="9291e-205">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="9291e-205">certificationAuthorityName</span></span>|<span data-ttu-id="9291e-206">String</span><span class="sxs-lookup"><span data-stu-id="9291e-206">String</span></span>|<span data-ttu-id="9291e-207">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="9291e-207">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="9291e-208">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="9291e-208">certificateTemplateName</span></span>|<span data-ttu-id="9291e-209">String</span><span class="sxs-lookup"><span data-stu-id="9291e-209">String</span></span>|<span data-ttu-id="9291e-210">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="9291e-210">PKCS certificate template name.</span></span>|
|<span data-ttu-id="9291e-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="9291e-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="9291e-212">String</span><span class="sxs-lookup"><span data-stu-id="9291e-212">String</span></span>|<span data-ttu-id="9291e-213">Строка формата, определяющая альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-213">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="9291e-214">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="9291e-214">subjectNameFormatString</span></span>|<span data-ttu-id="9291e-215">String</span><span class="sxs-lookup"><span data-stu-id="9291e-215">String</span></span>|<span data-ttu-id="9291e-216">Строка формата, определяющая имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-216">Format string that defines the subject name.</span></span> <span data-ttu-id="9291e-217">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="9291e-217">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="9291e-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9291e-218">certificateStore</span></span>|[<span data-ttu-id="9291e-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="9291e-219">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="9291e-220">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="9291e-220">Target store certificate.</span></span> <span data-ttu-id="9291e-221">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="9291e-221">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="9291e-222">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="9291e-222">customSubjectAlternativeNames</span></span>|<span data-ttu-id="9291e-223">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="9291e-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="9291e-224">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="9291e-224">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="9291e-225">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9291e-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9291e-226">алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="9291e-226">allowAllAppsAccess</span></span>|<span data-ttu-id="9291e-227">Логический</span><span class="sxs-lookup"><span data-stu-id="9291e-227">Boolean</span></span>|<span data-ttu-id="9291e-228">Параметр Алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="9291e-228">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="9291e-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="9291e-229">Response</span></span>
<span data-ttu-id="9291e-230">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9291e-230">If successful, this method returns a `200 OK` response code and an updated [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9291e-231">Пример</span><span class="sxs-lookup"><span data-stu-id="9291e-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="9291e-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="9291e-232">Request</span></span>
<span data-ttu-id="9291e-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9291e-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
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
  ],
  "allowAllAppsAccess": true
}
```

### <a name="response"></a><span data-ttu-id="9291e-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="9291e-234">Response</span></span>
<span data-ttu-id="9291e-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9291e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSPkcsCertificateProfile",
  "id": "4b489237-9237-4b48-3792-484b3792484b",
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
  ],
  "allowAllAppsAccess": true
}
```




