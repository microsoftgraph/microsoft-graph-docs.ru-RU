---
title: Создание Макоспкксцертификатепрофиле
description: Создание нового объекта Макоспкксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d62ff86107ceeab4c6f1de284abc0c3178e2d24e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432503"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="0900b-103">Создание Макоспкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="0900b-103">Create macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="0900b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0900b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0900b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0900b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0900b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0900b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0900b-107">Создание нового объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0900b-107">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0900b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0900b-108">Prerequisites</span></span>
<span data-ttu-id="0900b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0900b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0900b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0900b-111">Permission type</span></span>|<span data-ttu-id="0900b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0900b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0900b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0900b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0900b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0900b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0900b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0900b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0900b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0900b-116">Not supported.</span></span>|
|<span data-ttu-id="0900b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0900b-117">Application</span></span>|<span data-ttu-id="0900b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0900b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0900b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0900b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0900b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0900b-120">Request headers</span></span>
|<span data-ttu-id="0900b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0900b-121">Header</span></span>|<span data-ttu-id="0900b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0900b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0900b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0900b-123">Authorization</span></span>|<span data-ttu-id="0900b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0900b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0900b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0900b-125">Accept</span></span>|<span data-ttu-id="0900b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0900b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0900b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0900b-127">Request body</span></span>
<span data-ttu-id="0900b-128">В тексте запроса добавьте представление объекта Макоспкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0900b-128">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="0900b-129">В следующей таблице приведены свойства, необходимые при создании Макоспкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="0900b-129">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="0900b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0900b-130">Property</span></span>|<span data-ttu-id="0900b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0900b-131">Type</span></span>|<span data-ttu-id="0900b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0900b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0900b-133">id</span><span class="sxs-lookup"><span data-stu-id="0900b-133">id</span></span>|<span data-ttu-id="0900b-134">String</span><span class="sxs-lookup"><span data-stu-id="0900b-134">String</span></span>|<span data-ttu-id="0900b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-135">Key of the entity.</span></span> <span data-ttu-id="0900b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0900b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0900b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0900b-138">DateTimeOffset</span></span>|<span data-ttu-id="0900b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0900b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0900b-141">roleScopeTagIds</span></span>|<span data-ttu-id="0900b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0900b-142">String collection</span></span>|<span data-ttu-id="0900b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0900b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0900b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0900b-145">supportsScopeTags</span></span>|<span data-ttu-id="0900b-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="0900b-146">Boolean</span></span>|<span data-ttu-id="0900b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0900b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0900b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0900b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0900b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0900b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0900b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0900b-150">This property is read-only.</span></span> <span data-ttu-id="0900b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0900b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0900b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0900b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0900b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0900b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0900b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0900b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0900b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0900b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0900b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0900b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0900b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0900b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0900b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0900b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0900b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0900b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0900b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0900b-164">createdDateTime</span></span>|<span data-ttu-id="0900b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0900b-165">DateTimeOffset</span></span>|<span data-ttu-id="0900b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-166">DateTime the object was created.</span></span> <span data-ttu-id="0900b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-168">description</span><span class="sxs-lookup"><span data-stu-id="0900b-168">description</span></span>|<span data-ttu-id="0900b-169">String</span><span class="sxs-lookup"><span data-stu-id="0900b-169">String</span></span>|<span data-ttu-id="0900b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0900b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0900b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0900b-172">displayName</span></span>|<span data-ttu-id="0900b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="0900b-173">String</span></span>|<span data-ttu-id="0900b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0900b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0900b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-176">version</span><span class="sxs-lookup"><span data-stu-id="0900b-176">version</span></span>|<span data-ttu-id="0900b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0900b-177">Int32</span></span>|<span data-ttu-id="0900b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0900b-178">Version of the device configuration.</span></span> <span data-ttu-id="0900b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0900b-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="0900b-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="0900b-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0900b-181">Int32</span></span>|<span data-ttu-id="0900b-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="0900b-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0900b-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0900b-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0900b-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0900b-184">subjectNameFormat</span></span>|[<span data-ttu-id="0900b-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="0900b-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="0900b-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0900b-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="0900b-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0900b-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="0900b-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="0900b-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0900b-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0900b-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0900b-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0900b-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0900b-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0900b-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0900b-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0900b-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0900b-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0900b-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0900b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="0900b-195">Int32</span></span>|<span data-ttu-id="0900b-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0900b-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0900b-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0900b-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0900b-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0900b-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0900b-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0900b-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0900b-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0900b-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0900b-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0900b-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="0900b-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0900b-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0900b-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="0900b-203">certificationAuthority</span></span>|<span data-ttu-id="0900b-204">String</span><span class="sxs-lookup"><span data-stu-id="0900b-204">String</span></span>|<span data-ttu-id="0900b-205">Полное доменное имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="0900b-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="0900b-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="0900b-206">certificationAuthorityName</span></span>|<span data-ttu-id="0900b-207">String</span><span class="sxs-lookup"><span data-stu-id="0900b-207">String</span></span>|<span data-ttu-id="0900b-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="0900b-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="0900b-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="0900b-209">certificateTemplateName</span></span>|<span data-ttu-id="0900b-210">String</span><span class="sxs-lookup"><span data-stu-id="0900b-210">String</span></span>|<span data-ttu-id="0900b-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="0900b-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="0900b-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="0900b-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="0900b-213">String</span><span class="sxs-lookup"><span data-stu-id="0900b-213">String</span></span>|<span data-ttu-id="0900b-214">Строка формата, определяющая альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="0900b-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="0900b-215">subjectNameFormatString</span></span>|<span data-ttu-id="0900b-216">String</span><span class="sxs-lookup"><span data-stu-id="0900b-216">String</span></span>|<span data-ttu-id="0900b-217">Строка формата, определяющая имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-217">Format string that defines the subject name.</span></span> <span data-ttu-id="0900b-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="0900b-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="0900b-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0900b-219">certificateStore</span></span>|[<span data-ttu-id="0900b-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="0900b-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="0900b-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="0900b-221">Target store certificate.</span></span> <span data-ttu-id="0900b-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="0900b-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="0900b-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="0900b-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="0900b-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="0900b-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="0900b-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="0900b-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="0900b-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0900b-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0900b-227">алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="0900b-227">allowAllAppsAccess</span></span>|<span data-ttu-id="0900b-228">Логическое</span><span class="sxs-lookup"><span data-stu-id="0900b-228">Boolean</span></span>|<span data-ttu-id="0900b-229">Параметр Алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="0900b-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="0900b-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="0900b-230">Response</span></span>
<span data-ttu-id="0900b-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0900b-231">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0900b-232">Пример</span><span class="sxs-lookup"><span data-stu-id="0900b-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="0900b-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="0900b-233">Request</span></span>
<span data-ttu-id="0900b-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0900b-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0900b-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="0900b-235">Response</span></span>
<span data-ttu-id="0900b-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0900b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



