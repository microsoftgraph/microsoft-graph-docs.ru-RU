---
title: Создание iosPkcsCertificateProfile
description: Создание нового объекта iosPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a55acb790e4d5b13d2ffb23724d0a955421e7be
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220457"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="690d4-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="690d4-103">Create iosPkcsCertificateProfile</span></span>

<span data-ttu-id="690d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="690d4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="690d4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="690d4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="690d4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="690d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="690d4-107">Создание нового объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="690d4-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="690d4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="690d4-108">Prerequisites</span></span>
<span data-ttu-id="690d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="690d4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="690d4-111">Permission type</span></span>|<span data-ttu-id="690d4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="690d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="690d4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="690d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="690d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="690d4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="690d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="690d4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="690d4-116">Not supported.</span></span>|
|<span data-ttu-id="690d4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="690d4-117">Application</span></span>|<span data-ttu-id="690d4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="690d4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="690d4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="690d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="690d4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="690d4-120">Request headers</span></span>
|<span data-ttu-id="690d4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="690d4-121">Header</span></span>|<span data-ttu-id="690d4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="690d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="690d4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="690d4-123">Authorization</span></span>|<span data-ttu-id="690d4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="690d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="690d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="690d4-125">Accept</span></span>|<span data-ttu-id="690d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="690d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="690d4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="690d4-127">Request body</span></span>
<span data-ttu-id="690d4-128">В тексте запроса добавьте представление объекта iosPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="690d4-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="690d4-129">В следующей таблице приведены свойства, необходимые при создании iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="690d4-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="690d4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="690d4-130">Property</span></span>|<span data-ttu-id="690d4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="690d4-131">Type</span></span>|<span data-ttu-id="690d4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="690d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="690d4-133">id</span><span class="sxs-lookup"><span data-stu-id="690d4-133">id</span></span>|<span data-ttu-id="690d4-134">String</span><span class="sxs-lookup"><span data-stu-id="690d4-134">String</span></span>|<span data-ttu-id="690d4-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="690d4-135">Key of the entity.</span></span> <span data-ttu-id="690d4-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="690d4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="690d4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690d4-138">DateTimeOffset</span></span>|<span data-ttu-id="690d4-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="690d4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="690d4-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="690d4-141">roleScopeTagIds</span></span>|<span data-ttu-id="690d4-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="690d4-142">String collection</span></span>|<span data-ttu-id="690d4-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="690d4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="690d4-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="690d4-145">supportsScopeTags</span></span>|<span data-ttu-id="690d4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="690d4-146">Boolean</span></span>|<span data-ttu-id="690d4-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="690d4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="690d4-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="690d4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="690d4-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="690d4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="690d4-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="690d4-150">This property is read-only.</span></span> <span data-ttu-id="690d4-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="690d4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="690d4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="690d4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="690d4-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="690d4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="690d4-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="690d4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="690d4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="690d4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="690d4-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="690d4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="690d4-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="690d4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="690d4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="690d4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="690d4-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="690d4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="690d4-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="690d4-164">createdDateTime</span></span>|<span data-ttu-id="690d4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="690d4-165">DateTimeOffset</span></span>|<span data-ttu-id="690d4-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="690d4-166">DateTime the object was created.</span></span> <span data-ttu-id="690d4-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-168">description</span><span class="sxs-lookup"><span data-stu-id="690d4-168">description</span></span>|<span data-ttu-id="690d4-169">String</span><span class="sxs-lookup"><span data-stu-id="690d4-169">String</span></span>|<span data-ttu-id="690d4-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="690d4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="690d4-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="690d4-172">displayName</span></span>|<span data-ttu-id="690d4-173">String</span><span class="sxs-lookup"><span data-stu-id="690d4-173">String</span></span>|<span data-ttu-id="690d4-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="690d4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="690d4-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-176">version</span><span class="sxs-lookup"><span data-stu-id="690d4-176">version</span></span>|<span data-ttu-id="690d4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="690d4-177">Int32</span></span>|<span data-ttu-id="690d4-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="690d4-178">Version of the device configuration.</span></span> <span data-ttu-id="690d4-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="690d4-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="690d4-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="690d4-181">Int32</span><span class="sxs-lookup"><span data-stu-id="690d4-181">Int32</span></span>|<span data-ttu-id="690d4-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="690d4-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="690d4-183">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="690d4-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="690d4-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="690d4-184">subjectNameFormat</span></span>|[<span data-ttu-id="690d4-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="690d4-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="690d4-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="690d4-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="690d4-187">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="690d4-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="690d4-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="690d4-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="690d4-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="690d4-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="690d4-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="690d4-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="690d4-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="690d4-192">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="690d4-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="690d4-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="690d4-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="690d4-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="690d4-195">Int32</span><span class="sxs-lookup"><span data-stu-id="690d4-195">Int32</span></span>|<span data-ttu-id="690d4-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="690d4-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="690d4-197">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="690d4-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="690d4-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="690d4-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="690d4-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="690d4-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="690d4-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="690d4-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="690d4-201">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="690d4-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="690d4-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="690d4-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="690d4-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="690d4-203">certificationAuthority</span></span>|<span data-ttu-id="690d4-204">String</span><span class="sxs-lookup"><span data-stu-id="690d4-204">String</span></span>|<span data-ttu-id="690d4-205">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="690d4-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="690d4-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="690d4-206">certificationAuthorityName</span></span>|<span data-ttu-id="690d4-207">String</span><span class="sxs-lookup"><span data-stu-id="690d4-207">String</span></span>|<span data-ttu-id="690d4-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="690d4-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="690d4-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="690d4-209">certificateTemplateName</span></span>|<span data-ttu-id="690d4-210">String</span><span class="sxs-lookup"><span data-stu-id="690d4-210">String</span></span>|<span data-ttu-id="690d4-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="690d4-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="690d4-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="690d4-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="690d4-213">String</span><span class="sxs-lookup"><span data-stu-id="690d4-213">String</span></span>|<span data-ttu-id="690d4-214">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="690d4-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="690d4-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="690d4-215">subjectNameFormatString</span></span>|<span data-ttu-id="690d4-216">String</span><span class="sxs-lookup"><span data-stu-id="690d4-216">String</span></span>|<span data-ttu-id="690d4-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="690d4-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="690d4-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="690d4-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="690d4-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="690d4-219">certificateStore</span></span>|[<span data-ttu-id="690d4-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="690d4-220">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="690d4-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="690d4-221">Target store certificate.</span></span> <span data-ttu-id="690d4-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="690d4-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="690d4-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="690d4-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="690d4-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="690d4-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="690d4-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="690d4-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="690d4-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="690d4-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="690d4-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="690d4-227">Response</span></span>
<span data-ttu-id="690d4-228">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="690d4-228">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="690d4-229">Пример</span><span class="sxs-lookup"><span data-stu-id="690d4-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="690d4-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="690d4-230">Request</span></span>
<span data-ttu-id="690d4-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="690d4-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="690d4-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="690d4-232">Response</span></span>
<span data-ttu-id="690d4-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="690d4-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




