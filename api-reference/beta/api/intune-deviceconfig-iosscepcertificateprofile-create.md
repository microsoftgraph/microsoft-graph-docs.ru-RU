---
title: Создание iosScepCertificateProfile
description: Создание нового объекта iosScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d32e7ef3c409e4c6089ffc83b3c27af130b140f5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315830"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="e7418-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e7418-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="e7418-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7418-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7418-106">Создание нового объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e7418-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7418-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e7418-107">Prerequisites</span></span>
<span data-ttu-id="e7418-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7418-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7418-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7418-110">Permission type</span></span>|<span data-ttu-id="e7418-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7418-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7418-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7418-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7418-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7418-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7418-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7418-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7418-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7418-115">Not supported.</span></span>|
|<span data-ttu-id="e7418-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7418-116">Application</span></span>|<span data-ttu-id="e7418-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7418-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7418-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7418-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7418-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7418-119">Request headers</span></span>
|<span data-ttu-id="e7418-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7418-120">Header</span></span>|<span data-ttu-id="e7418-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e7418-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7418-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7418-122">Authorization</span></span>|<span data-ttu-id="e7418-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7418-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7418-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7418-124">Accept</span></span>|<span data-ttu-id="e7418-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7418-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7418-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7418-126">Request body</span></span>
<span data-ttu-id="e7418-127">В тексте запроса добавьте представление объекта iosScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7418-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="e7418-128">В следующей таблице приведены свойства, необходимые при создании iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="e7418-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="e7418-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7418-129">Property</span></span>|<span data-ttu-id="e7418-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e7418-130">Type</span></span>|<span data-ttu-id="e7418-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e7418-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7418-132">id</span><span class="sxs-lookup"><span data-stu-id="e7418-132">id</span></span>|<span data-ttu-id="e7418-133">String</span><span class="sxs-lookup"><span data-stu-id="e7418-133">String</span></span>|<span data-ttu-id="e7418-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e7418-134">Key of the entity.</span></span> <span data-ttu-id="e7418-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7418-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7418-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7418-137">DateTimeOffset</span></span>|<span data-ttu-id="e7418-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e7418-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7418-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7418-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7418-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7418-141">String collection</span></span>|<span data-ttu-id="e7418-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e7418-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7418-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e7418-144">supportsScopeTags</span></span>|<span data-ttu-id="e7418-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7418-145">Boolean</span></span>|<span data-ttu-id="e7418-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e7418-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7418-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e7418-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7418-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e7418-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7418-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7418-149">This property is read-only.</span></span> <span data-ttu-id="e7418-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7418-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e7418-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e7418-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e7418-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7418-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e7418-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7418-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e7418-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e7418-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e7418-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7418-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e7418-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e7418-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e7418-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="e7418-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e7418-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e7418-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e7418-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7418-163">createdDateTime</span></span>|<span data-ttu-id="e7418-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7418-164">DateTimeOffset</span></span>|<span data-ttu-id="e7418-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e7418-165">DateTime the object was created.</span></span> <span data-ttu-id="e7418-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-167">description</span><span class="sxs-lookup"><span data-stu-id="e7418-167">description</span></span>|<span data-ttu-id="e7418-168">String</span><span class="sxs-lookup"><span data-stu-id="e7418-168">String</span></span>|<span data-ttu-id="e7418-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7418-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7418-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e7418-171">displayName</span></span>|<span data-ttu-id="e7418-172">Строка</span><span class="sxs-lookup"><span data-stu-id="e7418-172">String</span></span>|<span data-ttu-id="e7418-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7418-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7418-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-175">version</span><span class="sxs-lookup"><span data-stu-id="e7418-175">version</span></span>|<span data-ttu-id="e7418-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e7418-176">Int32</span></span>|<span data-ttu-id="e7418-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e7418-177">Version of the device configuration.</span></span> <span data-ttu-id="e7418-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7418-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="e7418-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="e7418-180">Int32</span><span class="sxs-lookup"><span data-stu-id="e7418-180">Int32</span></span>|<span data-ttu-id="e7418-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="e7418-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e7418-182">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e7418-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e7418-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e7418-183">subjectNameFormat</span></span>|[<span data-ttu-id="e7418-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="e7418-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="e7418-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e7418-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="e7418-186">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="e7418-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="e7418-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="e7418-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e7418-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e7418-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e7418-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e7418-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e7418-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="e7418-191">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="e7418-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e7418-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e7418-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e7418-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e7418-194">Int32</span><span class="sxs-lookup"><span data-stu-id="e7418-194">Int32</span></span>|<span data-ttu-id="e7418-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e7418-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="e7418-196">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e7418-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="e7418-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e7418-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e7418-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e7418-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e7418-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e7418-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e7418-200">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e7418-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="e7418-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e7418-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e7418-202">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="e7418-202">scepServerUrls</span></span>|<span data-ttu-id="e7418-203">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e7418-203">String collection</span></span>|<span data-ttu-id="e7418-204">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="e7418-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="e7418-205">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="e7418-205">subjectNameFormatString</span></span>|<span data-ttu-id="e7418-206">String</span><span class="sxs-lookup"><span data-stu-id="e7418-206">String</span></span>|<span data-ttu-id="e7418-207">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="e7418-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="e7418-208">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="e7418-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="e7418-209">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="e7418-209">keyUsage</span></span>|[<span data-ttu-id="e7418-210">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="e7418-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e7418-211">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="e7418-211">SCEP Key Usage.</span></span> <span data-ttu-id="e7418-212">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e7418-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e7418-213">keySize</span><span class="sxs-lookup"><span data-stu-id="e7418-213">keySize</span></span>|[<span data-ttu-id="e7418-214">keySize</span><span class="sxs-lookup"><span data-stu-id="e7418-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="e7418-215">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="e7418-215">SCEP Key Size.</span></span> <span data-ttu-id="e7418-216">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="e7418-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="e7418-217">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="e7418-217">extendedKeyUsages</span></span>|<span data-ttu-id="e7418-218">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="e7418-218">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e7418-219">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="e7418-219">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e7418-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e7418-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e7418-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e7418-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e7418-222">String</span><span class="sxs-lookup"><span data-stu-id="e7418-222">String</span></span>|<span data-ttu-id="e7418-223">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="e7418-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="e7418-224">certificateStore</span><span class="sxs-lookup"><span data-stu-id="e7418-224">certificateStore</span></span>|[<span data-ttu-id="e7418-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="e7418-225">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="e7418-226">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="e7418-226">Target store certificate.</span></span> <span data-ttu-id="e7418-227">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="e7418-227">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="e7418-228">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="e7418-228">customSubjectAlternativeNames</span></span>|<span data-ttu-id="e7418-229">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="e7418-229">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="e7418-230">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="e7418-230">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="e7418-231">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e7418-231">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e7418-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7418-232">Response</span></span>
<span data-ttu-id="e7418-233">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e7418-233">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7418-234">Пример</span><span class="sxs-lookup"><span data-stu-id="e7418-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7418-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7418-235">Request</span></span>
<span data-ttu-id="e7418-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7418-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e7418-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7418-237">Response</span></span>
<span data-ttu-id="e7418-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e7418-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






