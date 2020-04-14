---
title: Создание Макосимпортедпфксцертификатепрофиле
description: Создание нового объекта Макосимпортедпфксцертификатепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3bfddce25e368c7b5f7c28330447c48348487b8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432586"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="28f56-103">Создание Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="28f56-103">Create macOSImportedPFXCertificateProfile</span></span>

<span data-ttu-id="28f56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28f56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28f56-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28f56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28f56-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28f56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28f56-107">Создание нового объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="28f56-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28f56-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="28f56-108">Prerequisites</span></span>
<span data-ttu-id="28f56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28f56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28f56-111">Permission type</span></span>|<span data-ttu-id="28f56-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28f56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28f56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28f56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28f56-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28f56-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28f56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28f56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28f56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28f56-116">Not supported.</span></span>|
|<span data-ttu-id="28f56-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="28f56-117">Application</span></span>|<span data-ttu-id="28f56-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28f56-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="28f56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28f56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="28f56-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="28f56-120">Request headers</span></span>
|<span data-ttu-id="28f56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28f56-121">Header</span></span>|<span data-ttu-id="28f56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28f56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28f56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28f56-123">Authorization</span></span>|<span data-ttu-id="28f56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28f56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28f56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28f56-125">Accept</span></span>|<span data-ttu-id="28f56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28f56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28f56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28f56-127">Request body</span></span>
<span data-ttu-id="28f56-128">В тексте запроса добавьте представление объекта Макосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28f56-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="28f56-129">В следующей таблице приведены свойства, необходимые при создании Макосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="28f56-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="28f56-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="28f56-130">Property</span></span>|<span data-ttu-id="28f56-131">Тип</span><span class="sxs-lookup"><span data-stu-id="28f56-131">Type</span></span>|<span data-ttu-id="28f56-132">Описание</span><span class="sxs-lookup"><span data-stu-id="28f56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28f56-133">id</span><span class="sxs-lookup"><span data-stu-id="28f56-133">id</span></span>|<span data-ttu-id="28f56-134">String</span><span class="sxs-lookup"><span data-stu-id="28f56-134">String</span></span>|<span data-ttu-id="28f56-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="28f56-135">Key of the entity.</span></span> <span data-ttu-id="28f56-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28f56-137">lastModifiedDateTime</span></span>|<span data-ttu-id="28f56-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28f56-138">DateTimeOffset</span></span>|<span data-ttu-id="28f56-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="28f56-139">DateTime the object was last modified.</span></span> <span data-ttu-id="28f56-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="28f56-141">roleScopeTagIds</span></span>|<span data-ttu-id="28f56-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28f56-142">String collection</span></span>|<span data-ttu-id="28f56-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="28f56-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28f56-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="28f56-145">supportsScopeTags</span></span>|<span data-ttu-id="28f56-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="28f56-146">Boolean</span></span>|<span data-ttu-id="28f56-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="28f56-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="28f56-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="28f56-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="28f56-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="28f56-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="28f56-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="28f56-150">This property is read-only.</span></span> <span data-ttu-id="28f56-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="28f56-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="28f56-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="28f56-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="28f56-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="28f56-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="28f56-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="28f56-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="28f56-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="28f56-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="28f56-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="28f56-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="28f56-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="28f56-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="28f56-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="28f56-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="28f56-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="28f56-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="28f56-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28f56-164">createdDateTime</span></span>|<span data-ttu-id="28f56-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28f56-165">DateTimeOffset</span></span>|<span data-ttu-id="28f56-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="28f56-166">DateTime the object was created.</span></span> <span data-ttu-id="28f56-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-168">description</span><span class="sxs-lookup"><span data-stu-id="28f56-168">description</span></span>|<span data-ttu-id="28f56-169">String</span><span class="sxs-lookup"><span data-stu-id="28f56-169">String</span></span>|<span data-ttu-id="28f56-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28f56-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28f56-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-172">displayName</span><span class="sxs-lookup"><span data-stu-id="28f56-172">displayName</span></span>|<span data-ttu-id="28f56-173">Строка</span><span class="sxs-lookup"><span data-stu-id="28f56-173">String</span></span>|<span data-ttu-id="28f56-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28f56-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28f56-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-176">version</span><span class="sxs-lookup"><span data-stu-id="28f56-176">version</span></span>|<span data-ttu-id="28f56-177">Int32</span><span class="sxs-lookup"><span data-stu-id="28f56-177">Int32</span></span>|<span data-ttu-id="28f56-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="28f56-178">Version of the device configuration.</span></span> <span data-ttu-id="28f56-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28f56-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="28f56-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="28f56-181">Int32</span><span class="sxs-lookup"><span data-stu-id="28f56-181">Int32</span></span>|<span data-ttu-id="28f56-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="28f56-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="28f56-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="28f56-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="28f56-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="28f56-184">subjectNameFormat</span></span>|[<span data-ttu-id="28f56-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="28f56-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="28f56-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="28f56-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="28f56-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="28f56-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="28f56-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="28f56-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="28f56-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="28f56-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="28f56-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="28f56-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="28f56-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="28f56-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="28f56-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="28f56-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="28f56-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="28f56-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="28f56-195">Int32</span><span class="sxs-lookup"><span data-stu-id="28f56-195">Int32</span></span>|<span data-ttu-id="28f56-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="28f56-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="28f56-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="28f56-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="28f56-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="28f56-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="28f56-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="28f56-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="28f56-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="28f56-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="28f56-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="28f56-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="28f56-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="28f56-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="28f56-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="28f56-203">intendedPurpose</span></span>|[<span data-ttu-id="28f56-204">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="28f56-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="28f56-205">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="28f56-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="28f56-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="28f56-206">Response</span></span>
<span data-ttu-id="28f56-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28f56-207">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28f56-208">Пример</span><span class="sxs-lookup"><span data-stu-id="28f56-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="28f56-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="28f56-209">Request</span></span>
<span data-ttu-id="28f56-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28f56-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="28f56-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="28f56-211">Response</span></span>
<span data-ttu-id="28f56-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28f56-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



