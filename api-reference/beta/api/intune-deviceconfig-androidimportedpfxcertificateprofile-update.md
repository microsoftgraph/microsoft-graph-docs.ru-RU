---
title: Обновление Андроидимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Андроидимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c13a5d5e9b0437b0c022c31437204971ba9e1358
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970116"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="0d305-103">Обновление Андроидимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="0d305-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="0d305-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d305-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d305-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d305-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d305-106">Обновление свойств объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0d305-106">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d305-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0d305-107">Prerequisites</span></span>
<span data-ttu-id="0d305-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d305-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d305-110">Permission type</span></span>|<span data-ttu-id="0d305-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d305-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d305-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d305-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d305-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d305-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0d305-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d305-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d305-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d305-115">Not supported.</span></span>|
|<span data-ttu-id="0d305-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d305-116">Application</span></span>|<span data-ttu-id="0d305-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d305-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d305-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d305-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0d305-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d305-119">Request headers</span></span>
|<span data-ttu-id="0d305-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d305-120">Header</span></span>|<span data-ttu-id="0d305-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d305-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d305-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d305-122">Authorization</span></span>|<span data-ttu-id="0d305-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d305-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d305-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d305-124">Accept</span></span>|<span data-ttu-id="0d305-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d305-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d305-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d305-126">Request body</span></span>
<span data-ttu-id="0d305-127">В тексте запроса добавьте представление объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d305-127">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="0d305-128">В следующей таблице приведены свойства, необходимые при создании [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-128">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="0d305-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d305-129">Property</span></span>|<span data-ttu-id="0d305-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d305-130">Type</span></span>|<span data-ttu-id="0d305-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d305-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d305-132">id</span><span class="sxs-lookup"><span data-stu-id="0d305-132">id</span></span>|<span data-ttu-id="0d305-133">String</span><span class="sxs-lookup"><span data-stu-id="0d305-133">String</span></span>|<span data-ttu-id="0d305-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d305-134">Key of the entity.</span></span> <span data-ttu-id="0d305-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d305-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0d305-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d305-137">DateTimeOffset</span></span>|<span data-ttu-id="0d305-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d305-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0d305-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d305-140">roleScopeTagIds</span></span>|<span data-ttu-id="0d305-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d305-141">String collection</span></span>|<span data-ttu-id="0d305-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0d305-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0d305-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0d305-144">supportsScopeTags</span></span>|<span data-ttu-id="0d305-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d305-145">Boolean</span></span>|<span data-ttu-id="0d305-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0d305-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0d305-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0d305-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0d305-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0d305-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0d305-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0d305-149">This property is read-only.</span></span> <span data-ttu-id="0d305-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0d305-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0d305-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0d305-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0d305-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0d305-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0d305-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0d305-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0d305-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0d305-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0d305-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0d305-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0d305-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="0d305-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0d305-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="0d305-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0d305-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0d305-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0d305-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d305-163">createdDateTime</span></span>|<span data-ttu-id="0d305-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d305-164">DateTimeOffset</span></span>|<span data-ttu-id="0d305-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0d305-165">DateTime the object was created.</span></span> <span data-ttu-id="0d305-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-167">description</span><span class="sxs-lookup"><span data-stu-id="0d305-167">description</span></span>|<span data-ttu-id="0d305-168">String</span><span class="sxs-lookup"><span data-stu-id="0d305-168">String</span></span>|<span data-ttu-id="0d305-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d305-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d305-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0d305-171">displayName</span></span>|<span data-ttu-id="0d305-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0d305-172">String</span></span>|<span data-ttu-id="0d305-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d305-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d305-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-175">version</span><span class="sxs-lookup"><span data-stu-id="0d305-175">version</span></span>|<span data-ttu-id="0d305-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0d305-176">Int32</span></span>|<span data-ttu-id="0d305-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d305-177">Version of the device configuration.</span></span> <span data-ttu-id="0d305-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0d305-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="0d305-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="0d305-180">Int32</span><span class="sxs-lookup"><span data-stu-id="0d305-180">Int32</span></span>|<span data-ttu-id="0d305-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="0d305-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="0d305-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d305-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0d305-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0d305-183">subjectNameFormat</span></span>|[<span data-ttu-id="0d305-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="0d305-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="0d305-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0d305-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="0d305-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="0d305-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="0d305-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="0d305-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0d305-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="0d305-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="0d305-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="0d305-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="0d305-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="0d305-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="0d305-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="0d305-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="0d305-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="0d305-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="0d305-194">Int32</span><span class="sxs-lookup"><span data-stu-id="0d305-194">Int32</span></span>|<span data-ttu-id="0d305-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0d305-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="0d305-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d305-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0d305-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0d305-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="0d305-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="0d305-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="0d305-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="0d305-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="0d305-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0d305-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="0d305-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="0d305-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="0d305-202">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="0d305-202">extendedKeyUsages</span></span>|<span data-ttu-id="0d305-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="0d305-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="0d305-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="0d305-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="0d305-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0d305-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="0d305-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0d305-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="0d305-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0d305-207">intendedPurpose</span></span>|[<span data-ttu-id="0d305-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="0d305-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="0d305-209">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="0d305-209">Not yet documented.</span></span> <span data-ttu-id="0d305-210">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="0d305-210">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="0d305-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d305-211">Response</span></span>
<span data-ttu-id="0d305-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0d305-212">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d305-213">Пример</span><span class="sxs-lookup"><span data-stu-id="0d305-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d305-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d305-214">Request</span></span>
<span data-ttu-id="0d305-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d305-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d305-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d305-216">Response</span></span>
<span data-ttu-id="0d305-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d305-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





