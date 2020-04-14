---
title: Создание windows81SCEPCertificateProfile
description: Создание нового объекта windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8eedf4b5ec94812fbfcb5ff25fa8bf754f89b24
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43430325"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="07c1c-103">Создание windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="07c1c-103">Create windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="07c1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07c1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07c1c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07c1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07c1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07c1c-107">Создание нового объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="07c1c-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07c1c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07c1c-108">Prerequisites</span></span>
<span data-ttu-id="07c1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07c1c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07c1c-111">Permission type</span></span>|<span data-ttu-id="07c1c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07c1c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07c1c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07c1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07c1c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c1c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07c1c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07c1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07c1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07c1c-116">Not supported.</span></span>|
|<span data-ttu-id="07c1c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="07c1c-117">Application</span></span>|<span data-ttu-id="07c1c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07c1c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07c1c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07c1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="07c1c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07c1c-120">Request headers</span></span>
|<span data-ttu-id="07c1c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07c1c-121">Header</span></span>|<span data-ttu-id="07c1c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07c1c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07c1c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c1c-123">Authorization</span></span>|<span data-ttu-id="07c1c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07c1c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07c1c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07c1c-125">Accept</span></span>|<span data-ttu-id="07c1c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07c1c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07c1c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07c1c-127">Request body</span></span>
<span data-ttu-id="07c1c-128">В тексте запроса добавьте представление объекта windows81SCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07c1c-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="07c1c-129">В следующей таблице приведены свойства, необходимые при создании windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="07c1c-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="07c1c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07c1c-130">Property</span></span>|<span data-ttu-id="07c1c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07c1c-131">Type</span></span>|<span data-ttu-id="07c1c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07c1c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07c1c-133">id</span><span class="sxs-lookup"><span data-stu-id="07c1c-133">id</span></span>|<span data-ttu-id="07c1c-134">String</span><span class="sxs-lookup"><span data-stu-id="07c1c-134">String</span></span>|<span data-ttu-id="07c1c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07c1c-135">Key of the entity.</span></span> <span data-ttu-id="07c1c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07c1c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="07c1c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07c1c-138">DateTimeOffset</span></span>|<span data-ttu-id="07c1c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="07c1c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="07c1c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07c1c-141">roleScopeTagIds</span></span>|<span data-ttu-id="07c1c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07c1c-142">String collection</span></span>|<span data-ttu-id="07c1c-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="07c1c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="07c1c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="07c1c-145">supportsScopeTags</span></span>|<span data-ttu-id="07c1c-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="07c1c-146">Boolean</span></span>|<span data-ttu-id="07c1c-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="07c1c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="07c1c-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="07c1c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="07c1c-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="07c1c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="07c1c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07c1c-150">This property is read-only.</span></span> <span data-ttu-id="07c1c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07c1c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="07c1c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="07c1c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="07c1c-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07c1c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="07c1c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07c1c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="07c1c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="07c1c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="07c1c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07c1c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="07c1c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07c1c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="07c1c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="07c1c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="07c1c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="07c1c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="07c1c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07c1c-164">createdDateTime</span></span>|<span data-ttu-id="07c1c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07c1c-165">DateTimeOffset</span></span>|<span data-ttu-id="07c1c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="07c1c-166">DateTime the object was created.</span></span> <span data-ttu-id="07c1c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-168">description</span><span class="sxs-lookup"><span data-stu-id="07c1c-168">description</span></span>|<span data-ttu-id="07c1c-169">String</span><span class="sxs-lookup"><span data-stu-id="07c1c-169">String</span></span>|<span data-ttu-id="07c1c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07c1c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="07c1c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="07c1c-172">displayName</span></span>|<span data-ttu-id="07c1c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="07c1c-173">String</span></span>|<span data-ttu-id="07c1c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07c1c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="07c1c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-176">version</span><span class="sxs-lookup"><span data-stu-id="07c1c-176">version</span></span>|<span data-ttu-id="07c1c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1c-177">Int32</span></span>|<span data-ttu-id="07c1c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07c1c-178">Version of the device configuration.</span></span> <span data-ttu-id="07c1c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07c1c-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="07c1c-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="07c1c-181">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1c-181">Int32</span></span>|<span data-ttu-id="07c1c-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="07c1c-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="07c1c-183">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="07c1c-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="07c1c-184">keyStorageProvider</span></span>|[<span data-ttu-id="07c1c-185">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="07c1c-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="07c1c-186">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="07c1c-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="07c1c-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="07c1c-188">subjectNameFormat</span></span>|[<span data-ttu-id="07c1c-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="07c1c-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="07c1c-190">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="07c1c-191">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="07c1c-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="07c1c-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="07c1c-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="07c1c-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="07c1c-194">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="07c1c-195">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="07c1c-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="07c1c-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="07c1c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="07c1c-197">Int32</span></span>|<span data-ttu-id="07c1c-198">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="07c1c-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="07c1c-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="07c1c-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="07c1c-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="07c1c-201">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07c1c-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="07c1c-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="07c1c-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="07c1c-203">extendedKeyUsages</span></span>|<span data-ttu-id="07c1c-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="07c1c-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="07c1c-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="07c1c-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="07c1c-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="07c1c-207">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="07c1c-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="07c1c-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="07c1c-209">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="07c1c-210">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="07c1c-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="07c1c-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="07c1c-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="07c1c-212">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07c1c-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="07c1c-213">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="07c1c-213">scepServerUrls</span></span>|<span data-ttu-id="07c1c-214">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07c1c-214">String collection</span></span>|<span data-ttu-id="07c1c-215">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="07c1c-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="07c1c-216">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="07c1c-216">subjectNameFormatString</span></span>|<span data-ttu-id="07c1c-217">String</span><span class="sxs-lookup"><span data-stu-id="07c1c-217">String</span></span>|<span data-ttu-id="07c1c-218">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="07c1c-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="07c1c-219">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="07c1c-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="07c1c-220">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="07c1c-220">keyUsage</span></span>|[<span data-ttu-id="07c1c-221">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="07c1c-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="07c1c-222">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="07c1c-222">SCEP Key Usage.</span></span> <span data-ttu-id="07c1c-223">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="07c1c-224">keySize</span><span class="sxs-lookup"><span data-stu-id="07c1c-224">keySize</span></span>|[<span data-ttu-id="07c1c-225">keySize</span><span class="sxs-lookup"><span data-stu-id="07c1c-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="07c1c-226">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="07c1c-226">SCEP Key Size.</span></span> <span data-ttu-id="07c1c-227">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-227">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="07c1c-228">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="07c1c-228">hashAlgorithm</span></span>|[<span data-ttu-id="07c1c-229">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="07c1c-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="07c1c-230">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="07c1c-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="07c1c-231">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="07c1c-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="07c1c-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="07c1c-233">String</span><span class="sxs-lookup"><span data-stu-id="07c1c-233">String</span></span>|<span data-ttu-id="07c1c-234">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="07c1c-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="07c1c-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="07c1c-235">certificateStore</span></span>|[<span data-ttu-id="07c1c-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="07c1c-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="07c1c-237">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="07c1c-237">Target store certificate.</span></span> <span data-ttu-id="07c1c-238">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="07c1c-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="07c1c-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c1c-239">Response</span></span>
<span data-ttu-id="07c1c-240">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="07c1c-240">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07c1c-241">Пример</span><span class="sxs-lookup"><span data-stu-id="07c1c-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="07c1c-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="07c1c-242">Request</span></span>
<span data-ttu-id="07c1c-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07c1c-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="07c1c-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="07c1c-244">Response</span></span>
<span data-ttu-id="07c1c-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07c1c-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```



