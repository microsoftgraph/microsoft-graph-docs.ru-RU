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
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="df479-103">Создание Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="df479-103">Create macOSImportedPFXCertificateProfile</span></span>

<span data-ttu-id="df479-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df479-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df479-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df479-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df479-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df479-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df479-107">Создание нового объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="df479-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df479-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="df479-108">Prerequisites</span></span>
<span data-ttu-id="df479-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df479-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df479-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df479-111">Permission type</span></span>|<span data-ttu-id="df479-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="df479-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df479-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df479-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df479-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df479-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df479-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df479-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df479-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df479-116">Not supported.</span></span>|
|<span data-ttu-id="df479-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df479-117">Application</span></span>|<span data-ttu-id="df479-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df479-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="df479-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df479-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="df479-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="df479-120">Request headers</span></span>
|<span data-ttu-id="df479-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df479-121">Header</span></span>|<span data-ttu-id="df479-122">Значение</span><span class="sxs-lookup"><span data-stu-id="df479-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df479-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df479-123">Authorization</span></span>|<span data-ttu-id="df479-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df479-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df479-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df479-125">Accept</span></span>|<span data-ttu-id="df479-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df479-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df479-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="df479-127">Request body</span></span>
<span data-ttu-id="df479-128">В тексте запроса добавьте представление объекта Макосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df479-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="df479-129">В следующей таблице приведены свойства, необходимые при создании Макосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="df479-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="df479-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df479-130">Property</span></span>|<span data-ttu-id="df479-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df479-131">Type</span></span>|<span data-ttu-id="df479-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df479-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df479-133">id</span><span class="sxs-lookup"><span data-stu-id="df479-133">id</span></span>|<span data-ttu-id="df479-134">String</span><span class="sxs-lookup"><span data-stu-id="df479-134">String</span></span>|<span data-ttu-id="df479-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="df479-135">Key of the entity.</span></span> <span data-ttu-id="df479-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df479-137">lastModifiedDateTime</span></span>|<span data-ttu-id="df479-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df479-138">DateTimeOffset</span></span>|<span data-ttu-id="df479-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="df479-139">DateTime the object was last modified.</span></span> <span data-ttu-id="df479-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df479-141">roleScopeTagIds</span></span>|<span data-ttu-id="df479-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="df479-142">String collection</span></span>|<span data-ttu-id="df479-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="df479-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="df479-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="df479-145">supportsScopeTags</span></span>|<span data-ttu-id="df479-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="df479-146">Boolean</span></span>|<span data-ttu-id="df479-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="df479-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="df479-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="df479-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="df479-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="df479-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="df479-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="df479-150">This property is read-only.</span></span> <span data-ttu-id="df479-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="df479-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="df479-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="df479-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="df479-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="df479-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="df479-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="df479-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="df479-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="df479-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="df479-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="df479-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="df479-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="df479-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="df479-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="df479-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="df479-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="df479-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="df479-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df479-164">createdDateTime</span></span>|<span data-ttu-id="df479-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df479-165">DateTimeOffset</span></span>|<span data-ttu-id="df479-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="df479-166">DateTime the object was created.</span></span> <span data-ttu-id="df479-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-168">description</span><span class="sxs-lookup"><span data-stu-id="df479-168">description</span></span>|<span data-ttu-id="df479-169">String</span><span class="sxs-lookup"><span data-stu-id="df479-169">String</span></span>|<span data-ttu-id="df479-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="df479-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df479-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-172">displayName</span><span class="sxs-lookup"><span data-stu-id="df479-172">displayName</span></span>|<span data-ttu-id="df479-173">Строка</span><span class="sxs-lookup"><span data-stu-id="df479-173">String</span></span>|<span data-ttu-id="df479-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="df479-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df479-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-176">version</span><span class="sxs-lookup"><span data-stu-id="df479-176">version</span></span>|<span data-ttu-id="df479-177">Int32</span><span class="sxs-lookup"><span data-stu-id="df479-177">Int32</span></span>|<span data-ttu-id="df479-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="df479-178">Version of the device configuration.</span></span> <span data-ttu-id="df479-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="df479-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df479-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="df479-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="df479-181">Int32</span><span class="sxs-lookup"><span data-stu-id="df479-181">Int32</span></span>|<span data-ttu-id="df479-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="df479-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="df479-183">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="df479-183">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="df479-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="df479-184">subjectNameFormat</span></span>|[<span data-ttu-id="df479-185">апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="df479-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="df479-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="df479-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="df479-187">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df479-187">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="df479-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="df479-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="df479-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="df479-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="df479-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="df479-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="df479-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="df479-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="df479-192">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df479-192">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="df479-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="df479-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="df479-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="df479-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="df479-195">Int32</span><span class="sxs-lookup"><span data-stu-id="df479-195">Int32</span></span>|<span data-ttu-id="df479-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="df479-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="df479-197">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="df479-197">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="df479-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="df479-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="df479-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="df479-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="df479-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="df479-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="df479-201">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="df479-201">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="df479-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="df479-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="df479-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="df479-203">intendedPurpose</span></span>|[<span data-ttu-id="df479-204">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="df479-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="df479-205">Предполагаемое назначение профиля сертификата, который может быть неназначенным, Смиминкриптион, Смимесигнинг и т. д. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`,. `wifi`</span><span class="sxs-lookup"><span data-stu-id="df479-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="df479-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="df479-206">Response</span></span>
<span data-ttu-id="df479-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df479-207">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df479-208">Пример</span><span class="sxs-lookup"><span data-stu-id="df479-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="df479-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="df479-209">Request</span></span>
<span data-ttu-id="df479-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df479-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df479-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="df479-211">Response</span></span>
<span data-ttu-id="df479-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df479-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



