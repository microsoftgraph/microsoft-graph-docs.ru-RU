---
title: Создание macOSScepCertificateProfile
description: Создание нового объекта macOSScepCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38964b45ea970258c0ff64f91ae7c5e2608508f7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42745193"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="7bd00-103">Создание macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7bd00-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="7bd00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bd00-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bd00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bd00-106">Создание нового объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7bd00-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bd00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7bd00-107">Prerequisites</span></span>
<span data-ttu-id="7bd00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bd00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bd00-110">Permission type</span></span>|<span data-ttu-id="7bd00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bd00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bd00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bd00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7bd00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7bd00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bd00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bd00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd00-115">Not supported.</span></span>|
|<span data-ttu-id="7bd00-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7bd00-116">Application</span></span>|<span data-ttu-id="7bd00-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd00-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bd00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bd00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7bd00-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7bd00-119">Request headers</span></span>
|<span data-ttu-id="7bd00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bd00-120">Header</span></span>|<span data-ttu-id="7bd00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7bd00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bd00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd00-122">Authorization</span></span>|<span data-ttu-id="7bd00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bd00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bd00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7bd00-124">Accept</span></span>|<span data-ttu-id="7bd00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7bd00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd00-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bd00-126">Request body</span></span>
<span data-ttu-id="7bd00-127">В тексте запроса добавьте представление объекта macOSScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bd00-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="7bd00-128">В следующей таблице приведены свойства, необходимые при создании macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="7bd00-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="7bd00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bd00-129">Property</span></span>|<span data-ttu-id="7bd00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7bd00-130">Type</span></span>|<span data-ttu-id="7bd00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd00-132">id</span><span class="sxs-lookup"><span data-stu-id="7bd00-132">id</span></span>|<span data-ttu-id="7bd00-133">String</span><span class="sxs-lookup"><span data-stu-id="7bd00-133">String</span></span>|<span data-ttu-id="7bd00-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd00-134">Key of the entity.</span></span> <span data-ttu-id="7bd00-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd00-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7bd00-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd00-137">DateTimeOffset</span></span>|<span data-ttu-id="7bd00-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd00-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7bd00-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7bd00-140">roleScopeTagIds</span></span>|<span data-ttu-id="7bd00-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7bd00-141">String collection</span></span>|<span data-ttu-id="7bd00-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7bd00-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7bd00-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7bd00-144">supportsScopeTags</span></span>|<span data-ttu-id="7bd00-145">Логический</span><span class="sxs-lookup"><span data-stu-id="7bd00-145">Boolean</span></span>|<span data-ttu-id="7bd00-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7bd00-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7bd00-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7bd00-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7bd00-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7bd00-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7bd00-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bd00-149">This property is read-only.</span></span> <span data-ttu-id="7bd00-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7bd00-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7bd00-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7bd00-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7bd00-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7bd00-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7bd00-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7bd00-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7bd00-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7bd00-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7bd00-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7bd00-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7bd00-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7bd00-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7bd00-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7bd00-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7bd00-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7bd00-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7bd00-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd00-163">createdDateTime</span></span>|<span data-ttu-id="7bd00-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd00-164">DateTimeOffset</span></span>|<span data-ttu-id="7bd00-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd00-165">DateTime the object was created.</span></span> <span data-ttu-id="7bd00-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-167">description</span><span class="sxs-lookup"><span data-stu-id="7bd00-167">description</span></span>|<span data-ttu-id="7bd00-168">String</span><span class="sxs-lookup"><span data-stu-id="7bd00-168">String</span></span>|<span data-ttu-id="7bd00-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd00-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7bd00-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7bd00-171">displayName</span></span>|<span data-ttu-id="7bd00-172">Строка</span><span class="sxs-lookup"><span data-stu-id="7bd00-172">String</span></span>|<span data-ttu-id="7bd00-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd00-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7bd00-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-175">version</span><span class="sxs-lookup"><span data-stu-id="7bd00-175">version</span></span>|<span data-ttu-id="7bd00-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd00-176">Int32</span></span>|<span data-ttu-id="7bd00-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7bd00-177">Version of the device configuration.</span></span> <span data-ttu-id="7bd00-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7bd00-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="7bd00-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="7bd00-180">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd00-180">Int32</span></span>|<span data-ttu-id="7bd00-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd00-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7bd00-182">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7bd00-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7bd00-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7bd00-183">subjectNameFormat</span></span>|[<span data-ttu-id="7bd00-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="7bd00-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7bd00-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd00-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="7bd00-186">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd00-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7bd00-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7bd00-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7bd00-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7bd00-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7bd00-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd00-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7bd00-191">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd00-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7bd00-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7bd00-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7bd00-194">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd00-194">Int32</span></span>|<span data-ttu-id="7bd00-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd00-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7bd00-196">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7bd00-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7bd00-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7bd00-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7bd00-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7bd00-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7bd00-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7bd00-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7bd00-200">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7bd00-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="7bd00-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7bd00-202">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="7bd00-202">scepServerUrls</span></span>|<span data-ttu-id="7bd00-203">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7bd00-203">String collection</span></span>|<span data-ttu-id="7bd00-204">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd00-204">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="7bd00-205">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="7bd00-205">subjectNameFormatString</span></span>|<span data-ttu-id="7bd00-206">String</span><span class="sxs-lookup"><span data-stu-id="7bd00-206">String</span></span>|<span data-ttu-id="7bd00-207">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="7bd00-207">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7bd00-208">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="7bd00-208">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7bd00-209">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="7bd00-209">keyUsage</span></span>|[<span data-ttu-id="7bd00-210">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="7bd00-210">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7bd00-211">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd00-211">SCEP Key Usage.</span></span> <span data-ttu-id="7bd00-212">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-212">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7bd00-213">keySize</span><span class="sxs-lookup"><span data-stu-id="7bd00-213">keySize</span></span>|[<span data-ttu-id="7bd00-214">keySize</span><span class="sxs-lookup"><span data-stu-id="7bd00-214">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7bd00-215">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd00-215">SCEP Key Size.</span></span> <span data-ttu-id="7bd00-216">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-216">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7bd00-217">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="7bd00-217">hashAlgorithm</span></span>|[<span data-ttu-id="7bd00-218">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="7bd00-218">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="7bd00-219">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="7bd00-219">SCEP Hash Algorithm.</span></span> <span data-ttu-id="7bd00-220">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-220">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="7bd00-221">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="7bd00-221">extendedKeyUsages</span></span>|<span data-ttu-id="7bd00-222">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="7bd00-222">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7bd00-223">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="7bd00-223">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7bd00-224">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7bd00-224">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7bd00-225">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7bd00-225">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7bd00-226">String</span><span class="sxs-lookup"><span data-stu-id="7bd00-226">String</span></span>|<span data-ttu-id="7bd00-227">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="7bd00-227">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7bd00-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7bd00-228">certificateStore</span></span>|[<span data-ttu-id="7bd00-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7bd00-229">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7bd00-230">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="7bd00-230">Target store certificate.</span></span> <span data-ttu-id="7bd00-231">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="7bd00-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7bd00-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7bd00-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7bd00-233">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="7bd00-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7bd00-234">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="7bd00-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="7bd00-235">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7bd00-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7bd00-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd00-236">Response</span></span>
<span data-ttu-id="7bd00-237">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bd00-237">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bd00-238">Пример</span><span class="sxs-lookup"><span data-stu-id="7bd00-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bd00-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bd00-239">Request</span></span>
<span data-ttu-id="7bd00-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bd00-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1962

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="7bd00-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bd00-241">Response</span></span>
<span data-ttu-id="7bd00-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7bd00-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2134

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




