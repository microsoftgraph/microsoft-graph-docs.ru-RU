---
title: Обновление Андроидфорворкимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Андроидфорворкимпортедпфксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 203a8add84bce7e43528387e9bcea7fb7e0da1d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005539"
---
# <a name="update-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="68828-103">Обновление Андроидфорворкимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="68828-103">Update androidForWorkImportedPFXCertificateProfile</span></span>

<span data-ttu-id="68828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68828-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68828-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68828-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68828-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68828-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68828-107">Обновление свойств объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="68828-107">Update the properties of a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68828-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68828-108">Prerequisites</span></span>
<span data-ttu-id="68828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68828-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68828-111">Permission type</span></span>|<span data-ttu-id="68828-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68828-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68828-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68828-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68828-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68828-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68828-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68828-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68828-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68828-116">Not supported.</span></span>|
|<span data-ttu-id="68828-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="68828-117">Application</span></span>|<span data-ttu-id="68828-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68828-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68828-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68828-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="68828-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68828-120">Request headers</span></span>
|<span data-ttu-id="68828-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68828-121">Header</span></span>|<span data-ttu-id="68828-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68828-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68828-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68828-123">Authorization</span></span>|<span data-ttu-id="68828-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68828-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68828-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68828-125">Accept</span></span>|<span data-ttu-id="68828-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68828-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68828-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68828-127">Request body</span></span>
<span data-ttu-id="68828-128">В тексте запроса добавьте представление объекта [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68828-128">In the request body, supply a JSON representation for the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="68828-129">В следующей таблице приведены свойства, необходимые при создании [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="68828-129">The following table shows the properties that are required when you create the [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="68828-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68828-130">Property</span></span>|<span data-ttu-id="68828-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68828-131">Type</span></span>|<span data-ttu-id="68828-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68828-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68828-133">id</span><span class="sxs-lookup"><span data-stu-id="68828-133">id</span></span>|<span data-ttu-id="68828-134">String</span><span class="sxs-lookup"><span data-stu-id="68828-134">String</span></span>|<span data-ttu-id="68828-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="68828-135">Key of the entity.</span></span> <span data-ttu-id="68828-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68828-137">lastModifiedDateTime</span></span>|<span data-ttu-id="68828-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68828-138">DateTimeOffset</span></span>|<span data-ttu-id="68828-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="68828-139">DateTime the object was last modified.</span></span> <span data-ttu-id="68828-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="68828-141">roleScopeTagIds</span></span>|<span data-ttu-id="68828-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68828-142">String collection</span></span>|<span data-ttu-id="68828-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="68828-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="68828-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="68828-145">supportsScopeTags</span></span>|<span data-ttu-id="68828-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="68828-146">Boolean</span></span>|<span data-ttu-id="68828-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="68828-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="68828-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="68828-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="68828-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="68828-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="68828-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68828-150">This property is read-only.</span></span> <span data-ttu-id="68828-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="68828-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="68828-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="68828-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="68828-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="68828-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="68828-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="68828-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="68828-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="68828-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="68828-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="68828-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="68828-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="68828-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="68828-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="68828-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="68828-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="68828-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="68828-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68828-164">createdDateTime</span></span>|<span data-ttu-id="68828-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68828-165">DateTimeOffset</span></span>|<span data-ttu-id="68828-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="68828-166">DateTime the object was created.</span></span> <span data-ttu-id="68828-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-168">description</span><span class="sxs-lookup"><span data-stu-id="68828-168">description</span></span>|<span data-ttu-id="68828-169">String</span><span class="sxs-lookup"><span data-stu-id="68828-169">String</span></span>|<span data-ttu-id="68828-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68828-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="68828-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-172">displayName</span><span class="sxs-lookup"><span data-stu-id="68828-172">displayName</span></span>|<span data-ttu-id="68828-173">String</span><span class="sxs-lookup"><span data-stu-id="68828-173">String</span></span>|<span data-ttu-id="68828-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68828-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="68828-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-176">version</span><span class="sxs-lookup"><span data-stu-id="68828-176">version</span></span>|<span data-ttu-id="68828-177">Int32</span><span class="sxs-lookup"><span data-stu-id="68828-177">Int32</span></span>|<span data-ttu-id="68828-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="68828-178">Version of the device configuration.</span></span> <span data-ttu-id="68828-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="68828-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="68828-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="68828-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="68828-181">Int32</span><span class="sxs-lookup"><span data-stu-id="68828-181">Int32</span></span>|<span data-ttu-id="68828-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="68828-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="68828-183">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="68828-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="68828-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="68828-184">subjectNameFormat</span></span>|[<span data-ttu-id="68828-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="68828-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="68828-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="68828-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="68828-187">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="68828-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="68828-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="68828-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="68828-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="68828-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="68828-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="68828-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="68828-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="68828-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="68828-192">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="68828-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="68828-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="68828-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="68828-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="68828-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="68828-195">Int32</span><span class="sxs-lookup"><span data-stu-id="68828-195">Int32</span></span>|<span data-ttu-id="68828-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="68828-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="68828-197">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="68828-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="68828-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="68828-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="68828-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="68828-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="68828-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="68828-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="68828-201">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="68828-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="68828-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="68828-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="68828-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="68828-203">extendedKeyUsages</span></span>|<span data-ttu-id="68828-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="68828-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="68828-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="68828-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="68828-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="68828-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="68828-207">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="68828-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="68828-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="68828-208">intendedPurpose</span></span>|[<span data-ttu-id="68828-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="68828-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="68828-210">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned` ,, `smimeEncryption` `smimeSigning` , `vpn` , `wifi` .</span><span class="sxs-lookup"><span data-stu-id="68828-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="68828-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="68828-211">Response</span></span>
<span data-ttu-id="68828-212">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидфорворкимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68828-212">If successful, this method returns a `200 OK` response code and an updated [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68828-213">Пример</span><span class="sxs-lookup"><span data-stu-id="68828-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="68828-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="68828-214">Request</span></span>
<span data-ttu-id="68828-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68828-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68828-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="68828-216">Response</span></span>
<span data-ttu-id="68828-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68828-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






