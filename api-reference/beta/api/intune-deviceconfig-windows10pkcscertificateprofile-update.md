---
title: Обновление windows10PkcsCertificateProfile
description: Обновление свойств объекта windows10PkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5eaf9f9ea123752aa75957b99911bcbdd013b6e7
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947248"
---
# <a name="update-windows10pkcscertificateprofile"></a><span data-ttu-id="5ce3a-103">Обновление windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5ce3a-103">Update windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="5ce3a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ce3a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ce3a-106">Обновление свойств объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ce3a-106">Update the properties of a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ce3a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ce3a-107">Prerequisites</span></span>
<span data-ttu-id="5ce3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ce3a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ce3a-110">Permission type</span></span>|<span data-ttu-id="5ce3a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ce3a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ce3a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ce3a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ce3a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ce3a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-115">Not supported.</span></span>|
|<span data-ttu-id="5ce3a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ce3a-116">Application</span></span>|<span data-ttu-id="5ce3a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ce3a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ce3a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ce3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ce3a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5ce3a-119">Request headers</span></span>
|<span data-ttu-id="5ce3a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ce3a-120">Header</span></span>|<span data-ttu-id="5ce3a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ce3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ce3a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ce3a-122">Authorization</span></span>|<span data-ttu-id="5ce3a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ce3a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5ce3a-124">Accept</span></span>|<span data-ttu-id="5ce3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ce3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ce3a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ce3a-126">Request body</span></span>
<span data-ttu-id="5ce3a-127">В тексте запроса добавьте представление объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-127">In the request body, supply a JSON representation for the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="5ce3a-128">В следующей таблице приведены свойства, необходимые при создании [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-128">The following table shows the properties that are required when you create the [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md).</span></span>

