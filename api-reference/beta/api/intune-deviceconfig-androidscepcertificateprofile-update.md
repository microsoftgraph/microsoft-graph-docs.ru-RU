---
title: Обновление androidScepCertificateProfile
description: Обновление свойств объекта androidScepCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 808822b8dd60e611ca8e36c505545a8a15626e2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443645"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="27098-103">Обновление androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="27098-103">Update androidScepCertificateProfile</span></span>

<span data-ttu-id="27098-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="27098-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27098-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27098-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27098-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27098-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27098-107">Обновление свойств объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="27098-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27098-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="27098-108">Prerequisites</span></span>
<span data-ttu-id="27098-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27098-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27098-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27098-111">Permission type</span></span>|<span data-ttu-id="27098-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27098-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27098-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27098-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27098-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27098-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27098-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27098-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27098-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27098-116">Not supported.</span></span>|
|<span data-ttu-id="27098-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27098-117">Application</span></span>|<span data-ttu-id="27098-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27098-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27098-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27098-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="27098-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="27098-120">Request headers</span></span>
|<span data-ttu-id="27098-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27098-121">Header</span></span>|<span data-ttu-id="27098-122">Значение</span><span class="sxs-lookup"><span data-stu-id="27098-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27098-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27098-123">Authorization</span></span>|<span data-ttu-id="27098-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27098-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27098-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27098-125">Accept</span></span>|<span data-ttu-id="27098-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27098-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27098-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27098-127">Request body</span></span>
<span data-ttu-id="27098-128">В тексте запроса добавьте представление объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27098-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="27098-129">В следующей таблице приведены свойства, необходимые при создании [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="27098-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="27098-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="27098-130">Property</span></span>|<span data-ttu-id="27098-131">Тип</span><span class="sxs-lookup"><span data-stu-id="27098-131">Type</span></span>|<span data-ttu-id="27098-132">Описание</span><span class="sxs-lookup"><span data-stu-id="27098-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27098-133">id</span><span class="sxs-lookup"><span data-stu-id="27098-133">id</span></span>|<span data-ttu-id="27098-134">String</span><span class="sxs-lookup"><span data-stu-id="27098-134">String</span></span>|<span data-ttu-id="27098-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="27098-135">Key of the entity.</span></span> <span data-ttu-id="27098-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27098-137">lastModifiedDateTime</span></span>|<span data-ttu-id="27098-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27098-138">DateTimeOffset</span></span>|<span data-ttu-id="27098-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="27098-139">DateTime the object was last modified.</span></span> <span data-ttu-id="27098-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27098-141">roleScopeTagIds</span></span>|<span data-ttu-id="27098-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27098-142">String collection</span></span>|<span data-ttu-id="27098-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="27098-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="27098-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="27098-145">supportsScopeTags</span></span>|<span data-ttu-id="27098-146">Логический</span><span class="sxs-lookup"><span data-stu-id="27098-146">Boolean</span></span>|<span data-ttu-id="27098-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="27098-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="27098-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="27098-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="27098-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="27098-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="27098-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27098-150">This property is read-only.</span></span> <span data-ttu-id="27098-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27098-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="27098-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="27098-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="27098-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="27098-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="27098-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27098-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="27098-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="27098-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="27098-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="27098-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="27098-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27098-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="27098-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="27098-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="27098-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="27098-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="27098-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27098-164">createdDateTime</span></span>|<span data-ttu-id="27098-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27098-165">DateTimeOffset</span></span>|<span data-ttu-id="27098-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="27098-166">DateTime the object was created.</span></span> <span data-ttu-id="27098-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-168">description</span><span class="sxs-lookup"><span data-stu-id="27098-168">description</span></span>|<span data-ttu-id="27098-169">String</span><span class="sxs-lookup"><span data-stu-id="27098-169">String</span></span>|<span data-ttu-id="27098-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="27098-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="27098-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-172">displayName</span><span class="sxs-lookup"><span data-stu-id="27098-172">displayName</span></span>|<span data-ttu-id="27098-173">Строка</span><span class="sxs-lookup"><span data-stu-id="27098-173">String</span></span>|<span data-ttu-id="27098-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="27098-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="27098-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-176">version</span><span class="sxs-lookup"><span data-stu-id="27098-176">version</span></span>|<span data-ttu-id="27098-177">Int32</span><span class="sxs-lookup"><span data-stu-id="27098-177">Int32</span></span>|<span data-ttu-id="27098-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="27098-178">Version of the device configuration.</span></span> <span data-ttu-id="27098-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27098-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="27098-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="27098-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="27098-181">Int32</span><span class="sxs-lookup"><span data-stu-id="27098-181">Int32</span></span>|<span data-ttu-id="27098-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="27098-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="27098-183">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="27098-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="27098-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="27098-184">subjectNameFormat</span></span>|[<span data-ttu-id="27098-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="27098-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="27098-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="27098-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="27098-187">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="27098-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="27098-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="27098-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="27098-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="27098-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="27098-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="27098-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="27098-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="27098-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="27098-192">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="27098-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="27098-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="27098-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="27098-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="27098-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="27098-195">Int32</span><span class="sxs-lookup"><span data-stu-id="27098-195">Int32</span></span>|<span data-ttu-id="27098-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="27098-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="27098-197">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="27098-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="27098-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="27098-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="27098-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="27098-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="27098-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="27098-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="27098-201">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="27098-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="27098-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="27098-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="27098-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="27098-203">extendedKeyUsages</span></span>|<span data-ttu-id="27098-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="27098-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="27098-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="27098-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="27098-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="27098-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="27098-207">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="27098-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="27098-208">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="27098-208">scepServerUrls</span></span>|<span data-ttu-id="27098-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="27098-209">String collection</span></span>|<span data-ttu-id="27098-210">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="27098-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="27098-211">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="27098-211">subjectNameFormatString</span></span>|<span data-ttu-id="27098-212">String</span><span class="sxs-lookup"><span data-stu-id="27098-212">String</span></span>|<span data-ttu-id="27098-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="27098-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="27098-214">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="27098-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="27098-215">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="27098-215">keyUsage</span></span>|[<span data-ttu-id="27098-216">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="27098-216">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="27098-217">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="27098-217">SCEP Key Usage.</span></span> <span data-ttu-id="27098-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="27098-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="27098-219">keySize</span><span class="sxs-lookup"><span data-stu-id="27098-219">keySize</span></span>|[<span data-ttu-id="27098-220">keySize</span><span class="sxs-lookup"><span data-stu-id="27098-220">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="27098-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="27098-221">SCEP Key Size.</span></span> <span data-ttu-id="27098-222">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="27098-222">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="27098-223">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="27098-223">hashAlgorithm</span></span>|[<span data-ttu-id="27098-224">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="27098-224">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="27098-225">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="27098-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="27098-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="27098-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="27098-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="27098-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="27098-228">String</span><span class="sxs-lookup"><span data-stu-id="27098-228">String</span></span>|<span data-ttu-id="27098-229">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="27098-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="27098-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="27098-230">Response</span></span>
<span data-ttu-id="27098-231">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="27098-231">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27098-232">Пример</span><span class="sxs-lookup"><span data-stu-id="27098-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="27098-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="27098-233">Request</span></span>
<span data-ttu-id="27098-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27098-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="27098-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="27098-235">Response</span></span>
<span data-ttu-id="27098-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27098-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





