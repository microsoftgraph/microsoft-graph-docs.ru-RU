---
title: Создание windowsPhone81ImportedPFXCertificateProfile
description: Создайте новый объект WindowsPhone81ImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d8c8c77801405524294ceb2229cff05b1a109bf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154800"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="fcfb9-103">Создание windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fcfb9-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

<span data-ttu-id="fcfb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcfb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcfb9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcfb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcfb9-107">Создайте [новый объект WindowsPhone81ImportedPFXCertificateProfile.](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-107">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcfb9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fcfb9-108">Prerequisites</span></span>
<span data-ttu-id="fcfb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcfb9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfb9-111">Permission type</span></span>|<span data-ttu-id="fcfb9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcfb9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcfb9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcfb9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcfb9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcfb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-116">Not supported.</span></span>|
|<span data-ttu-id="fcfb9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcfb9-117">Application</span></span>|<span data-ttu-id="fcfb9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcfb9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcfb9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcfb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fcfb9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fcfb9-120">Request headers</span></span>
|<span data-ttu-id="fcfb9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcfb9-121">Header</span></span>|<span data-ttu-id="fcfb9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcfb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcfb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcfb9-123">Authorization</span></span>|<span data-ttu-id="fcfb9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcfb9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcfb9-125">Accept</span></span>|<span data-ttu-id="fcfb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcfb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcfb9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcfb9-127">Request body</span></span>
<span data-ttu-id="fcfb9-128">В теле запроса поставляем представление JSON для объекта windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-128">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="fcfb9-129">В следующей таблице показаны свойства, необходимые при создании windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-129">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="fcfb9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcfb9-130">Property</span></span>|<span data-ttu-id="fcfb9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fcfb9-131">Type</span></span>|<span data-ttu-id="fcfb9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fcfb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcfb9-133">id</span><span class="sxs-lookup"><span data-stu-id="fcfb9-133">id</span></span>|<span data-ttu-id="fcfb9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fcfb9-134">String</span></span>|<span data-ttu-id="fcfb9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-135">Key of the entity.</span></span> <span data-ttu-id="fcfb9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcfb9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fcfb9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcfb9-138">DateTimeOffset</span></span>|<span data-ttu-id="fcfb9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fcfb9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fcfb9-141">roleScopeTagIds</span></span>|<span data-ttu-id="fcfb9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fcfb9-142">String collection</span></span>|<span data-ttu-id="fcfb9-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fcfb9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fcfb9-145">supportsScopeTags</span></span>|<span data-ttu-id="fcfb9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fcfb9-146">Boolean</span></span>|<span data-ttu-id="fcfb9-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fcfb9-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fcfb9-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fcfb9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-150">This property is read-only.</span></span> <span data-ttu-id="fcfb9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fcfb9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fcfb9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fcfb9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fcfb9-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fcfb9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fcfb9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fcfb9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fcfb9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fcfb9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fcfb9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fcfb9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fcfb9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fcfb9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fcfb9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fcfb9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcfb9-164">createdDateTime</span></span>|<span data-ttu-id="fcfb9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcfb9-165">DateTimeOffset</span></span>|<span data-ttu-id="fcfb9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-166">DateTime the object was created.</span></span> <span data-ttu-id="fcfb9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-168">description</span><span class="sxs-lookup"><span data-stu-id="fcfb9-168">description</span></span>|<span data-ttu-id="fcfb9-169">Строка</span><span class="sxs-lookup"><span data-stu-id="fcfb9-169">String</span></span>|<span data-ttu-id="fcfb9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fcfb9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fcfb9-172">displayName</span></span>|<span data-ttu-id="fcfb9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fcfb9-173">String</span></span>|<span data-ttu-id="fcfb9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fcfb9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-176">version</span><span class="sxs-lookup"><span data-stu-id="fcfb9-176">version</span></span>|<span data-ttu-id="fcfb9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fcfb9-177">Int32</span></span>|<span data-ttu-id="fcfb9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-178">Version of the device configuration.</span></span> <span data-ttu-id="fcfb9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fcfb9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fcfb9-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="fcfb9-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="fcfb9-181">Int32</span><span class="sxs-lookup"><span data-stu-id="fcfb9-181">Int32</span></span>|<span data-ttu-id="fcfb9-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fcfb9-183">Допустимые значения от 1 до 99, унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fcfb9-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="fcfb9-184">keyStorageProvider</span></span>|[<span data-ttu-id="fcfb9-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="fcfb9-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="fcfb9-186">Поставщик ключей для хранения данных (KSP), унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="fcfb9-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="fcfb9-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fcfb9-188">subjectNameFormat</span></span>|[<span data-ttu-id="fcfb9-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fcfb9-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fcfb9-190">Формат имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="fcfb9-191">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fcfb9-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fcfb9-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fcfb9-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fcfb9-193">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="fcfb9-194">Тип альтернативного имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="fcfb9-195">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="fcfb9-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fcfb9-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fcfb9-197">Int32</span><span class="sxs-lookup"><span data-stu-id="fcfb9-197">Int32</span></span>|<span data-ttu-id="fcfb9-198">Значение для периода действия сертификата, унаследованной от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fcfb9-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fcfb9-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fcfb9-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fcfb9-200">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="fcfb9-201">Масштабировать период действия сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fcfb9-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="fcfb9-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fcfb9-203">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="fcfb9-203">intendedPurpose</span></span>|[<span data-ttu-id="fcfb9-204">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="fcfb9-204">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="fcfb9-205">Предназначено для профиля сертификата, который может быть ненаназданным, SmimeEncryption, SmimeSigning и т.д. Возможные значения: `unassigned` `smimeEncryption` , , , `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="fcfb9-205">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="fcfb9-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfb9-206">Response</span></span>
<span data-ttu-id="fcfb9-207">В случае успеха этот метод возвращает код отклика и `201 Created` [объект WindowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-207">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcfb9-208">Пример</span><span class="sxs-lookup"><span data-stu-id="fcfb9-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcfb9-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfb9-209">Request</span></span>
<span data-ttu-id="fcfb9-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1364

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="fcfb9-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfb9-211">Response</span></span>
<span data-ttu-id="fcfb9-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcfb9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1536

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
  "intendedPurpose": "smimeEncryption"
}
```




