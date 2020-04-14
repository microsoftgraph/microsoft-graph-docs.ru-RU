---
title: Создание Андроидимпортедпфксцертификатепрофиле
description: Создание нового объекта Андроидимпортедпфксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f67cea53fd5be5cc1c2400da83fad835eefac2b8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43344625"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="d471f-103">Создание Андроидимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="d471f-103">Create androidImportedPFXCertificateProfile</span></span>

<span data-ttu-id="d471f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d471f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d471f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d471f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d471f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d471f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d471f-107">Создание нового объекта [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d471f-107">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d471f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d471f-108">Prerequisites</span></span>
<span data-ttu-id="d471f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d471f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d471f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d471f-111">Permission type</span></span>|<span data-ttu-id="d471f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d471f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d471f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d471f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d471f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d471f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d471f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d471f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d471f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d471f-116">Not supported.</span></span>|
|<span data-ttu-id="d471f-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d471f-117">Application</span></span>|<span data-ttu-id="d471f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d471f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d471f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d471f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d471f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d471f-120">Request headers</span></span>
|<span data-ttu-id="d471f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d471f-121">Header</span></span>|<span data-ttu-id="d471f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d471f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d471f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d471f-123">Authorization</span></span>|<span data-ttu-id="d471f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d471f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d471f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d471f-125">Accept</span></span>|<span data-ttu-id="d471f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d471f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d471f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d471f-127">Request body</span></span>
<span data-ttu-id="d471f-128">В тексте запроса добавьте представление объекта Андроидимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d471f-128">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="d471f-129">В следующей таблице приведены свойства, необходимые при создании Андроидимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="d471f-129">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="d471f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d471f-130">Property</span></span>|<span data-ttu-id="d471f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d471f-131">Type</span></span>|<span data-ttu-id="d471f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d471f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d471f-133">id</span><span class="sxs-lookup"><span data-stu-id="d471f-133">id</span></span>|<span data-ttu-id="d471f-134">String</span><span class="sxs-lookup"><span data-stu-id="d471f-134">String</span></span>|<span data-ttu-id="d471f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d471f-135">Key of the entity.</span></span> <span data-ttu-id="d471f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d471f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d471f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d471f-138">DateTimeOffset</span></span>|<span data-ttu-id="d471f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d471f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d471f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d471f-141">roleScopeTagIds</span></span>|<span data-ttu-id="d471f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d471f-142">String collection</span></span>|<span data-ttu-id="d471f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d471f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d471f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d471f-145">supportsScopeTags</span></span>|<span data-ttu-id="d471f-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="d471f-146">Boolean</span></span>|<span data-ttu-id="d471f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d471f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d471f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d471f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d471f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d471f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d471f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d471f-150">This property is read-only.</span></span> <span data-ttu-id="d471f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d471f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d471f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d471f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d471f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d471f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d471f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d471f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d471f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d471f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d471f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d471f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d471f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d471f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d471f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d471f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d471f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d471f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d471f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d471f-164">createdDateTime</span></span>|<span data-ttu-id="d471f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d471f-165">DateTimeOffset</span></span>|<span data-ttu-id="d471f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d471f-166">DateTime the object was created.</span></span> <span data-ttu-id="d471f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-168">description</span><span class="sxs-lookup"><span data-stu-id="d471f-168">description</span></span>|<span data-ttu-id="d471f-169">String</span><span class="sxs-lookup"><span data-stu-id="d471f-169">String</span></span>|<span data-ttu-id="d471f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d471f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d471f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d471f-172">displayName</span></span>|<span data-ttu-id="d471f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d471f-173">String</span></span>|<span data-ttu-id="d471f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d471f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d471f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-176">version</span><span class="sxs-lookup"><span data-stu-id="d471f-176">version</span></span>|<span data-ttu-id="d471f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d471f-177">Int32</span></span>|<span data-ttu-id="d471f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d471f-178">Version of the device configuration.</span></span> <span data-ttu-id="d471f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471f-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="d471f-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="d471f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="d471f-181">Int32</span></span>|<span data-ttu-id="d471f-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="d471f-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="d471f-183">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d471f-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d471f-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d471f-184">subjectNameFormat</span></span>|[<span data-ttu-id="d471f-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="d471f-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="d471f-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d471f-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="d471f-187">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d471f-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="d471f-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="d471f-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d471f-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="d471f-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="d471f-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="d471f-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="d471f-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="d471f-192">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d471f-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="d471f-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="d471f-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="d471f-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="d471f-195">Int32</span><span class="sxs-lookup"><span data-stu-id="d471f-195">Int32</span></span>|<span data-ttu-id="d471f-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d471f-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="d471f-197">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d471f-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d471f-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d471f-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="d471f-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="d471f-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="d471f-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="d471f-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="d471f-201">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d471f-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="d471f-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="d471f-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="d471f-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="d471f-203">extendedKeyUsages</span></span>|<span data-ttu-id="d471f-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="d471f-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="d471f-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="d471f-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="d471f-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d471f-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d471f-207">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d471f-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="d471f-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d471f-208">intendedPurpose</span></span>|[<span data-ttu-id="d471f-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="d471f-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="d471f-210">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="d471f-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="d471f-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="d471f-211">Response</span></span>
<span data-ttu-id="d471f-212">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d471f-212">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d471f-213">Пример</span><span class="sxs-lookup"><span data-stu-id="d471f-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="d471f-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="d471f-214">Request</span></span>
<span data-ttu-id="d471f-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d471f-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d471f-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="d471f-216">Response</span></span>
<span data-ttu-id="d471f-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d471f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



