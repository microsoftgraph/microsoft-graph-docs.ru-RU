---
title: Обновление iosPkcsCertificateProfile
description: Обновление свойств объекта iosPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4329f46b4714919aa12aca38cc6d378d1291318c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448846"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="06c8b-103">Обновление iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="06c8b-103">Update iosPkcsCertificateProfile</span></span>

<span data-ttu-id="06c8b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06c8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06c8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06c8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06c8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c8b-107">Обновление свойств объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="06c8b-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06c8b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06c8b-108">Prerequisites</span></span>
<span data-ttu-id="06c8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06c8b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06c8b-111">Permission type</span></span>|<span data-ttu-id="06c8b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06c8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c8b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06c8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06c8b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c8b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06c8b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06c8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c8b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06c8b-116">Not supported.</span></span>|
|<span data-ttu-id="06c8b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06c8b-117">Application</span></span>|<span data-ttu-id="06c8b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c8b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c8b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06c8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06c8b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="06c8b-120">Request headers</span></span>
|<span data-ttu-id="06c8b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06c8b-121">Header</span></span>|<span data-ttu-id="06c8b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="06c8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c8b-123">Authorization</span></span>|<span data-ttu-id="06c8b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06c8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="06c8b-125">Accept</span></span>|<span data-ttu-id="06c8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06c8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c8b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06c8b-127">Request body</span></span>
<span data-ttu-id="06c8b-128">В тексте запроса добавьте представление объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06c8b-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="06c8b-129">В следующей таблице приведены свойства, необходимые при создании [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="06c8b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="06c8b-130">Property</span></span>|<span data-ttu-id="06c8b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="06c8b-131">Type</span></span>|<span data-ttu-id="06c8b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="06c8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06c8b-133">id</span><span class="sxs-lookup"><span data-stu-id="06c8b-133">id</span></span>|<span data-ttu-id="06c8b-134">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-134">String</span></span>|<span data-ttu-id="06c8b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="06c8b-135">Key of the entity.</span></span> <span data-ttu-id="06c8b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06c8b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="06c8b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c8b-138">DateTimeOffset</span></span>|<span data-ttu-id="06c8b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="06c8b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="06c8b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06c8b-141">roleScopeTagIds</span></span>|<span data-ttu-id="06c8b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06c8b-142">String collection</span></span>|<span data-ttu-id="06c8b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="06c8b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06c8b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="06c8b-145">supportsScopeTags</span></span>|<span data-ttu-id="06c8b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="06c8b-146">Boolean</span></span>|<span data-ttu-id="06c8b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="06c8b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06c8b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="06c8b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06c8b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="06c8b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06c8b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="06c8b-150">This property is read-only.</span></span> <span data-ttu-id="06c8b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06c8b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="06c8b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06c8b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="06c8b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="06c8b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="06c8b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06c8b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="06c8b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06c8b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="06c8b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="06c8b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="06c8b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06c8b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="06c8b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06c8b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="06c8b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="06c8b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="06c8b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06c8b-164">createdDateTime</span></span>|<span data-ttu-id="06c8b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06c8b-165">DateTimeOffset</span></span>|<span data-ttu-id="06c8b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="06c8b-166">DateTime the object was created.</span></span> <span data-ttu-id="06c8b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-168">description</span><span class="sxs-lookup"><span data-stu-id="06c8b-168">description</span></span>|<span data-ttu-id="06c8b-169">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-169">String</span></span>|<span data-ttu-id="06c8b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06c8b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06c8b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="06c8b-172">displayName</span></span>|<span data-ttu-id="06c8b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="06c8b-173">String</span></span>|<span data-ttu-id="06c8b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06c8b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06c8b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-176">version</span><span class="sxs-lookup"><span data-stu-id="06c8b-176">version</span></span>|<span data-ttu-id="06c8b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="06c8b-177">Int32</span></span>|<span data-ttu-id="06c8b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="06c8b-178">Version of the device configuration.</span></span> <span data-ttu-id="06c8b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06c8b-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="06c8b-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="06c8b-181">Int32</span><span class="sxs-lookup"><span data-stu-id="06c8b-181">Int32</span></span>|<span data-ttu-id="06c8b-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="06c8b-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="06c8b-183">Допустимые значения — от 1 до 99, наследуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="06c8b-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="06c8b-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="06c8b-184">subjectNameFormat</span></span>|[<span data-ttu-id="06c8b-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="06c8b-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="06c8b-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="06c8b-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="06c8b-187">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="06c8b-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="06c8b-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="06c8b-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="06c8b-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="06c8b-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="06c8b-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="06c8b-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="06c8b-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="06c8b-192">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="06c8b-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="06c8b-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="06c8b-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="06c8b-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="06c8b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="06c8b-195">Int32</span></span>|<span data-ttu-id="06c8b-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="06c8b-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="06c8b-197">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="06c8b-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="06c8b-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="06c8b-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="06c8b-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="06c8b-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="06c8b-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="06c8b-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="06c8b-201">Наследуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="06c8b-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="06c8b-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="06c8b-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="06c8b-203">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="06c8b-203">certificationAuthority</span></span>|<span data-ttu-id="06c8b-204">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-204">String</span></span>|<span data-ttu-id="06c8b-205">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="06c8b-205">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="06c8b-206">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="06c8b-206">certificationAuthorityName</span></span>|<span data-ttu-id="06c8b-207">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-207">String</span></span>|<span data-ttu-id="06c8b-208">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="06c8b-208">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="06c8b-209">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="06c8b-209">certificateTemplateName</span></span>|<span data-ttu-id="06c8b-210">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-210">String</span></span>|<span data-ttu-id="06c8b-211">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="06c8b-211">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="06c8b-212">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="06c8b-212">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="06c8b-213">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-213">String</span></span>|<span data-ttu-id="06c8b-214">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="06c8b-214">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="06c8b-215">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="06c8b-215">subjectNameFormatString</span></span>|<span data-ttu-id="06c8b-216">String</span><span class="sxs-lookup"><span data-stu-id="06c8b-216">String</span></span>|<span data-ttu-id="06c8b-217">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="06c8b-217">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="06c8b-218">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="06c8b-218">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="06c8b-219">certificateStore</span><span class="sxs-lookup"><span data-stu-id="06c8b-219">certificateStore</span></span>|[<span data-ttu-id="06c8b-220">certificateStore</span><span class="sxs-lookup"><span data-stu-id="06c8b-220">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="06c8b-221">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="06c8b-221">Target store certificate.</span></span> <span data-ttu-id="06c8b-222">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="06c8b-222">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="06c8b-223">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="06c8b-223">customSubjectAlternativeNames</span></span>|<span data-ttu-id="06c8b-224">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="06c8b-224">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="06c8b-225">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="06c8b-225">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="06c8b-226">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="06c8b-226">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="06c8b-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="06c8b-227">Response</span></span>
<span data-ttu-id="06c8b-228">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06c8b-228">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c8b-229">Пример</span><span class="sxs-lookup"><span data-stu-id="06c8b-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="06c8b-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="06c8b-230">Request</span></span>
<span data-ttu-id="06c8b-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06c8b-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="06c8b-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="06c8b-232">Response</span></span>
<span data-ttu-id="06c8b-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06c8b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





