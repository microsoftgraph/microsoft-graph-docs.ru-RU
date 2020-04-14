---
title: Обновление Макоспкксцертификатепрофиле
description: Обновление свойств объекта Макоспкксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a16d66d1e87cfee4d1847392427e068cea76db8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432470"
---
# <a name="update-macospkcscertificateprofile"></a><span data-ttu-id="537ca-103">Обновление Макоспкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="537ca-103">Update macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="537ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="537ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="537ca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="537ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="537ca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="537ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="537ca-107">Обновление свойств объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="537ca-107">Update the properties of a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="537ca-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="537ca-108">Prerequisites</span></span>
<span data-ttu-id="537ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="537ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="537ca-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="537ca-111">Permission type</span></span>|<span data-ttu-id="537ca-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="537ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="537ca-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="537ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="537ca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537ca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="537ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="537ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="537ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="537ca-116">Not supported.</span></span>|
|<span data-ttu-id="537ca-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="537ca-117">Application</span></span>|<span data-ttu-id="537ca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="537ca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="537ca-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="537ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="537ca-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="537ca-120">Request headers</span></span>
|<span data-ttu-id="537ca-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="537ca-121">Header</span></span>|<span data-ttu-id="537ca-122">Значение</span><span class="sxs-lookup"><span data-stu-id="537ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="537ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="537ca-123">Authorization</span></span>|<span data-ttu-id="537ca-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="537ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="537ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="537ca-125">Accept</span></span>|<span data-ttu-id="537ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="537ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="537ca-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="537ca-127">Request body</span></span>
<span data-ttu-id="537ca-128">В тексте запроса добавьте представление объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="537ca-128">In the request body, supply a JSON representation for the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="537ca-129">В следующей таблице приведены свойства, необходимые при создании [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-129">The following table shows the properties that are required when you create the [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="537ca-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="537ca-130">Property</span></span>|<span data-ttu-id="537ca-131">Тип</span><span class="sxs-lookup"><span data-stu-id="537ca-131">Type</span></span>|<span data-ttu-id="537ca-132">Описание</span><span class="sxs-lookup"><span data-stu-id="537ca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="537ca-133">id</span><span class="sxs-lookup"><span data-stu-id="537ca-133">id</span></span>|<span data-ttu-id="537ca-134">String</span><span class="sxs-lookup"><span data-stu-id="537ca-134">String</span></span>|<span data-ttu-id="537ca-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-135">Key of the entity.</span></span> <span data-ttu-id="537ca-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="537ca-137">lastModifiedDateTime</span></span>|<span data-ttu-id="537ca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537ca-138">DateTimeOffset</span></span>|<span data-ttu-id="537ca-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-139">DateTime the object was last modified.</span></span> <span data-ttu-id="537ca-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="537ca-141">roleScopeTagIds</span></span>|<span data-ttu-id="537ca-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="537ca-142">String collection</span></span>|<span data-ttu-id="537ca-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="537ca-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="537ca-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="537ca-145">supportsScopeTags</span></span>|<span data-ttu-id="537ca-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="537ca-146">Boolean</span></span>|<span data-ttu-id="537ca-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="537ca-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="537ca-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="537ca-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="537ca-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="537ca-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="537ca-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="537ca-150">This property is read-only.</span></span> <span data-ttu-id="537ca-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="537ca-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="537ca-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="537ca-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="537ca-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="537ca-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="537ca-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="537ca-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="537ca-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="537ca-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="537ca-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="537ca-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="537ca-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="537ca-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="537ca-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="537ca-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="537ca-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="537ca-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="537ca-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="537ca-164">createdDateTime</span></span>|<span data-ttu-id="537ca-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="537ca-165">DateTimeOffset</span></span>|<span data-ttu-id="537ca-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-166">DateTime the object was created.</span></span> <span data-ttu-id="537ca-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-168">description</span><span class="sxs-lookup"><span data-stu-id="537ca-168">description</span></span>|<span data-ttu-id="537ca-169">String</span><span class="sxs-lookup"><span data-stu-id="537ca-169">String</span></span>|<span data-ttu-id="537ca-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="537ca-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="537ca-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-172">displayName</span><span class="sxs-lookup"><span data-stu-id="537ca-172">displayName</span></span>|<span data-ttu-id="537ca-173">Строка</span><span class="sxs-lookup"><span data-stu-id="537ca-173">String</span></span>|<span data-ttu-id="537ca-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="537ca-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="537ca-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-176">version</span><span class="sxs-lookup"><span data-stu-id="537ca-176">version</span></span>|<span data-ttu-id="537ca-177">Int32</span><span class="sxs-lookup"><span data-stu-id="537ca-177">Int32</span></span>|<span data-ttu-id="537ca-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="537ca-178">Version of the device configuration.</span></span> <span data-ttu-id="537ca-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="537ca-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="537ca-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="537ca-181">Int32</span><span class="sxs-lookup"><span data-stu-id="537ca-181">Int32</span></span>|<span data-ttu-id="537ca-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="537ca-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="537ca-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="537ca-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="537ca-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="537ca-184">subjectNameFormat</span></span>|[<span data-ttu-id="537ca-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="537ca-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="537ca-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="537ca-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="537ca-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="537ca-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="537ca-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="537ca-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="537ca-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="537ca-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="537ca-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="537ca-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="537ca-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="537ca-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="537ca-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="537ca-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="537ca-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="537ca-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="537ca-195">Int32</span><span class="sxs-lookup"><span data-stu-id="537ca-195">Int32</span></span>|<span data-ttu-id="537ca-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="537ca-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="537ca-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="537ca-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="537ca-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="537ca-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="537ca-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="537ca-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="537ca-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="537ca-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="537ca-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="537ca-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="537ca-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="537ca-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="537ca-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="537ca-203">certificationAuthority</span></span>|<span data-ttu-id="537ca-204">String</span><span class="sxs-lookup"><span data-stu-id="537ca-204">String</span></span>|<span data-ttu-id="537ca-205">Полное доменное имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="537ca-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="537ca-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="537ca-206">certificationAuthorityName</span></span>|<span data-ttu-id="537ca-207">String</span><span class="sxs-lookup"><span data-stu-id="537ca-207">String</span></span>|<span data-ttu-id="537ca-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="537ca-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="537ca-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="537ca-209">certificateTemplateName</span></span>|<span data-ttu-id="537ca-210">String</span><span class="sxs-lookup"><span data-stu-id="537ca-210">String</span></span>|<span data-ttu-id="537ca-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="537ca-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="537ca-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="537ca-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="537ca-213">String</span><span class="sxs-lookup"><span data-stu-id="537ca-213">String</span></span>|<span data-ttu-id="537ca-214">Строка формата, определяющая альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="537ca-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="537ca-215">subjectNameFormatString</span></span>|<span data-ttu-id="537ca-216">String</span><span class="sxs-lookup"><span data-stu-id="537ca-216">String</span></span>|<span data-ttu-id="537ca-217">Строка формата, определяющая имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-217">Format string that defines the subject name.</span></span> <span data-ttu-id="537ca-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="537ca-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="537ca-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="537ca-219">certificateStore</span></span>|[<span data-ttu-id="537ca-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="537ca-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="537ca-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="537ca-221">Target store certificate.</span></span> <span data-ttu-id="537ca-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="537ca-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="537ca-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="537ca-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="537ca-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="537ca-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="537ca-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="537ca-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="537ca-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="537ca-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="537ca-227">алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="537ca-227">allowAllAppsAccess</span></span>|<span data-ttu-id="537ca-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="537ca-228">Boolean</span></span>|<span data-ttu-id="537ca-229">Параметр Алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="537ca-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="537ca-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="537ca-230">Response</span></span>
<span data-ttu-id="537ca-231">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="537ca-231">If successful, this method returns a `200 OK` response code and an updated [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="537ca-232">Пример</span><span class="sxs-lookup"><span data-stu-id="537ca-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="537ca-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="537ca-233">Request</span></span>
<span data-ttu-id="537ca-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="537ca-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="537ca-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="537ca-235">Response</span></span>
<span data-ttu-id="537ca-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="537ca-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



