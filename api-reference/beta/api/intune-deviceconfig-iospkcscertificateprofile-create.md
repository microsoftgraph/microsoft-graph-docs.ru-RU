---
title: Создание iosPkcsCertificateProfile
description: Создание нового объекта iosPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f4c489b2e7fd1b4156521b1fe1819737bfb293b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995158"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="293f8-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="293f8-103">Create iosPkcsCertificateProfile</span></span>

<span data-ttu-id="293f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="293f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="293f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="293f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="293f8-107">Создание нового объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="293f8-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="293f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="293f8-108">Prerequisites</span></span>
<span data-ttu-id="293f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="293f8-111">Permission type</span></span>|<span data-ttu-id="293f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="293f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="293f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="293f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="293f8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293f8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="293f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="293f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="293f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293f8-116">Not supported.</span></span>|
|<span data-ttu-id="293f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="293f8-117">Application</span></span>|<span data-ttu-id="293f8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293f8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="293f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="293f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="293f8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="293f8-120">Request headers</span></span>
|<span data-ttu-id="293f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="293f8-121">Header</span></span>|<span data-ttu-id="293f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="293f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="293f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="293f8-123">Authorization</span></span>|<span data-ttu-id="293f8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="293f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="293f8-125">Accept</span></span>|<span data-ttu-id="293f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="293f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="293f8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="293f8-127">Request body</span></span>
<span data-ttu-id="293f8-128">В тексте запроса добавьте представление объекта iosPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="293f8-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="293f8-129">В следующей таблице приведены свойства, необходимые при создании iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="293f8-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="293f8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="293f8-130">Property</span></span>|<span data-ttu-id="293f8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="293f8-131">Type</span></span>|<span data-ttu-id="293f8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="293f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293f8-133">id</span><span class="sxs-lookup"><span data-stu-id="293f8-133">id</span></span>|<span data-ttu-id="293f8-134">String</span><span class="sxs-lookup"><span data-stu-id="293f8-134">String</span></span>|<span data-ttu-id="293f8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="293f8-135">Key of the entity.</span></span> <span data-ttu-id="293f8-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="293f8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="293f8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="293f8-138">DateTimeOffset</span></span>|<span data-ttu-id="293f8-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="293f8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="293f8-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="293f8-141">roleScopeTagIds</span></span>|<span data-ttu-id="293f8-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="293f8-142">String collection</span></span>|<span data-ttu-id="293f8-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="293f8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="293f8-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="293f8-145">supportsScopeTags</span></span>|<span data-ttu-id="293f8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="293f8-146">Boolean</span></span>|<span data-ttu-id="293f8-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="293f8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="293f8-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="293f8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="293f8-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="293f8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="293f8-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="293f8-150">This property is read-only.</span></span> <span data-ttu-id="293f8-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="293f8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="293f8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="293f8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="293f8-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="293f8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="293f8-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="293f8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="293f8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="293f8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="293f8-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="293f8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="293f8-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="293f8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="293f8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="293f8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="293f8-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="293f8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="293f8-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="293f8-164">createdDateTime</span></span>|<span data-ttu-id="293f8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="293f8-165">DateTimeOffset</span></span>|<span data-ttu-id="293f8-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="293f8-166">DateTime the object was created.</span></span> <span data-ttu-id="293f8-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-168">description</span><span class="sxs-lookup"><span data-stu-id="293f8-168">description</span></span>|<span data-ttu-id="293f8-169">String</span><span class="sxs-lookup"><span data-stu-id="293f8-169">String</span></span>|<span data-ttu-id="293f8-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="293f8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="293f8-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="293f8-172">displayName</span></span>|<span data-ttu-id="293f8-173">String</span><span class="sxs-lookup"><span data-stu-id="293f8-173">String</span></span>|<span data-ttu-id="293f8-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="293f8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="293f8-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-176">version</span><span class="sxs-lookup"><span data-stu-id="293f8-176">version</span></span>|<span data-ttu-id="293f8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="293f8-177">Int32</span></span>|<span data-ttu-id="293f8-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="293f8-178">Version of the device configuration.</span></span> <span data-ttu-id="293f8-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="293f8-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="293f8-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="293f8-181">Int32</span><span class="sxs-lookup"><span data-stu-id="293f8-181">Int32</span></span>|<span data-ttu-id="293f8-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="293f8-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="293f8-183">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="293f8-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="293f8-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="293f8-184">subjectNameFormat</span></span>|[<span data-ttu-id="293f8-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="293f8-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="293f8-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="293f8-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="293f8-187">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="293f8-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="293f8-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="293f8-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="293f8-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="293f8-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="293f8-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="293f8-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="293f8-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="293f8-192">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="293f8-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="293f8-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="293f8-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="293f8-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="293f8-195">Int32</span><span class="sxs-lookup"><span data-stu-id="293f8-195">Int32</span></span>|<span data-ttu-id="293f8-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="293f8-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="293f8-197">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="293f8-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="293f8-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="293f8-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="293f8-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="293f8-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="293f8-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="293f8-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="293f8-201">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="293f8-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="293f8-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="293f8-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="293f8-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="293f8-203">certificationAuthority</span></span>|<span data-ttu-id="293f8-204">String</span><span class="sxs-lookup"><span data-stu-id="293f8-204">String</span></span>|<span data-ttu-id="293f8-205">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="293f8-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="293f8-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="293f8-206">certificationAuthorityName</span></span>|<span data-ttu-id="293f8-207">String</span><span class="sxs-lookup"><span data-stu-id="293f8-207">String</span></span>|<span data-ttu-id="293f8-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="293f8-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="293f8-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="293f8-209">certificateTemplateName</span></span>|<span data-ttu-id="293f8-210">String</span><span class="sxs-lookup"><span data-stu-id="293f8-210">String</span></span>|<span data-ttu-id="293f8-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="293f8-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="293f8-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="293f8-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="293f8-213">String</span><span class="sxs-lookup"><span data-stu-id="293f8-213">String</span></span>|<span data-ttu-id="293f8-214">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="293f8-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="293f8-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="293f8-215">subjectNameFormatString</span></span>|<span data-ttu-id="293f8-216">String</span><span class="sxs-lookup"><span data-stu-id="293f8-216">String</span></span>|<span data-ttu-id="293f8-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="293f8-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="293f8-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="293f8-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="293f8-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="293f8-219">certificateStore</span></span>|[<span data-ttu-id="293f8-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="293f8-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="293f8-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="293f8-221">Target store certificate.</span></span> <span data-ttu-id="293f8-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="293f8-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="293f8-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="293f8-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="293f8-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="293f8-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="293f8-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="293f8-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="293f8-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="293f8-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="293f8-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="293f8-227">Response</span></span>
<span data-ttu-id="293f8-228">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="293f8-228">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293f8-229">Пример</span><span class="sxs-lookup"><span data-stu-id="293f8-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="293f8-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="293f8-230">Request</span></span>
<span data-ttu-id="293f8-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="293f8-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1824

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="293f8-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="293f8-232">Response</span></span>
<span data-ttu-id="293f8-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="293f8-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1996

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  ]
}
```