|<span data-ttu-id="5ce3a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ce3a-129">Property</span></span>|<span data-ttu-id="5ce3a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5ce3a-130">Type</span></span>|<span data-ttu-id="5ce3a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ce3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ce3a-132">id</span><span class="sxs-lookup"><span data-stu-id="5ce3a-132">id</span></span>|<span data-ttu-id="5ce3a-133">String</span><span class="sxs-lookup"><span data-stu-id="5ce3a-133">String</span></span>|<span data-ttu-id="5ce3a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-134">Key of the entity.</span></span> <span data-ttu-id="5ce3a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ce3a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ce3a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ce3a-137">DateTimeOffset</span></span>|<span data-ttu-id="5ce3a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ce3a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ce3a-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ce3a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5ce3a-141">String collection</span></span>|<span data-ttu-id="5ce3a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ce3a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5ce3a-144">supportsScopeTags</span></span>|<span data-ttu-id="5ce3a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ce3a-145">Boolean</span></span>|<span data-ttu-id="5ce3a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ce3a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ce3a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ce3a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-149">This property is read-only.</span></span> <span data-ttu-id="5ce3a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ce3a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5ce3a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ce3a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5ce3a-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5ce3a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ce3a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5ce3a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ce3a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5ce3a-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5ce3a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ce3a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5ce3a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ce3a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5ce3a-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5ce3a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ce3a-163">createdDateTime</span></span>|<span data-ttu-id="5ce3a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ce3a-164">DateTimeOffset</span></span>|<span data-ttu-id="5ce3a-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-165">DateTime the object was created.</span></span> <span data-ttu-id="5ce3a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-167">description</span><span class="sxs-lookup"><span data-stu-id="5ce3a-167">description</span></span>|<span data-ttu-id="5ce3a-168">String</span><span class="sxs-lookup"><span data-stu-id="5ce3a-168">String</span></span>|<span data-ttu-id="5ce3a-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ce3a-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5ce3a-171">displayName</span></span>|<span data-ttu-id="5ce3a-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-172">String</span></span>|<span data-ttu-id="5ce3a-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ce3a-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-175">version</span><span class="sxs-lookup"><span data-stu-id="5ce3a-175">version</span></span>|<span data-ttu-id="5ce3a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5ce3a-176">Int32</span></span>|<span data-ttu-id="5ce3a-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-177">Version of the device configuration.</span></span> <span data-ttu-id="5ce3a-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ce3a-179">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="5ce3a-179">renewalThresholdPercentage</span></span>|<span data-ttu-id="5ce3a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="5ce3a-180">Int32</span></span>|<span data-ttu-id="5ce3a-181">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-181">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5ce3a-182">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-182">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ce3a-183">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="5ce3a-183">keyStorageProvider</span></span>|[<span data-ttu-id="5ce3a-184">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="5ce3a-184">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="5ce3a-185">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-185">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ce3a-186">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-186">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="5ce3a-187">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5ce3a-187">subjectNameFormat</span></span>|[<span data-ttu-id="5ce3a-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5ce3a-188">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5ce3a-189">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-189">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ce3a-190">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-190">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5ce3a-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ce3a-191">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5ce3a-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ce3a-192">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5ce3a-193">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-193">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ce3a-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5ce3a-195">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5ce3a-195">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5ce3a-196">Int32</span><span class="sxs-lookup"><span data-stu-id="5ce3a-196">Int32</span></span>|<span data-ttu-id="5ce3a-197">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-197">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ce3a-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ce3a-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5ce3a-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ce3a-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5ce3a-200">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-200">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5ce3a-201">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-201">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5ce3a-202">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="5ce3a-202">certificationAuthority</span></span>|<span data-ttu-id="5ce3a-203">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-203">String</span></span>|<span data-ttu-id="5ce3a-204">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="5ce3a-204">PKCS Certification Authority</span></span>|
|<span data-ttu-id="5ce3a-205">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="5ce3a-205">certificationAuthorityName</span></span>|<span data-ttu-id="5ce3a-206">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-206">String</span></span>|<span data-ttu-id="5ce3a-207">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="5ce3a-207">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="5ce3a-208">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="5ce3a-208">certificateTemplateName</span></span>|<span data-ttu-id="5ce3a-209">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-209">String</span></span>|<span data-ttu-id="5ce3a-210">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="5ce3a-210">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="5ce3a-211">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5ce3a-211">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5ce3a-212">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-212">String</span></span>|<span data-ttu-id="5ce3a-213">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-213">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5ce3a-214">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="5ce3a-214">extendedKeyUsages</span></span>|<span data-ttu-id="5ce3a-215">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-215">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5ce3a-216">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="5ce3a-216">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5ce3a-217">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-217">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5ce3a-218">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="5ce3a-218">subjectNameFormatString</span></span>|<span data-ttu-id="5ce3a-219">Строка</span><span class="sxs-lookup"><span data-stu-id="5ce3a-219">String</span></span>|<span data-ttu-id="5ce3a-220">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-220">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5ce3a-221">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="5ce3a-221">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5ce3a-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5ce3a-222">certificateStore</span></span>|[<span data-ttu-id="5ce3a-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5ce3a-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="5ce3a-224">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-224">Target store certificate.</span></span> <span data-ttu-id="5ce3a-225">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-225">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5ce3a-226">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="5ce3a-226">customSubjectAlternativeNames</span></span>|<span data-ttu-id="5ce3a-227">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="5ce3a-227">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="5ce3a-228">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-228">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="5ce3a-229">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-229">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5ce3a-230">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ce3a-230">Response</span></span>
<span data-ttu-id="5ce3a-231">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-231">If successful, this method returns a `200 OK` response code and an updated [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ce3a-232">Пример</span><span class="sxs-lookup"><span data-stu-id="5ce3a-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ce3a-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ce3a-233">Request</span></span>
<span data-ttu-id="5ce3a-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2074

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value",
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

### <a name="response"></a><span data-ttu-id="5ce3a-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ce3a-235">Response</span></span>
<span data-ttu-id="5ce3a-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ce3a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2246

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectNameFormatString": "Subject Name Format String value",
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





