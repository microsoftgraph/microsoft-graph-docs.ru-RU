---
title: Обновление Андроидфорворкимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Андроидфорворкимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 61182880b291c7060cc3d69a8c774d9e8f998489
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963425"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="889b3-103">Обновление Андроидфорворкимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="889b3-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="889b3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="889b3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="889b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="889b3-106">Обновление свойств объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="889b3-106">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="889b3-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="889b3-107">Prerequisites</span></span>
<span data-ttu-id="889b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="889b3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="889b3-110">Permission type</span></span>|<span data-ttu-id="889b3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="889b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="889b3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="889b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="889b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="889b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="889b3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="889b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="889b3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889b3-115">Not supported.</span></span>|
|<span data-ttu-id="889b3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="889b3-116">Application</span></span>|<span data-ttu-id="889b3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="889b3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="889b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="889b3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="889b3-119">Request headers</span></span>
|<span data-ttu-id="889b3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="889b3-120">Header</span></span>|<span data-ttu-id="889b3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="889b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="889b3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="889b3-122">Authorization</span></span>|<span data-ttu-id="889b3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="889b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="889b3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="889b3-124">Accept</span></span>|<span data-ttu-id="889b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="889b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="889b3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="889b3-126">Request body</span></span>
<span data-ttu-id="889b3-127">В тексте запроса добавьте представление объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="889b3-127">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="889b3-128">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-128">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="889b3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="889b3-129">Property</span></span>|<span data-ttu-id="889b3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="889b3-130">Type</span></span>|<span data-ttu-id="889b3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="889b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="889b3-132">id</span><span class="sxs-lookup"><span data-stu-id="889b3-132">id</span></span>|<span data-ttu-id="889b3-133">String</span><span class="sxs-lookup"><span data-stu-id="889b3-133">String</span></span>|<span data-ttu-id="889b3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="889b3-134">Key of the entity.</span></span> <span data-ttu-id="889b3-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="889b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="889b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="889b3-137">DateTimeOffset</span></span>|<span data-ttu-id="889b3-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="889b3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="889b3-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="889b3-140">roleScopeTagIds</span></span>|<span data-ttu-id="889b3-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="889b3-141">String collection</span></span>|<span data-ttu-id="889b3-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="889b3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="889b3-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="889b3-144">supportsScopeTags</span></span>|<span data-ttu-id="889b3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="889b3-145">Boolean</span></span>|<span data-ttu-id="889b3-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="889b3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="889b3-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="889b3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="889b3-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="889b3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="889b3-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="889b3-149">This property is read-only.</span></span> <span data-ttu-id="889b3-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="889b3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="889b3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="889b3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="889b3-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="889b3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="889b3-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="889b3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="889b3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="889b3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="889b3-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="889b3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="889b3-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="889b3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="889b3-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="889b3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="889b3-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="889b3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="889b3-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="889b3-163">createdDateTime</span></span>|<span data-ttu-id="889b3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="889b3-164">DateTimeOffset</span></span>|<span data-ttu-id="889b3-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="889b3-165">DateTime the object was created.</span></span> <span data-ttu-id="889b3-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-167">description</span><span class="sxs-lookup"><span data-stu-id="889b3-167">description</span></span>|<span data-ttu-id="889b3-168">String</span><span class="sxs-lookup"><span data-stu-id="889b3-168">String</span></span>|<span data-ttu-id="889b3-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="889b3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="889b3-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="889b3-171">displayName</span></span>|<span data-ttu-id="889b3-172">Строка</span><span class="sxs-lookup"><span data-stu-id="889b3-172">String</span></span>|<span data-ttu-id="889b3-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="889b3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="889b3-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-175">version</span><span class="sxs-lookup"><span data-stu-id="889b3-175">version</span></span>|<span data-ttu-id="889b3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="889b3-176">Int32</span></span>|<span data-ttu-id="889b3-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="889b3-177">Version of the device configuration.</span></span> <span data-ttu-id="889b3-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="889b3-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="889b3-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="889b3-180">Int32</span><span class="sxs-lookup"><span data-stu-id="889b3-180">Int32</span></span>|<span data-ttu-id="889b3-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="889b3-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="889b3-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="889b3-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="889b3-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="889b3-183">subjectNameFormat</span></span>|[<span data-ttu-id="889b3-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="889b3-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="889b3-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="889b3-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="889b3-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="889b3-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="889b3-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="889b3-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="889b3-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="889b3-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="889b3-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="889b3-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="889b3-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="889b3-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="889b3-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="889b3-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="889b3-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="889b3-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="889b3-194">Int32</span><span class="sxs-lookup"><span data-stu-id="889b3-194">Int32</span></span>|<span data-ttu-id="889b3-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="889b3-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="889b3-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="889b3-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="889b3-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="889b3-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="889b3-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="889b3-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="889b3-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="889b3-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="889b3-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="889b3-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="889b3-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="889b3-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="889b3-202">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="889b3-202">extendedKeyUsages</span></span>|<span data-ttu-id="889b3-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="889b3-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="889b3-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="889b3-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="889b3-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="889b3-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="889b3-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="889b3-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="889b3-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="889b3-207">intendedPurpose</span></span>|[<span data-ttu-id="889b3-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="889b3-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="889b3-209">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="889b3-209">Not yet documented.</span></span> <span data-ttu-id="889b3-210">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="889b3-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="889b3-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="889b3-211">Response</span></span>
<span data-ttu-id="889b3-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="889b3-212">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="889b3-213">Пример</span><span class="sxs-lookup"><span data-stu-id="889b3-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="889b3-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="889b3-214">Request</span></span>
<span data-ttu-id="889b3-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="889b3-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1499

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="889b3-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="889b3-216">Response</span></span>
<span data-ttu-id="889b3-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="889b3-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1671

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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





