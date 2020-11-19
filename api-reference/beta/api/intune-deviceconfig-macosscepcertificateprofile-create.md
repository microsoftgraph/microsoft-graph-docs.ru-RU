---
title: Создание macOSScepCertificateProfile
description: Создание нового объекта macOSScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f0b4aba9f5cde78285d10aa91a07cbe917ec9e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49236948"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="86482-103">Создание macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="86482-103">Create macOSScepCertificateProfile</span></span>

<span data-ttu-id="86482-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86482-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86482-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86482-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86482-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86482-107">Создание нового объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="86482-107">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86482-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86482-108">Prerequisites</span></span>
<span data-ttu-id="86482-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86482-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86482-111">Permission type</span></span>|<span data-ttu-id="86482-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86482-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86482-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86482-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86482-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86482-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86482-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86482-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86482-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86482-116">Not supported.</span></span>|
|<span data-ttu-id="86482-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="86482-117">Application</span></span>|<span data-ttu-id="86482-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86482-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86482-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86482-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86482-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86482-120">Request headers</span></span>
|<span data-ttu-id="86482-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86482-121">Header</span></span>|<span data-ttu-id="86482-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86482-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86482-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86482-123">Authorization</span></span>|<span data-ttu-id="86482-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86482-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86482-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86482-125">Accept</span></span>|<span data-ttu-id="86482-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86482-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86482-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86482-127">Request body</span></span>
<span data-ttu-id="86482-128">В тексте запроса добавьте представление объекта macOSScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86482-128">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="86482-129">В следующей таблице приведены свойства, необходимые при создании macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="86482-129">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="86482-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="86482-130">Property</span></span>|<span data-ttu-id="86482-131">Тип</span><span class="sxs-lookup"><span data-stu-id="86482-131">Type</span></span>|<span data-ttu-id="86482-132">Описание</span><span class="sxs-lookup"><span data-stu-id="86482-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86482-133">id</span><span class="sxs-lookup"><span data-stu-id="86482-133">id</span></span>|<span data-ttu-id="86482-134">String</span><span class="sxs-lookup"><span data-stu-id="86482-134">String</span></span>|<span data-ttu-id="86482-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86482-135">Key of the entity.</span></span> <span data-ttu-id="86482-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86482-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86482-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86482-138">DateTimeOffset</span></span>|<span data-ttu-id="86482-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="86482-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86482-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86482-141">roleScopeTagIds</span></span>|<span data-ttu-id="86482-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86482-142">String collection</span></span>|<span data-ttu-id="86482-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="86482-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86482-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="86482-145">supportsScopeTags</span></span>|<span data-ttu-id="86482-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="86482-146">Boolean</span></span>|<span data-ttu-id="86482-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="86482-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86482-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="86482-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86482-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="86482-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86482-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86482-150">This property is read-only.</span></span> <span data-ttu-id="86482-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86482-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86482-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86482-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86482-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86482-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86482-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86482-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86482-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86482-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86482-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86482-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86482-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86482-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86482-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86482-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86482-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86482-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86482-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86482-164">createdDateTime</span></span>|<span data-ttu-id="86482-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86482-165">DateTimeOffset</span></span>|<span data-ttu-id="86482-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="86482-166">DateTime the object was created.</span></span> <span data-ttu-id="86482-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-168">description</span><span class="sxs-lookup"><span data-stu-id="86482-168">description</span></span>|<span data-ttu-id="86482-169">String</span><span class="sxs-lookup"><span data-stu-id="86482-169">String</span></span>|<span data-ttu-id="86482-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86482-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86482-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-172">displayName</span><span class="sxs-lookup"><span data-stu-id="86482-172">displayName</span></span>|<span data-ttu-id="86482-173">String</span><span class="sxs-lookup"><span data-stu-id="86482-173">String</span></span>|<span data-ttu-id="86482-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86482-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86482-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-176">version</span><span class="sxs-lookup"><span data-stu-id="86482-176">version</span></span>|<span data-ttu-id="86482-177">Int32</span><span class="sxs-lookup"><span data-stu-id="86482-177">Int32</span></span>|<span data-ttu-id="86482-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86482-178">Version of the device configuration.</span></span> <span data-ttu-id="86482-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86482-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86482-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="86482-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="86482-181">Int32</span><span class="sxs-lookup"><span data-stu-id="86482-181">Int32</span></span>|<span data-ttu-id="86482-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="86482-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="86482-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86482-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86482-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86482-184">subjectNameFormat</span></span>|[<span data-ttu-id="86482-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="86482-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="86482-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="86482-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="86482-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86482-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="86482-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="86482-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="86482-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86482-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="86482-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86482-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="86482-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="86482-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="86482-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86482-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="86482-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="86482-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="86482-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="86482-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="86482-195">Int32</span><span class="sxs-lookup"><span data-stu-id="86482-195">Int32</span></span>|<span data-ttu-id="86482-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="86482-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="86482-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86482-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86482-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86482-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="86482-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86482-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="86482-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="86482-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="86482-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86482-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="86482-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="86482-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="86482-203">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="86482-203">scepServerUrls</span></span>|<span data-ttu-id="86482-204">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86482-204">String collection</span></span>|<span data-ttu-id="86482-205">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="86482-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="86482-206">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="86482-206">subjectNameFormatString</span></span>|<span data-ttu-id="86482-207">String</span><span class="sxs-lookup"><span data-stu-id="86482-207">String</span></span>|<span data-ttu-id="86482-208">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="86482-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="86482-209">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="86482-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="86482-210">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="86482-210">keyUsage</span></span>|[<span data-ttu-id="86482-211">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="86482-211">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="86482-212">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="86482-212">SCEP Key Usage.</span></span> <span data-ttu-id="86482-213">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="86482-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="86482-214">keySize</span><span class="sxs-lookup"><span data-stu-id="86482-214">keySize</span></span>|[<span data-ttu-id="86482-215">keySize</span><span class="sxs-lookup"><span data-stu-id="86482-215">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="86482-216">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="86482-216">SCEP Key Size.</span></span> <span data-ttu-id="86482-217">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="86482-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="86482-218">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="86482-218">hashAlgorithm</span></span>|[<span data-ttu-id="86482-219">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="86482-219">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="86482-220">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="86482-220">SCEP Hash Algorithm.</span></span> <span data-ttu-id="86482-221">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="86482-221">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="86482-222">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="86482-222">extendedKeyUsages</span></span>|<span data-ttu-id="86482-223">Коллекция [екстендедкэйусаже](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="86482-223">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="86482-224">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="86482-224">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="86482-225">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="86482-225">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="86482-226">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="86482-226">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="86482-227">String</span><span class="sxs-lookup"><span data-stu-id="86482-227">String</span></span>|<span data-ttu-id="86482-228">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="86482-228">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="86482-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="86482-229">certificateStore</span></span>|[<span data-ttu-id="86482-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="86482-230">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="86482-231">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="86482-231">Target store certificate.</span></span> <span data-ttu-id="86482-232">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="86482-232">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="86482-233">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="86482-233">customSubjectAlternativeNames</span></span>|<span data-ttu-id="86482-234">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="86482-234">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="86482-235">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="86482-235">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="86482-236">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="86482-236">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="86482-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="86482-237">Response</span></span>
<span data-ttu-id="86482-238">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86482-238">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86482-239">Пример</span><span class="sxs-lookup"><span data-stu-id="86482-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="86482-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="86482-240">Request</span></span>
<span data-ttu-id="86482-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86482-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="86482-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="86482-242">Response</span></span>
<span data-ttu-id="86482-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86482-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
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




