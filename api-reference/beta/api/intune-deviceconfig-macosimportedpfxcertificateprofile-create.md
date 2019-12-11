---
title: Создание Макосимпортедпфксцертификатепрофиле
description: Создание нового объекта Макосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 164d9cdbbbe5ad6f9c43e2bd22c4cdf9b064cbef
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948256"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="63305-103">Создание Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="63305-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="63305-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63305-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63305-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63305-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63305-106">Создание нового объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="63305-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63305-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="63305-107">Prerequisites</span></span>
<span data-ttu-id="63305-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63305-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63305-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63305-110">Permission type</span></span>|<span data-ttu-id="63305-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="63305-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63305-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63305-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63305-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63305-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63305-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63305-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63305-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63305-115">Not supported.</span></span>|
|<span data-ttu-id="63305-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63305-116">Application</span></span>|<span data-ttu-id="63305-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63305-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63305-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63305-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63305-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="63305-119">Request headers</span></span>
|<span data-ttu-id="63305-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63305-120">Header</span></span>|<span data-ttu-id="63305-121">Значение</span><span class="sxs-lookup"><span data-stu-id="63305-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63305-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63305-122">Authorization</span></span>|<span data-ttu-id="63305-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63305-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63305-124">Accept</span><span class="sxs-lookup"><span data-stu-id="63305-124">Accept</span></span>|<span data-ttu-id="63305-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63305-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63305-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63305-126">Request body</span></span>
<span data-ttu-id="63305-127">В тексте запроса добавьте представление объекта Макосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63305-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="63305-128">В следующей таблице приведены свойства, необходимые при создании Макосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="63305-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="63305-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="63305-129">Property</span></span>|<span data-ttu-id="63305-130">Тип</span><span class="sxs-lookup"><span data-stu-id="63305-130">Type</span></span>|<span data-ttu-id="63305-131">Описание</span><span class="sxs-lookup"><span data-stu-id="63305-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63305-132">id</span><span class="sxs-lookup"><span data-stu-id="63305-132">id</span></span>|<span data-ttu-id="63305-133">String</span><span class="sxs-lookup"><span data-stu-id="63305-133">String</span></span>|<span data-ttu-id="63305-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="63305-134">Key of the entity.</span></span> <span data-ttu-id="63305-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63305-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63305-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63305-137">DateTimeOffset</span></span>|<span data-ttu-id="63305-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="63305-138">DateTime the object was last modified.</span></span> <span data-ttu-id="63305-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63305-140">roleScopeTagIds</span></span>|<span data-ttu-id="63305-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="63305-141">String collection</span></span>|<span data-ttu-id="63305-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="63305-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63305-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="63305-144">supportsScopeTags</span></span>|<span data-ttu-id="63305-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="63305-145">Boolean</span></span>|<span data-ttu-id="63305-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="63305-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63305-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="63305-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63305-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="63305-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63305-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="63305-149">This property is read-only.</span></span> <span data-ttu-id="63305-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63305-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="63305-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="63305-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="63305-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63305-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="63305-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63305-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="63305-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="63305-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="63305-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63305-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="63305-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63305-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="63305-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="63305-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="63305-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="63305-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="63305-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63305-163">createdDateTime</span></span>|<span data-ttu-id="63305-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63305-164">DateTimeOffset</span></span>|<span data-ttu-id="63305-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="63305-165">DateTime the object was created.</span></span> <span data-ttu-id="63305-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-167">description</span><span class="sxs-lookup"><span data-stu-id="63305-167">description</span></span>|<span data-ttu-id="63305-168">String</span><span class="sxs-lookup"><span data-stu-id="63305-168">String</span></span>|<span data-ttu-id="63305-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63305-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63305-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-171">displayName</span><span class="sxs-lookup"><span data-stu-id="63305-171">displayName</span></span>|<span data-ttu-id="63305-172">Строка</span><span class="sxs-lookup"><span data-stu-id="63305-172">String</span></span>|<span data-ttu-id="63305-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63305-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63305-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-175">version</span><span class="sxs-lookup"><span data-stu-id="63305-175">version</span></span>|<span data-ttu-id="63305-176">Int32</span><span class="sxs-lookup"><span data-stu-id="63305-176">Int32</span></span>|<span data-ttu-id="63305-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="63305-177">Version of the device configuration.</span></span> <span data-ttu-id="63305-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63305-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63305-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="63305-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="63305-180">Int32</span><span class="sxs-lookup"><span data-stu-id="63305-180">Int32</span></span>|<span data-ttu-id="63305-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="63305-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="63305-182">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="63305-182">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="63305-183">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="63305-183">subjectNameFormat</span></span>|[<span data-ttu-id="63305-184">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="63305-184">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="63305-185">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="63305-185">Certificate Subject Name Format.</span></span> <span data-ttu-id="63305-186">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="63305-186">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="63305-187">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="63305-187">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="63305-188">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="63305-188">subjectAlternativeNameType</span></span>|[<span data-ttu-id="63305-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="63305-189">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="63305-190">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="63305-190">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="63305-191">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="63305-191">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="63305-192">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="63305-192">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="63305-193">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="63305-193">certificateValidityPeriodValue</span></span>|<span data-ttu-id="63305-194">Int32</span><span class="sxs-lookup"><span data-stu-id="63305-194">Int32</span></span>|<span data-ttu-id="63305-195">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="63305-195">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="63305-196">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="63305-196">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="63305-197">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="63305-197">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="63305-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="63305-198">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="63305-199">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="63305-199">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="63305-200">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="63305-200">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="63305-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="63305-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="63305-202">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="63305-202">intendedPurpose</span></span>|[<span data-ttu-id="63305-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="63305-203">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="63305-204">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="63305-204">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="63305-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="63305-205">Response</span></span>
<span data-ttu-id="63305-206">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63305-206">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63305-207">Пример</span><span class="sxs-lookup"><span data-stu-id="63305-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="63305-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="63305-208">Request</span></span>
<span data-ttu-id="63305-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63305-209">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63305-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="63305-210">Response</span></span>
<span data-ttu-id="63305-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63305-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





