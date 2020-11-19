---
title: Обновление androidPkcsCertificateProfile
description: Обновление свойств объекта androidPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5934af8c704d218b9b6a948f1b6091546dc5b730
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221731"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="3d368-103">Обновление androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3d368-103">Update androidPkcsCertificateProfile</span></span>

<span data-ttu-id="3d368-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d368-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d368-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d368-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d368-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d368-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d368-107">Обновление свойств объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3d368-107">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d368-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d368-108">Prerequisites</span></span>
<span data-ttu-id="3d368-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d368-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d368-111">Permission type</span></span>|<span data-ttu-id="3d368-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d368-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d368-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d368-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d368-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d368-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d368-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d368-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d368-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d368-116">Not supported.</span></span>|
|<span data-ttu-id="3d368-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d368-117">Application</span></span>|<span data-ttu-id="3d368-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d368-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d368-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d368-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3d368-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d368-120">Request headers</span></span>
|<span data-ttu-id="3d368-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d368-121">Header</span></span>|<span data-ttu-id="3d368-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d368-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d368-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d368-123">Authorization</span></span>|<span data-ttu-id="3d368-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d368-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d368-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d368-125">Accept</span></span>|<span data-ttu-id="3d368-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d368-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d368-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d368-127">Request body</span></span>
<span data-ttu-id="3d368-128">В тексте запроса добавьте представление объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d368-128">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="3d368-129">В следующей таблице приведены свойства, необходимые при создании [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-129">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="3d368-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d368-130">Property</span></span>|<span data-ttu-id="3d368-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d368-131">Type</span></span>|<span data-ttu-id="3d368-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d368-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d368-133">id</span><span class="sxs-lookup"><span data-stu-id="3d368-133">id</span></span>|<span data-ttu-id="3d368-134">String</span><span class="sxs-lookup"><span data-stu-id="3d368-134">String</span></span>|<span data-ttu-id="3d368-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3d368-135">Key of the entity.</span></span> <span data-ttu-id="3d368-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d368-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3d368-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d368-138">DateTimeOffset</span></span>|<span data-ttu-id="3d368-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3d368-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3d368-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d368-141">roleScopeTagIds</span></span>|<span data-ttu-id="3d368-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3d368-142">String collection</span></span>|<span data-ttu-id="3d368-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3d368-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3d368-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="3d368-145">supportsScopeTags</span></span>|<span data-ttu-id="3d368-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d368-146">Boolean</span></span>|<span data-ttu-id="3d368-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3d368-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3d368-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="3d368-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3d368-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3d368-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3d368-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d368-150">This property is read-only.</span></span> <span data-ttu-id="3d368-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3d368-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3d368-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3d368-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3d368-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3d368-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3d368-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3d368-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3d368-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3d368-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3d368-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3d368-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3d368-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3d368-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3d368-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3d368-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3d368-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3d368-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3d368-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d368-164">createdDateTime</span></span>|<span data-ttu-id="3d368-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d368-165">DateTimeOffset</span></span>|<span data-ttu-id="3d368-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3d368-166">DateTime the object was created.</span></span> <span data-ttu-id="3d368-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-168">description</span><span class="sxs-lookup"><span data-stu-id="3d368-168">description</span></span>|<span data-ttu-id="3d368-169">String</span><span class="sxs-lookup"><span data-stu-id="3d368-169">String</span></span>|<span data-ttu-id="3d368-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d368-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d368-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3d368-172">displayName</span></span>|<span data-ttu-id="3d368-173">String</span><span class="sxs-lookup"><span data-stu-id="3d368-173">String</span></span>|<span data-ttu-id="3d368-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d368-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d368-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-176">version</span><span class="sxs-lookup"><span data-stu-id="3d368-176">version</span></span>|<span data-ttu-id="3d368-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3d368-177">Int32</span></span>|<span data-ttu-id="3d368-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d368-178">Version of the device configuration.</span></span> <span data-ttu-id="3d368-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d368-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="3d368-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="3d368-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3d368-181">Int32</span></span>|<span data-ttu-id="3d368-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d368-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3d368-183">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3d368-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3d368-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3d368-184">subjectNameFormat</span></span>|[<span data-ttu-id="3d368-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3d368-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3d368-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d368-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="3d368-187">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3d368-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3d368-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3d368-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3d368-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3d368-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3d368-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="3d368-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d368-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="3d368-192">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3d368-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="3d368-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="3d368-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3d368-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3d368-195">Int32</span><span class="sxs-lookup"><span data-stu-id="3d368-195">Int32</span></span>|<span data-ttu-id="3d368-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d368-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3d368-197">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3d368-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3d368-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3d368-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3d368-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3d368-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="3d368-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d368-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3d368-201">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d368-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="3d368-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3d368-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3d368-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="3d368-203">extendedKeyUsages</span></span>|<span data-ttu-id="3d368-204">Коллекция [екстендедкэйусаже](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="3d368-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="3d368-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="3d368-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="3d368-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="3d368-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3d368-207">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3d368-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3d368-208">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="3d368-208">certificationAuthority</span></span>|<span data-ttu-id="3d368-209">String</span><span class="sxs-lookup"><span data-stu-id="3d368-209">String</span></span>|<span data-ttu-id="3d368-210">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3d368-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="3d368-211">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="3d368-211">certificationAuthorityName</span></span>|<span data-ttu-id="3d368-212">String</span><span class="sxs-lookup"><span data-stu-id="3d368-212">String</span></span>|<span data-ttu-id="3d368-213">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="3d368-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="3d368-214">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="3d368-214">certificateTemplateName</span></span>|<span data-ttu-id="3d368-215">String</span><span class="sxs-lookup"><span data-stu-id="3d368-215">String</span></span>|<span data-ttu-id="3d368-216">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="3d368-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="3d368-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3d368-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3d368-218">String</span><span class="sxs-lookup"><span data-stu-id="3d368-218">String</span></span>|<span data-ttu-id="3d368-219">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="3d368-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3d368-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d368-220">Response</span></span>
<span data-ttu-id="3d368-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d368-221">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d368-222">Пример</span><span class="sxs-lookup"><span data-stu-id="3d368-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d368-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d368-223">Request</span></span>
<span data-ttu-id="3d368-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d368-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1731

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="3d368-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d368-225">Response</span></span>
<span data-ttu-id="3d368-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d368-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1903

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




