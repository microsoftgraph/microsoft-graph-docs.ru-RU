---
title: Обновление windowsPhone81SCEPCertificateProfile
description: Обновление свойств объекта WindowsPhone81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f4be62b347f7a834c8f2000815ebc4c5defe0fa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147135"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="03738-103">Обновление windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="03738-103">Update windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="03738-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03738-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03738-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03738-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03738-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03738-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03738-107">Обновление свойств объекта [WindowsPhone81SCEPCertificateProfile.](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="03738-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03738-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03738-108">Prerequisites</span></span>
<span data-ttu-id="03738-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03738-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03738-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03738-111">Permission type</span></span>|<span data-ttu-id="03738-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03738-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03738-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03738-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03738-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03738-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03738-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03738-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03738-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03738-116">Not supported.</span></span>|
|<span data-ttu-id="03738-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="03738-117">Application</span></span>|<span data-ttu-id="03738-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03738-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03738-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03738-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03738-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03738-120">Request headers</span></span>
|<span data-ttu-id="03738-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03738-121">Header</span></span>|<span data-ttu-id="03738-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03738-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03738-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03738-123">Authorization</span></span>|<span data-ttu-id="03738-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03738-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03738-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03738-125">Accept</span></span>|<span data-ttu-id="03738-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03738-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03738-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03738-127">Request body</span></span>
<span data-ttu-id="03738-128">В теле запроса поставляем представление JSON для [объекта windowsPhone81SCEPCertificateProfile.](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="03738-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="03738-129">В следующей таблице показаны свойства, необходимые при создании [windowsPhone81SCEPCertificateProfile.](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="03738-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="03738-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03738-130">Property</span></span>|<span data-ttu-id="03738-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03738-131">Type</span></span>|<span data-ttu-id="03738-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03738-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03738-133">id</span><span class="sxs-lookup"><span data-stu-id="03738-133">id</span></span>|<span data-ttu-id="03738-134">Строка</span><span class="sxs-lookup"><span data-stu-id="03738-134">String</span></span>|<span data-ttu-id="03738-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03738-135">Key of the entity.</span></span> <span data-ttu-id="03738-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03738-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03738-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03738-138">DateTimeOffset</span></span>|<span data-ttu-id="03738-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="03738-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03738-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03738-141">roleScopeTagIds</span></span>|<span data-ttu-id="03738-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03738-142">String collection</span></span>|<span data-ttu-id="03738-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="03738-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03738-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03738-145">supportsScopeTags</span></span>|<span data-ttu-id="03738-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="03738-146">Boolean</span></span>|<span data-ttu-id="03738-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="03738-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03738-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="03738-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03738-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="03738-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03738-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03738-150">This property is read-only.</span></span> <span data-ttu-id="03738-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03738-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="03738-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03738-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="03738-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03738-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="03738-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03738-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="03738-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03738-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="03738-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03738-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="03738-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03738-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="03738-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03738-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="03738-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03738-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="03738-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03738-164">createdDateTime</span></span>|<span data-ttu-id="03738-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03738-165">DateTimeOffset</span></span>|<span data-ttu-id="03738-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="03738-166">DateTime the object was created.</span></span> <span data-ttu-id="03738-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-168">description</span><span class="sxs-lookup"><span data-stu-id="03738-168">description</span></span>|<span data-ttu-id="03738-169">Строка</span><span class="sxs-lookup"><span data-stu-id="03738-169">String</span></span>|<span data-ttu-id="03738-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03738-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03738-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-172">displayName</span><span class="sxs-lookup"><span data-stu-id="03738-172">displayName</span></span>|<span data-ttu-id="03738-173">Строка</span><span class="sxs-lookup"><span data-stu-id="03738-173">String</span></span>|<span data-ttu-id="03738-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03738-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03738-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-176">version</span><span class="sxs-lookup"><span data-stu-id="03738-176">version</span></span>|<span data-ttu-id="03738-177">Int32</span><span class="sxs-lookup"><span data-stu-id="03738-177">Int32</span></span>|<span data-ttu-id="03738-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03738-178">Version of the device configuration.</span></span> <span data-ttu-id="03738-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03738-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03738-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="03738-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="03738-181">Int32</span><span class="sxs-lookup"><span data-stu-id="03738-181">Int32</span></span>|<span data-ttu-id="03738-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="03738-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="03738-183">Унаследованный от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03738-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="03738-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="03738-184">keyStorageProvider</span></span>|[<span data-ttu-id="03738-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="03738-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="03738-186">Поставщик ключей для хранения данных (KSP).</span><span class="sxs-lookup"><span data-stu-id="03738-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="03738-187">Унаследовано от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03738-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="03738-188">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="03738-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="03738-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03738-189">subjectNameFormat</span></span>|[<span data-ttu-id="03738-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03738-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="03738-191">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="03738-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="03738-192">Унаследовано от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03738-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="03738-193">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="03738-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="03738-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03738-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="03738-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03738-195">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="03738-196">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="03738-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="03738-197">Унаследовано от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03738-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="03738-198">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="03738-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="03738-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="03738-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="03738-200">Int32</span><span class="sxs-lookup"><span data-stu-id="03738-200">Int32</span></span>|<span data-ttu-id="03738-201">Значение для периода проверки подлинности сертификатов.</span><span class="sxs-lookup"><span data-stu-id="03738-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="03738-202">Унаследованный от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03738-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="03738-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03738-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="03738-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03738-204">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="03738-205">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="03738-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="03738-206">Унаследовано от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03738-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="03738-207">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="03738-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="03738-208">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="03738-208">extendedKeyUsages</span></span>|<span data-ttu-id="03738-209">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="03738-209">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="03738-210">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="03738-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="03738-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="03738-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="03738-212">Унаследованный от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03738-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="03738-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="03738-213">scepServerUrls</span></span>|<span data-ttu-id="03738-214">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03738-214">String collection</span></span>|<span data-ttu-id="03738-215">URL-адрес сервера SCEP Server (s).</span><span class="sxs-lookup"><span data-stu-id="03738-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="03738-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="03738-216">subjectNameFormatString</span></span>|<span data-ttu-id="03738-217">Строка</span><span class="sxs-lookup"><span data-stu-id="03738-217">String</span></span>|<span data-ttu-id="03738-218">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="03738-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="03738-219">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="03738-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="03738-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="03738-220">keyUsage</span></span>|[<span data-ttu-id="03738-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="03738-221">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="03738-222">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="03738-222">SCEP Key Usage.</span></span> <span data-ttu-id="03738-223">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="03738-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="03738-224">keySize</span><span class="sxs-lookup"><span data-stu-id="03738-224">keySize</span></span>|[<span data-ttu-id="03738-225">keySize</span><span class="sxs-lookup"><span data-stu-id="03738-225">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="03738-226">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="03738-226">SCEP Key Size.</span></span> <span data-ttu-id="03738-227">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="03738-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="03738-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="03738-228">hashAlgorithm</span></span>|[<span data-ttu-id="03738-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="03738-229">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="03738-230">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="03738-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="03738-231">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="03738-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="03738-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="03738-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="03738-233">Строка</span><span class="sxs-lookup"><span data-stu-id="03738-233">String</span></span>|<span data-ttu-id="03738-234">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="03738-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="03738-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="03738-235">Response</span></span>
<span data-ttu-id="03738-236">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="03738-236">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03738-237">Пример</span><span class="sxs-lookup"><span data-stu-id="03738-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="03738-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="03738-238">Request</span></span>
<span data-ttu-id="03738-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03738-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="03738-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="03738-240">Response</span></span>
<span data-ttu-id="03738-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03738-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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




