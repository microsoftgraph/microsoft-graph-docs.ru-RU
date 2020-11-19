---
title: Создание Макоспкксцертификатепрофиле
description: Создание нового объекта Макоспкксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8d88684dbcd073b761ed588ff23fb5e86f8098a3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230494"
---
# <a name="create-macospkcscertificateprofile"></a><span data-ttu-id="47961-103">Создание Макоспкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="47961-103">Create macOSPkcsCertificateProfile</span></span>

<span data-ttu-id="47961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47961-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47961-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47961-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47961-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47961-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47961-107">Создание нового объекта [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="47961-107">Create a new [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47961-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="47961-108">Prerequisites</span></span>
<span data-ttu-id="47961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47961-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47961-111">Permission type</span></span>|<span data-ttu-id="47961-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47961-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47961-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47961-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47961-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47961-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47961-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47961-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47961-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47961-116">Not supported.</span></span>|
|<span data-ttu-id="47961-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47961-117">Application</span></span>|<span data-ttu-id="47961-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47961-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47961-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47961-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47961-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="47961-120">Request headers</span></span>
|<span data-ttu-id="47961-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47961-121">Header</span></span>|<span data-ttu-id="47961-122">Значение</span><span class="sxs-lookup"><span data-stu-id="47961-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47961-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47961-123">Authorization</span></span>|<span data-ttu-id="47961-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47961-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47961-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47961-125">Accept</span></span>|<span data-ttu-id="47961-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47961-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47961-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47961-127">Request body</span></span>
<span data-ttu-id="47961-128">В тексте запроса добавьте представление объекта Макоспкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47961-128">In the request body, supply a JSON representation for the macOSPkcsCertificateProfile object.</span></span>

<span data-ttu-id="47961-129">В следующей таблице приведены свойства, необходимые при создании Макоспкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="47961-129">The following table shows the properties that are required when you create the macOSPkcsCertificateProfile.</span></span>

|<span data-ttu-id="47961-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="47961-130">Property</span></span>|<span data-ttu-id="47961-131">Тип</span><span class="sxs-lookup"><span data-stu-id="47961-131">Type</span></span>|<span data-ttu-id="47961-132">Описание</span><span class="sxs-lookup"><span data-stu-id="47961-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47961-133">id</span><span class="sxs-lookup"><span data-stu-id="47961-133">id</span></span>|<span data-ttu-id="47961-134">String</span><span class="sxs-lookup"><span data-stu-id="47961-134">String</span></span>|<span data-ttu-id="47961-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="47961-135">Key of the entity.</span></span> <span data-ttu-id="47961-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47961-137">lastModifiedDateTime</span></span>|<span data-ttu-id="47961-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47961-138">DateTimeOffset</span></span>|<span data-ttu-id="47961-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="47961-139">DateTime the object was last modified.</span></span> <span data-ttu-id="47961-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47961-141">roleScopeTagIds</span></span>|<span data-ttu-id="47961-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="47961-142">String collection</span></span>|<span data-ttu-id="47961-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="47961-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47961-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="47961-145">supportsScopeTags</span></span>|<span data-ttu-id="47961-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="47961-146">Boolean</span></span>|<span data-ttu-id="47961-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="47961-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47961-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="47961-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47961-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="47961-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47961-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47961-150">This property is read-only.</span></span> <span data-ttu-id="47961-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47961-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47961-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47961-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47961-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47961-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47961-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47961-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47961-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47961-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47961-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47961-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47961-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47961-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47961-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47961-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47961-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="47961-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47961-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47961-164">createdDateTime</span></span>|<span data-ttu-id="47961-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47961-165">DateTimeOffset</span></span>|<span data-ttu-id="47961-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="47961-166">DateTime the object was created.</span></span> <span data-ttu-id="47961-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-168">description</span><span class="sxs-lookup"><span data-stu-id="47961-168">description</span></span>|<span data-ttu-id="47961-169">String</span><span class="sxs-lookup"><span data-stu-id="47961-169">String</span></span>|<span data-ttu-id="47961-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47961-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47961-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-172">displayName</span><span class="sxs-lookup"><span data-stu-id="47961-172">displayName</span></span>|<span data-ttu-id="47961-173">String</span><span class="sxs-lookup"><span data-stu-id="47961-173">String</span></span>|<span data-ttu-id="47961-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47961-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47961-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-176">version</span><span class="sxs-lookup"><span data-stu-id="47961-176">version</span></span>|<span data-ttu-id="47961-177">Int32</span><span class="sxs-lookup"><span data-stu-id="47961-177">Int32</span></span>|<span data-ttu-id="47961-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="47961-178">Version of the device configuration.</span></span> <span data-ttu-id="47961-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47961-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47961-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="47961-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="47961-181">Int32</span><span class="sxs-lookup"><span data-stu-id="47961-181">Int32</span></span>|<span data-ttu-id="47961-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="47961-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="47961-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="47961-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="47961-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="47961-184">subjectNameFormat</span></span>|[<span data-ttu-id="47961-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="47961-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="47961-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="47961-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="47961-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="47961-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="47961-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="47961-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="47961-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="47961-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="47961-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="47961-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="47961-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="47961-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="47961-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="47961-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="47961-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="47961-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="47961-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="47961-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="47961-195">Int32</span><span class="sxs-lookup"><span data-stu-id="47961-195">Int32</span></span>|<span data-ttu-id="47961-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="47961-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="47961-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="47961-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="47961-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="47961-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="47961-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="47961-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="47961-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="47961-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="47961-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="47961-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="47961-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="47961-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="47961-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="47961-203">certificationAuthority</span></span>|<span data-ttu-id="47961-204">String</span><span class="sxs-lookup"><span data-stu-id="47961-204">String</span></span>|<span data-ttu-id="47961-205">Полное доменное имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="47961-205">PKCS certification authority FQDN.</span></span>|
|<span data-ttu-id="47961-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="47961-206">certificationAuthorityName</span></span>|<span data-ttu-id="47961-207">String</span><span class="sxs-lookup"><span data-stu-id="47961-207">String</span></span>|<span data-ttu-id="47961-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="47961-208">PKCS certification authority Name.</span></span>|
|<span data-ttu-id="47961-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="47961-209">certificateTemplateName</span></span>|<span data-ttu-id="47961-210">String</span><span class="sxs-lookup"><span data-stu-id="47961-210">String</span></span>|<span data-ttu-id="47961-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="47961-211">PKCS certificate template name.</span></span>|
|<span data-ttu-id="47961-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="47961-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="47961-213">String</span><span class="sxs-lookup"><span data-stu-id="47961-213">String</span></span>|<span data-ttu-id="47961-214">Строка формата, определяющая альтернативное имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="47961-214">Format string that defines the subject alternative name.</span></span>|
|<span data-ttu-id="47961-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="47961-215">subjectNameFormatString</span></span>|<span data-ttu-id="47961-216">String</span><span class="sxs-lookup"><span data-stu-id="47961-216">String</span></span>|<span data-ttu-id="47961-217">Строка формата, определяющая имя субъекта.</span><span class="sxs-lookup"><span data-stu-id="47961-217">Format string that defines the subject name.</span></span> <span data-ttu-id="47961-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="47961-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="47961-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="47961-219">certificateStore</span></span>|[<span data-ttu-id="47961-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="47961-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="47961-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="47961-221">Target store certificate.</span></span> <span data-ttu-id="47961-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="47961-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="47961-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="47961-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="47961-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="47961-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="47961-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="47961-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="47961-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="47961-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="47961-227">алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="47961-227">allowAllAppsAccess</span></span>|<span data-ttu-id="47961-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="47961-228">Boolean</span></span>|<span data-ttu-id="47961-229">Параметр Алловаллаппсакцесс</span><span class="sxs-lookup"><span data-stu-id="47961-229">AllowAllAppsAccess setting</span></span>|



## <a name="response"></a><span data-ttu-id="47961-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="47961-230">Response</span></span>
<span data-ttu-id="47961-231">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоспкксцертификатепрофиле](../resources/intune-deviceconfig-macospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47961-231">If successful, this method returns a `201 Created` response code and a [macOSPkcsCertificateProfile](../resources/intune-deviceconfig-macospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47961-232">Пример</span><span class="sxs-lookup"><span data-stu-id="47961-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="47961-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="47961-233">Request</span></span>
<span data-ttu-id="47961-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47961-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47961-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="47961-235">Response</span></span>
<span data-ttu-id="47961-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47961-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




