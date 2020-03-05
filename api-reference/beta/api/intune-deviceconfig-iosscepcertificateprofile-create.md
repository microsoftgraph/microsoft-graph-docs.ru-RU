---
title: Создание iosScepCertificateProfile
description: Создание нового объекта iosScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 410bfe67354b6789e984526682f603fa452fe8d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442714"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="ab774-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ab774-103">Create iosScepCertificateProfile</span></span>

<span data-ttu-id="ab774-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab774-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab774-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab774-107">Создание нового объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ab774-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab774-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab774-108">Prerequisites</span></span>
<span data-ttu-id="ab774-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab774-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab774-111">Permission type</span></span>|<span data-ttu-id="ab774-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab774-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab774-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab774-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab774-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab774-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab774-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab774-116">Not supported.</span></span>|
|<span data-ttu-id="ab774-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab774-117">Application</span></span>|<span data-ttu-id="ab774-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab774-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab774-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab774-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab774-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab774-120">Request headers</span></span>
|<span data-ttu-id="ab774-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab774-121">Header</span></span>|<span data-ttu-id="ab774-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab774-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab774-123">Authorization</span></span>|<span data-ttu-id="ab774-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab774-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab774-125">Accept</span></span>|<span data-ttu-id="ab774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab774-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab774-127">Request body</span></span>
<span data-ttu-id="ab774-128">В тексте запроса добавьте представление объекта iosScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab774-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="ab774-129">В следующей таблице приведены свойства, необходимые при создании iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ab774-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="ab774-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab774-130">Property</span></span>|<span data-ttu-id="ab774-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab774-131">Type</span></span>|<span data-ttu-id="ab774-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab774-133">id</span><span class="sxs-lookup"><span data-stu-id="ab774-133">id</span></span>|<span data-ttu-id="ab774-134">String</span><span class="sxs-lookup"><span data-stu-id="ab774-134">String</span></span>|<span data-ttu-id="ab774-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab774-135">Key of the entity.</span></span> <span data-ttu-id="ab774-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab774-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab774-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab774-138">DateTimeOffset</span></span>|<span data-ttu-id="ab774-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab774-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab774-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab774-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab774-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab774-142">String collection</span></span>|<span data-ttu-id="ab774-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ab774-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab774-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ab774-145">supportsScopeTags</span></span>|<span data-ttu-id="ab774-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ab774-146">Boolean</span></span>|<span data-ttu-id="ab774-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ab774-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab774-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ab774-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab774-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ab774-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab774-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab774-150">This property is read-only.</span></span> <span data-ttu-id="ab774-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab774-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ab774-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab774-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ab774-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab774-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ab774-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab774-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ab774-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab774-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ab774-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab774-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ab774-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab774-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ab774-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab774-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ab774-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab774-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ab774-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab774-164">createdDateTime</span></span>|<span data-ttu-id="ab774-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab774-165">DateTimeOffset</span></span>|<span data-ttu-id="ab774-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ab774-166">DateTime the object was created.</span></span> <span data-ttu-id="ab774-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-168">description</span><span class="sxs-lookup"><span data-stu-id="ab774-168">description</span></span>|<span data-ttu-id="ab774-169">String</span><span class="sxs-lookup"><span data-stu-id="ab774-169">String</span></span>|<span data-ttu-id="ab774-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab774-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab774-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ab774-172">displayName</span></span>|<span data-ttu-id="ab774-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ab774-173">String</span></span>|<span data-ttu-id="ab774-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab774-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab774-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-176">version</span><span class="sxs-lookup"><span data-stu-id="ab774-176">version</span></span>|<span data-ttu-id="ab774-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ab774-177">Int32</span></span>|<span data-ttu-id="ab774-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab774-178">Version of the device configuration.</span></span> <span data-ttu-id="ab774-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab774-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="ab774-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="ab774-181">Int32</span><span class="sxs-lookup"><span data-stu-id="ab774-181">Int32</span></span>|<span data-ttu-id="ab774-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab774-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ab774-183">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ab774-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ab774-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ab774-184">subjectNameFormat</span></span>|[<span data-ttu-id="ab774-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="ab774-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="ab774-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab774-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="ab774-187">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ab774-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="ab774-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="ab774-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ab774-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ab774-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ab774-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ab774-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab774-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="ab774-192">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ab774-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ab774-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ab774-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ab774-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ab774-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ab774-195">Int32</span></span>|<span data-ttu-id="ab774-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab774-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="ab774-197">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ab774-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ab774-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ab774-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ab774-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ab774-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ab774-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ab774-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ab774-201">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ab774-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="ab774-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ab774-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ab774-203">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="ab774-203">scepServerUrls</span></span>|<span data-ttu-id="ab774-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab774-204">String collection</span></span>|<span data-ttu-id="ab774-205">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="ab774-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ab774-206">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="ab774-206">subjectNameFormatString</span></span>|<span data-ttu-id="ab774-207">String</span><span class="sxs-lookup"><span data-stu-id="ab774-207">String</span></span>|<span data-ttu-id="ab774-208">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="ab774-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ab774-209">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="ab774-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ab774-210">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="ab774-210">keyUsage</span></span>|[<span data-ttu-id="ab774-211">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="ab774-211">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ab774-212">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="ab774-212">SCEP Key Usage.</span></span> <span data-ttu-id="ab774-213">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="ab774-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ab774-214">keySize</span><span class="sxs-lookup"><span data-stu-id="ab774-214">keySize</span></span>|[<span data-ttu-id="ab774-215">keySize</span><span class="sxs-lookup"><span data-stu-id="ab774-215">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ab774-216">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="ab774-216">SCEP Key Size.</span></span> <span data-ttu-id="ab774-217">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="ab774-217">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ab774-218">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="ab774-218">extendedKeyUsages</span></span>|<span data-ttu-id="ab774-219">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="ab774-219">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ab774-220">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="ab774-220">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ab774-221">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ab774-221">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ab774-222">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ab774-222">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ab774-223">String</span><span class="sxs-lookup"><span data-stu-id="ab774-223">String</span></span>|<span data-ttu-id="ab774-224">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="ab774-224">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="ab774-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ab774-225">certificateStore</span></span>|[<span data-ttu-id="ab774-226">certificateStore</span><span class="sxs-lookup"><span data-stu-id="ab774-226">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="ab774-227">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="ab774-227">Target store certificate.</span></span> <span data-ttu-id="ab774-228">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="ab774-228">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="ab774-229">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="ab774-229">customSubjectAlternativeNames</span></span>|<span data-ttu-id="ab774-230">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="ab774-230">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="ab774-231">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="ab774-231">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="ab774-232">Переменная OnPremisesUserPrincipalName также поддерживает и другие, описанные здесь: https://go.microsoft.com/fwlink/?LinkId=2027630.</span><span class="sxs-lookup"><span data-stu-id="ab774-232">The OnPremisesUserPrincipalName variable is support as well as others documented here: https://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="ab774-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ab774-233">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ab774-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab774-234">Response</span></span>
<span data-ttu-id="ab774-235">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab774-235">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab774-236">Пример</span><span class="sxs-lookup"><span data-stu-id="ab774-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab774-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab774-237">Request</span></span>
<span data-ttu-id="ab774-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab774-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ab774-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab774-239">Response</span></span>
<span data-ttu-id="ab774-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab774-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





