---
title: Обновление Андроидимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Андроидимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c97e692b660317d70320ac88175eb9c686ebb534
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084792"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="c20c2-103">Обновление Андроидимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="c20c2-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="c20c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c20c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c20c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c20c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c20c2-106">Обновление свойств объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c20c2-106">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c20c2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c20c2-107">Prerequisites</span></span>
<span data-ttu-id="c20c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c20c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c20c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c20c2-110">Permission type</span></span>|<span data-ttu-id="c20c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c20c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c20c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c20c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c20c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c20c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c20c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c20c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c20c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c20c2-115">Not supported.</span></span>|
|<span data-ttu-id="c20c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c20c2-116">Application</span></span>|<span data-ttu-id="c20c2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c20c2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c20c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c20c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c20c2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c20c2-119">Request headers</span></span>
|<span data-ttu-id="c20c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c20c2-120">Header</span></span>|<span data-ttu-id="c20c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c20c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c20c2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c20c2-122">Authorization</span></span>|<span data-ttu-id="c20c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c20c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c20c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c20c2-124">Accept</span></span>|<span data-ttu-id="c20c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c20c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c20c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c20c2-126">Request body</span></span>
<span data-ttu-id="c20c2-127">В тексте запроса добавьте представление объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c20c2-127">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="c20c2-128">В следующей таблице приведены свойства, необходимые при создании [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-128">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="c20c2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c20c2-129">Property</span></span>|<span data-ttu-id="c20c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c20c2-130">Type</span></span>|<span data-ttu-id="c20c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c20c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c20c2-132">id</span><span class="sxs-lookup"><span data-stu-id="c20c2-132">id</span></span>|<span data-ttu-id="c20c2-133">String</span><span class="sxs-lookup"><span data-stu-id="c20c2-133">String</span></span>|<span data-ttu-id="c20c2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c20c2-134">Key of the entity.</span></span> <span data-ttu-id="c20c2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c20c2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c20c2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c20c2-137">DateTimeOffset</span></span>|<span data-ttu-id="c20c2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c20c2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c20c2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c20c2-140">roleScopeTagIds</span></span>|<span data-ttu-id="c20c2-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c20c2-141">String collection</span></span>|<span data-ttu-id="c20c2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c20c2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c20c2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c20c2-144">supportsScopeTags</span></span>|<span data-ttu-id="c20c2-145">Логический</span><span class="sxs-lookup"><span data-stu-id="c20c2-145">Boolean</span></span>|<span data-ttu-id="c20c2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c20c2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c20c2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c20c2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c20c2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c20c2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c20c2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c20c2-149">This property is read-only.</span></span> <span data-ttu-id="c20c2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c20c2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c20c2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c20c2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c20c2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c20c2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c20c2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c20c2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c20c2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c20c2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c20c2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c20c2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c20c2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c20c2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c20c2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c20c2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c20c2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c20c2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c20c2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c20c2-163">createdDateTime</span></span>|<span data-ttu-id="c20c2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c20c2-164">DateTimeOffset</span></span>|<span data-ttu-id="c20c2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c20c2-165">DateTime the object was created.</span></span> <span data-ttu-id="c20c2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-167">description</span><span class="sxs-lookup"><span data-stu-id="c20c2-167">description</span></span>|<span data-ttu-id="c20c2-168">String</span><span class="sxs-lookup"><span data-stu-id="c20c2-168">String</span></span>|<span data-ttu-id="c20c2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c20c2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c20c2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c20c2-171">displayName</span></span>|<span data-ttu-id="c20c2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c20c2-172">String</span></span>|<span data-ttu-id="c20c2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c20c2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c20c2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-175">version</span><span class="sxs-lookup"><span data-stu-id="c20c2-175">version</span></span>|<span data-ttu-id="c20c2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c20c2-176">Int32</span></span>|<span data-ttu-id="c20c2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c20c2-177">Version of the device configuration.</span></span> <span data-ttu-id="c20c2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c20c2-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c20c2-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="c20c2-180">Int32</span><span class="sxs-lookup"><span data-stu-id="c20c2-180">Int32</span></span>|<span data-ttu-id="c20c2-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c20c2-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c20c2-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c20c2-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c20c2-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c20c2-183">subjectNameFormat</span></span>|[<span data-ttu-id="c20c2-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c20c2-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c20c2-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c20c2-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="c20c2-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c20c2-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c20c2-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c20c2-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c20c2-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c20c2-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c20c2-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c20c2-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c20c2-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c20c2-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c20c2-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c20c2-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c20c2-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c20c2-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c20c2-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c20c2-194">Int32</span></span>|<span data-ttu-id="c20c2-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c20c2-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c20c2-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c20c2-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c20c2-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c20c2-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c20c2-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c20c2-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c20c2-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c20c2-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c20c2-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c20c2-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c20c2-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c20c2-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c20c2-202">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c20c2-202">extendedKeyUsages</span></span>|<span data-ttu-id="c20c2-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c20c2-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c20c2-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c20c2-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c20c2-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c20c2-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c20c2-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c20c2-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c20c2-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c20c2-207">intendedPurpose</span></span>|[<span data-ttu-id="c20c2-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c20c2-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c20c2-209">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="c20c2-209">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c20c2-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="c20c2-210">Response</span></span>
<span data-ttu-id="c20c2-211">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c20c2-211">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c20c2-212">Пример</span><span class="sxs-lookup"><span data-stu-id="c20c2-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="c20c2-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="c20c2-213">Request</span></span>
<span data-ttu-id="c20c2-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c20c2-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1492

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="c20c2-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="c20c2-215">Response</span></span>
<span data-ttu-id="c20c2-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c20c2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1664

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```






