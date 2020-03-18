---
title: Создание Андроидимпортедпфксцертификатепрофиле
description: Создание нового объекта Андроидимпортедпфксцертификатепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9dd407edac0f3752a8f49fa2612bf1114f93a30
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758982"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="86386-103">Создание Андроидимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="86386-103">Create androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="86386-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86386-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86386-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86386-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86386-106">Создание нового объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="86386-106">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86386-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86386-107">Prerequisites</span></span>
<span data-ttu-id="86386-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86386-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86386-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86386-110">Permission type</span></span>|<span data-ttu-id="86386-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86386-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86386-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86386-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86386-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86386-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86386-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86386-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86386-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86386-115">Not supported.</span></span>|
|<span data-ttu-id="86386-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="86386-116">Application</span></span>|<span data-ttu-id="86386-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86386-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86386-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86386-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86386-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86386-119">Request headers</span></span>
|<span data-ttu-id="86386-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86386-120">Header</span></span>|<span data-ttu-id="86386-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86386-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86386-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86386-122">Authorization</span></span>|<span data-ttu-id="86386-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86386-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86386-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86386-124">Accept</span></span>|<span data-ttu-id="86386-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86386-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86386-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86386-126">Request body</span></span>
<span data-ttu-id="86386-127">В тексте запроса добавьте представление объекта Андроидимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86386-127">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="86386-128">В следующей таблице приведены свойства, необходимые при создании Андроидимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="86386-128">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="86386-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="86386-129">Property</span></span>|<span data-ttu-id="86386-130">Тип</span><span class="sxs-lookup"><span data-stu-id="86386-130">Type</span></span>|<span data-ttu-id="86386-131">Описание</span><span class="sxs-lookup"><span data-stu-id="86386-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86386-132">id</span><span class="sxs-lookup"><span data-stu-id="86386-132">id</span></span>|<span data-ttu-id="86386-133">String</span><span class="sxs-lookup"><span data-stu-id="86386-133">String</span></span>|<span data-ttu-id="86386-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86386-134">Key of the entity.</span></span> <span data-ttu-id="86386-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86386-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86386-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86386-137">DateTimeOffset</span></span>|<span data-ttu-id="86386-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="86386-138">DateTime the object was last modified.</span></span> <span data-ttu-id="86386-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86386-140">roleScopeTagIds</span></span>|<span data-ttu-id="86386-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86386-141">String collection</span></span>|<span data-ttu-id="86386-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="86386-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86386-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="86386-144">supportsScopeTags</span></span>|<span data-ttu-id="86386-145">Логический</span><span class="sxs-lookup"><span data-stu-id="86386-145">Boolean</span></span>|<span data-ttu-id="86386-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="86386-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86386-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="86386-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86386-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="86386-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86386-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86386-149">This property is read-only.</span></span> <span data-ttu-id="86386-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86386-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86386-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86386-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86386-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86386-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86386-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86386-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86386-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86386-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86386-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86386-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86386-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86386-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86386-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86386-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86386-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86386-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86386-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86386-163">createdDateTime</span></span>|<span data-ttu-id="86386-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86386-164">DateTimeOffset</span></span>|<span data-ttu-id="86386-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="86386-165">DateTime the object was created.</span></span> <span data-ttu-id="86386-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-167">description</span><span class="sxs-lookup"><span data-stu-id="86386-167">description</span></span>|<span data-ttu-id="86386-168">String</span><span class="sxs-lookup"><span data-stu-id="86386-168">String</span></span>|<span data-ttu-id="86386-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86386-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86386-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-171">displayName</span><span class="sxs-lookup"><span data-stu-id="86386-171">displayName</span></span>|<span data-ttu-id="86386-172">Строка</span><span class="sxs-lookup"><span data-stu-id="86386-172">String</span></span>|<span data-ttu-id="86386-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86386-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86386-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-175">version</span><span class="sxs-lookup"><span data-stu-id="86386-175">version</span></span>|<span data-ttu-id="86386-176">Int32</span><span class="sxs-lookup"><span data-stu-id="86386-176">Int32</span></span>|<span data-ttu-id="86386-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86386-177">Version of the device configuration.</span></span> <span data-ttu-id="86386-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86386-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86386-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="86386-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="86386-180">Int32</span><span class="sxs-lookup"><span data-stu-id="86386-180">Int32</span></span>|<span data-ttu-id="86386-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="86386-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="86386-182">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86386-182">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86386-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86386-183">subjectNameFormat</span></span>|[<span data-ttu-id="86386-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="86386-184">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="86386-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="86386-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="86386-186">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86386-186">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="86386-187">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="86386-187">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="86386-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86386-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="86386-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="86386-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="86386-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="86386-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="86386-191">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86386-191">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="86386-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="86386-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="86386-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="86386-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="86386-194">Int32</span><span class="sxs-lookup"><span data-stu-id="86386-194">Int32</span></span>|<span data-ttu-id="86386-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="86386-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="86386-196">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86386-196">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86386-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86386-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="86386-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="86386-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="86386-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="86386-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="86386-200">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="86386-200">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="86386-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="86386-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="86386-202">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="86386-202">extendedKeyUsages</span></span>|<span data-ttu-id="86386-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="86386-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="86386-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="86386-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="86386-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="86386-205">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="86386-206">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="86386-206">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="86386-207">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="86386-207">intendedPurpose</span></span>|[<span data-ttu-id="86386-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="86386-208">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="86386-209">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="86386-209">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="86386-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="86386-210">Response</span></span>
<span data-ttu-id="86386-211">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86386-211">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86386-212">Пример</span><span class="sxs-lookup"><span data-stu-id="86386-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="86386-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="86386-213">Request</span></span>
<span data-ttu-id="86386-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86386-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="86386-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="86386-215">Response</span></span>
<span data-ttu-id="86386-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86386-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




