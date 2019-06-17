---
title: Обновление Макосимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Макосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 243cd55427b717db7e9258455e81a0c590626f96
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963172"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="d40dd-103">Обновление Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="d40dd-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="d40dd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d40dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d40dd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d40dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d40dd-106">Обновление свойств объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d40dd-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d40dd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d40dd-107">Prerequisites</span></span>
<span data-ttu-id="d40dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d40dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d40dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d40dd-110">Permission type</span></span>|<span data-ttu-id="d40dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d40dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d40dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d40dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d40dd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d40dd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d40dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d40dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d40dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d40dd-115">Not supported.</span></span>|
|<span data-ttu-id="d40dd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d40dd-116">Application</span></span>|<span data-ttu-id="d40dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d40dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d40dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d40dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d40dd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d40dd-119">Request headers</span></span>
|<span data-ttu-id="d40dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d40dd-120">Header</span></span>|<span data-ttu-id="d40dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d40dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d40dd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d40dd-122">Authorization</span></span>|<span data-ttu-id="d40dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d40dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d40dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d40dd-124">Accept</span></span>|<span data-ttu-id="d40dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d40dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d40dd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d40dd-126">Request body</span></span>
<span data-ttu-id="d40dd-127">В тексте запроса добавьте представление объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d40dd-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="d40dd-128">В следующей таблице приведены свойства, необходимые при создании [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="d40dd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d40dd-129">Property</span></span>|<span data-ttu-id="d40dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d40dd-130">Type</span></span>|<span data-ttu-id="d40dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d40dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d40dd-132">id</span><span class="sxs-lookup"><span data-stu-id="d40dd-132">id</span></span>|<span data-ttu-id="d40dd-133">String</span><span class="sxs-lookup"><span data-stu-id="d40dd-133">String</span></span>|<span data-ttu-id="d40dd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d40dd-134">Key of the entity.</span></span> <span data-ttu-id="d40dd-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d40dd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d40dd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d40dd-137">DateTimeOffset</span></span>|<span data-ttu-id="d40dd-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d40dd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d40dd-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d40dd-140">roleScopeTagIds</span></span>|<span data-ttu-id="d40dd-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d40dd-141">String collection</span></span>|<span data-ttu-id="d40dd-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d40dd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d40dd-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d40dd-144">supportsScopeTags</span></span>|<span data-ttu-id="d40dd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d40dd-145">Boolean</span></span>|<span data-ttu-id="d40dd-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d40dd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d40dd-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d40dd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d40dd-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d40dd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d40dd-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d40dd-149">This property is read-only.</span></span> <span data-ttu-id="d40dd-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d40dd-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d40dd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d40dd-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d40dd-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d40dd-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d40dd-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d40dd-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d40dd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d40dd-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d40dd-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d40dd-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d40dd-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d40dd-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d40dd-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d40dd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d40dd-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d40dd-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d40dd-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d40dd-163">createdDateTime</span></span>|<span data-ttu-id="d40dd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d40dd-164">DateTimeOffset</span></span>|<span data-ttu-id="d40dd-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d40dd-165">DateTime the object was created.</span></span> <span data-ttu-id="d40dd-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-167">description</span><span class="sxs-lookup"><span data-stu-id="d40dd-167">description</span></span>|<span data-ttu-id="d40dd-168">String</span><span class="sxs-lookup"><span data-stu-id="d40dd-168">String</span></span>|<span data-ttu-id="d40dd-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d40dd-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d40dd-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d40dd-171">displayName</span></span>|<span data-ttu-id="d40dd-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d40dd-172">String</span></span>|<span data-ttu-id="d40dd-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d40dd-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d40dd-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-175">version</span><span class="sxs-lookup"><span data-stu-id="d40dd-175">version</span></span>|<span data-ttu-id="d40dd-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d40dd-176">Int32</span></span>|<span data-ttu-id="d40dd-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d40dd-177">Version of the device configuration.</span></span> <span data-ttu-id="d40dd-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d40dd-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="d40dd-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="d40dd-180">Int32</span><span class="sxs-lookup"><span data-stu-id="d40dd-180">Int32</span></span>|<span data-ttu-id="d40dd-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="d40dd-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d40dd-182">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d40dd-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d40dd-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d40dd-183">subjectNameFormat</span></span>|[<span data-ttu-id="d40dd-184">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="d40dd-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="d40dd-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d40dd-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="d40dd-186">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d40dd-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="d40dd-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="d40dd-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d40dd-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d40dd-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d40dd-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d40dd-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d40dd-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d40dd-191">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d40dd-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d40dd-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d40dd-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d40dd-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d40dd-194">Int32</span><span class="sxs-lookup"><span data-stu-id="d40dd-194">Int32</span></span>|<span data-ttu-id="d40dd-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d40dd-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d40dd-196">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d40dd-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d40dd-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d40dd-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d40dd-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d40dd-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d40dd-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d40dd-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d40dd-200">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d40dd-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="d40dd-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d40dd-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d40dd-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d40dd-202">intendedPurpose</span></span>|[<span data-ttu-id="d40dd-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d40dd-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d40dd-204">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d40dd-204">Not yet documented.</span></span> <span data-ttu-id="d40dd-205">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="d40dd-205">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d40dd-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="d40dd-206">Response</span></span>
<span data-ttu-id="d40dd-207">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d40dd-207">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d40dd-208">Пример</span><span class="sxs-lookup"><span data-stu-id="d40dd-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="d40dd-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="d40dd-209">Request</span></span>
<span data-ttu-id="d40dd-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d40dd-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1297

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="d40dd-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="d40dd-211">Response</span></span>
<span data-ttu-id="d40dd-p119">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d40dd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "intendedPurpose": "smimeEncryption"
}
```





