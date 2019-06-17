---
title: Обновление iosPkcsCertificateProfile
description: Обновление свойств объекта iosPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77879a44a4964283f29be33dcd3d8ef39521db65
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963683"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="5b371-103">Обновление iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5b371-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="5b371-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b371-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b371-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b371-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b371-106">Обновление свойств объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5b371-106">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b371-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b371-107">Prerequisites</span></span>
<span data-ttu-id="5b371-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b371-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b371-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b371-110">Permission type</span></span>|<span data-ttu-id="5b371-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b371-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b371-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b371-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b371-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b371-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b371-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b371-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b371-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b371-115">Not supported.</span></span>|
|<span data-ttu-id="5b371-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b371-116">Application</span></span>|<span data-ttu-id="5b371-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b371-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b371-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b371-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b371-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b371-119">Request headers</span></span>
|<span data-ttu-id="5b371-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b371-120">Header</span></span>|<span data-ttu-id="5b371-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b371-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b371-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b371-122">Authorization</span></span>|<span data-ttu-id="5b371-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b371-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b371-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5b371-124">Accept</span></span>|<span data-ttu-id="5b371-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b371-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b371-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5b371-126">Request body</span></span>
<span data-ttu-id="5b371-127">В тексте запроса добавьте представление объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b371-127">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="5b371-128">В следующей таблице приведены свойства, необходимые при создании [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-128">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="5b371-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b371-129">Property</span></span>|<span data-ttu-id="5b371-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5b371-130">Type</span></span>|<span data-ttu-id="5b371-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5b371-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b371-132">id</span><span class="sxs-lookup"><span data-stu-id="5b371-132">id</span></span>|<span data-ttu-id="5b371-133">String</span><span class="sxs-lookup"><span data-stu-id="5b371-133">String</span></span>|<span data-ttu-id="5b371-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b371-134">Key of the entity.</span></span> <span data-ttu-id="5b371-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b371-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5b371-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b371-137">DateTimeOffset</span></span>|<span data-ttu-id="5b371-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5b371-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5b371-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b371-140">roleScopeTagIds</span></span>|<span data-ttu-id="5b371-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5b371-141">String collection</span></span>|<span data-ttu-id="5b371-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5b371-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b371-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5b371-144">supportsScopeTags</span></span>|<span data-ttu-id="5b371-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b371-145">Boolean</span></span>|<span data-ttu-id="5b371-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5b371-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b371-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5b371-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b371-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5b371-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b371-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b371-149">This property is read-only.</span></span> <span data-ttu-id="5b371-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b371-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5b371-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5b371-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5b371-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b371-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5b371-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b371-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5b371-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5b371-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5b371-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b371-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5b371-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5b371-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5b371-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="5b371-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5b371-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5b371-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5b371-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b371-163">createdDateTime</span></span>|<span data-ttu-id="5b371-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b371-164">DateTimeOffset</span></span>|<span data-ttu-id="5b371-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5b371-165">DateTime the object was created.</span></span> <span data-ttu-id="5b371-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-167">description</span><span class="sxs-lookup"><span data-stu-id="5b371-167">description</span></span>|<span data-ttu-id="5b371-168">String</span><span class="sxs-lookup"><span data-stu-id="5b371-168">String</span></span>|<span data-ttu-id="5b371-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b371-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b371-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5b371-171">displayName</span></span>|<span data-ttu-id="5b371-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5b371-172">String</span></span>|<span data-ttu-id="5b371-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b371-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b371-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-175">version</span><span class="sxs-lookup"><span data-stu-id="5b371-175">version</span></span>|<span data-ttu-id="5b371-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5b371-176">Int32</span></span>|<span data-ttu-id="5b371-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5b371-177">Version of the device configuration.</span></span> <span data-ttu-id="5b371-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b371-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="5b371-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="5b371-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5b371-180">Int32</span></span>|<span data-ttu-id="5b371-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="5b371-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5b371-182">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5b371-182">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5b371-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5b371-183">subjectNameFormat</span></span>|[<span data-ttu-id="5b371-184">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="5b371-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5b371-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5b371-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="5b371-186">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-186">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5b371-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5b371-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5b371-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5b371-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5b371-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5b371-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5b371-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5b371-190">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="5b371-191">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-191">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5b371-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5b371-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5b371-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5b371-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5b371-194">Int32</span><span class="sxs-lookup"><span data-stu-id="5b371-194">Int32</span></span>|<span data-ttu-id="5b371-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5b371-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5b371-196">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5b371-196">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5b371-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5b371-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5b371-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5b371-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5b371-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5b371-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5b371-200">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5b371-200">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5b371-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5b371-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5b371-202">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="5b371-202">certificationAuthority</span></span>|<span data-ttu-id="5b371-203">String</span><span class="sxs-lookup"><span data-stu-id="5b371-203">String</span></span>|<span data-ttu-id="5b371-204">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="5b371-204">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="5b371-205">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="5b371-205">certificationAuthorityName</span></span>|<span data-ttu-id="5b371-206">String</span><span class="sxs-lookup"><span data-stu-id="5b371-206">String</span></span>|<span data-ttu-id="5b371-207">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="5b371-207">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="5b371-208">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="5b371-208">certificateTemplateName</span></span>|<span data-ttu-id="5b371-209">String</span><span class="sxs-lookup"><span data-stu-id="5b371-209">String</span></span>|<span data-ttu-id="5b371-210">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="5b371-210">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="5b371-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5b371-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5b371-212">String</span><span class="sxs-lookup"><span data-stu-id="5b371-212">String</span></span>|<span data-ttu-id="5b371-213">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="5b371-213">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="5b371-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b371-214">Response</span></span>
<span data-ttu-id="5b371-215">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b371-215">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b371-216">Пример</span><span class="sxs-lookup"><span data-stu-id="5b371-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b371-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b371-217">Request</span></span>
<span data-ttu-id="5b371-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b371-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1534

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="5b371-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b371-219">Response</span></span>
<span data-ttu-id="5b371-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b371-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1706

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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





