---
title: Обновление Макоспкксцертификатепрофиле
description: Обновление свойств объекта Макоспкксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 784b46d8778642b9e1d6ddeb03f010dba2f04bf1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948186"
---
# <a name="update-macospkcscertificateprofile"></a><span data-ttu-id="4694d-103">Обновление Макоспкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="4694d-103">Update macOSPkcsCertificateProfile</span></span>

> <span data-ttu-id="4694d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4694d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4694d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4694d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4694d-106">Обновление свойств объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4694d-106">Update the properties of a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4694d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4694d-107">Prerequisites</span></span>
<span data-ttu-id="4694d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4694d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4694d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4694d-110">Permission type</span></span>|<span data-ttu-id="4694d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4694d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4694d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4694d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4694d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4694d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4694d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4694d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4694d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4694d-115">Not supported.</span></span>|
|<span data-ttu-id="4694d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4694d-116">Application</span></span>|<span data-ttu-id="4694d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4694d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4694d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4694d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4694d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4694d-119">Request headers</span></span>
|<span data-ttu-id="4694d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4694d-120">Header</span></span>|<span data-ttu-id="4694d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4694d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4694d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4694d-122">Authorization</span></span>|<span data-ttu-id="4694d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4694d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4694d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4694d-124">Accept</span></span>|<span data-ttu-id="4694d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4694d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4694d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4694d-126">Request body</span></span>
<span data-ttu-id="4694d-127">В тексте запроса добавьте представление объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4694d-127">In the request body, supply a JSON representation for the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="4694d-128">В следующей таблице приведены свойства, необходимые при создании [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-128">The following table shows the properties that are required when you create the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="4694d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4694d-129">Property</span></span>|<span data-ttu-id="4694d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4694d-130">Type</span></span>|<span data-ttu-id="4694d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4694d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4694d-132">id</span><span class="sxs-lookup"><span data-stu-id="4694d-132">id</span></span>|<span data-ttu-id="4694d-133">String</span><span class="sxs-lookup"><span data-stu-id="4694d-133">String</span></span>|<span data-ttu-id="4694d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-134">Key of the entity.</span></span> <span data-ttu-id="4694d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4694d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4694d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4694d-137">DateTimeOffset</span></span>|<span data-ttu-id="4694d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4694d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4694d-140">roleScopeTagIds</span></span>|<span data-ttu-id="4694d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4694d-141">String collection</span></span>|<span data-ttu-id="4694d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4694d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4694d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4694d-144">supportsScopeTags</span></span>|<span data-ttu-id="4694d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4694d-145">Boolean</span></span>|<span data-ttu-id="4694d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4694d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4694d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4694d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4694d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4694d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4694d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4694d-149">This property is read-only.</span></span> <span data-ttu-id="4694d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4694d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4694d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4694d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4694d-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4694d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4694d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4694d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4694d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4694d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4694d-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4694d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4694d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4694d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4694d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4694d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4694d-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4694d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4694d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4694d-163">createdDateTime</span></span>|<span data-ttu-id="4694d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4694d-164">DateTimeOffset</span></span>|<span data-ttu-id="4694d-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-165">DateTime the object was created.</span></span> <span data-ttu-id="4694d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-167">description</span><span class="sxs-lookup"><span data-stu-id="4694d-167">description</span></span>|<span data-ttu-id="4694d-168">String</span><span class="sxs-lookup"><span data-stu-id="4694d-168">String</span></span>|<span data-ttu-id="4694d-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4694d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4694d-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4694d-171">displayName</span></span>|<span data-ttu-id="4694d-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-172">String</span></span>|<span data-ttu-id="4694d-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4694d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4694d-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-175">version</span><span class="sxs-lookup"><span data-stu-id="4694d-175">version</span></span>|<span data-ttu-id="4694d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4694d-176">Int32</span></span>|<span data-ttu-id="4694d-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4694d-177">Version of the device configuration.</span></span> <span data-ttu-id="4694d-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4694d-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="4694d-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="4694d-180">Int32</span><span class="sxs-lookup"><span data-stu-id="4694d-180">Int32</span></span>|<span data-ttu-id="4694d-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="4694d-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4694d-182">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4694d-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4694d-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4694d-183">subjectNameFormat</span></span>|[<span data-ttu-id="4694d-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="4694d-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="4694d-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="4694d-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="4694d-186">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4694d-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="4694d-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="4694d-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4694d-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4694d-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4694d-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="4694d-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="4694d-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="4694d-191">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4694d-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="4694d-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="4694d-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4694d-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4694d-194">Int32</span><span class="sxs-lookup"><span data-stu-id="4694d-194">Int32</span></span>|<span data-ttu-id="4694d-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="4694d-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4694d-196">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4694d-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4694d-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4694d-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4694d-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4694d-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="4694d-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="4694d-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4694d-200">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4694d-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="4694d-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="4694d-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4694d-202">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="4694d-202">certificationAuthority</span></span>|<span data-ttu-id="4694d-203">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-203">String</span></span>|<span data-ttu-id="4694d-204">Полное доменное имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="4694d-204">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="4694d-205">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="4694d-205">certificationAuthorityName</span></span>|<span data-ttu-id="4694d-206">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-206">String</span></span>|<span data-ttu-id="4694d-207">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="4694d-207">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="4694d-208">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="4694d-208">certificateTemplateName</span></span>|<span data-ttu-id="4694d-209">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-209">String</span></span>|<span data-ttu-id="4694d-210">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="4694d-210">PKCS certificate template name.</span></span>|
|<span data-ttu-id="4694d-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4694d-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4694d-212">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-212">String</span></span>|<span data-ttu-id="4694d-213">Строка формата, определяющая альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-213">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="4694d-214">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="4694d-214">subjectNameFormatString</span></span>|<span data-ttu-id="4694d-215">Строка</span><span class="sxs-lookup"><span data-stu-id="4694d-215">String</span></span>|<span data-ttu-id="4694d-216">Строка формата, определяющая имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-216">Format string that defines the subject name.</span></span> <span data-ttu-id="4694d-217">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="4694d-217">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="4694d-218">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4694d-218">certificateStore</span></span>|[<span data-ttu-id="4694d-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4694d-219">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="4694d-220">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="4694d-220">Target store certificate.</span></span> <span data-ttu-id="4694d-221">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="4694d-221">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="4694d-222">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="4694d-222">customSubjectAlternativeNames</span></span>|<span data-ttu-id="4694d-223">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="4694d-223">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="4694d-224">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="4694d-224">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="4694d-225">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4694d-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4694d-226">алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="4694d-226">allowAllAppsAccess</span></span>|<span data-ttu-id="4694d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="4694d-227">Boolean</span></span>|<span data-ttu-id="4694d-228">Параметр Алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="4694d-228">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="4694d-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="4694d-229">Response</span></span>
<span data-ttu-id="4694d-230">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4694d-230">If successful, this method returns a `200 OK` response code and an updated [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4694d-231">Пример</span><span class="sxs-lookup"><span data-stu-id="4694d-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="4694d-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="4694d-232">Request</span></span>
<span data-ttu-id="4694d-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4694d-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4694d-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="4694d-234">Response</span></span>
<span data-ttu-id="4694d-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4694d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





