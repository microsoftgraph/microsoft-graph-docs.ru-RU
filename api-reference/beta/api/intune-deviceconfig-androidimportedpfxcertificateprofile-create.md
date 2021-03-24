---
title: Создание androidImportedPFXCertificateProfile
description: Создайте новый объект androidImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8fbe8280d44d75c51cb5f0b847ca4baeec687c2c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138010"
---
# <a name="create-androidimportedpfxcertificateprofile"></a><span data-ttu-id="1959d-103">Создание androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="1959d-103">Create androidImportedPFXCertificateProfile</span></span>

<span data-ttu-id="1959d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1959d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1959d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1959d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1959d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1959d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1959d-107">Создайте [новый объект androidImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-107">Create a new [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1959d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1959d-108">Prerequisites</span></span>
<span data-ttu-id="1959d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1959d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1959d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1959d-111">Permission type</span></span>|<span data-ttu-id="1959d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1959d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1959d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1959d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1959d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1959d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1959d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1959d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1959d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1959d-116">Not supported.</span></span>|
|<span data-ttu-id="1959d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1959d-117">Application</span></span>|<span data-ttu-id="1959d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1959d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1959d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1959d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1959d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1959d-120">Request headers</span></span>
|<span data-ttu-id="1959d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1959d-121">Header</span></span>|<span data-ttu-id="1959d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1959d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1959d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1959d-123">Authorization</span></span>|<span data-ttu-id="1959d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1959d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1959d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1959d-125">Accept</span></span>|<span data-ttu-id="1959d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1959d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1959d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1959d-127">Request body</span></span>
<span data-ttu-id="1959d-128">В теле запроса поставляем представление JSON для объекта androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1959d-128">In the request body, supply a JSON representation for the androidImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1959d-129">В следующей таблице показаны свойства, необходимые при создании androidImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="1959d-129">The following table shows the properties that are required when you create the androidImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1959d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1959d-130">Property</span></span>|<span data-ttu-id="1959d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1959d-131">Type</span></span>|<span data-ttu-id="1959d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1959d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1959d-133">id</span><span class="sxs-lookup"><span data-stu-id="1959d-133">id</span></span>|<span data-ttu-id="1959d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1959d-134">String</span></span>|<span data-ttu-id="1959d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1959d-135">Key of the entity.</span></span> <span data-ttu-id="1959d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1959d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1959d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1959d-138">DateTimeOffset</span></span>|<span data-ttu-id="1959d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1959d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1959d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1959d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1959d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1959d-142">String collection</span></span>|<span data-ttu-id="1959d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="1959d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1959d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1959d-145">supportsScopeTags</span></span>|<span data-ttu-id="1959d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1959d-146">Boolean</span></span>|<span data-ttu-id="1959d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1959d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1959d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="1959d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1959d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1959d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1959d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1959d-150">This property is read-only.</span></span> <span data-ttu-id="1959d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1959d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1959d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1959d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1959d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1959d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1959d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1959d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1959d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1959d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1959d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1959d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1959d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1959d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1959d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1959d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1959d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1959d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1959d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1959d-164">createdDateTime</span></span>|<span data-ttu-id="1959d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1959d-165">DateTimeOffset</span></span>|<span data-ttu-id="1959d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1959d-166">DateTime the object was created.</span></span> <span data-ttu-id="1959d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-168">description</span><span class="sxs-lookup"><span data-stu-id="1959d-168">description</span></span>|<span data-ttu-id="1959d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="1959d-169">String</span></span>|<span data-ttu-id="1959d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1959d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1959d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1959d-172">displayName</span></span>|<span data-ttu-id="1959d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1959d-173">String</span></span>|<span data-ttu-id="1959d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1959d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1959d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-176">version</span><span class="sxs-lookup"><span data-stu-id="1959d-176">version</span></span>|<span data-ttu-id="1959d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1959d-177">Int32</span></span>|<span data-ttu-id="1959d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1959d-178">Version of the device configuration.</span></span> <span data-ttu-id="1959d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1959d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1959d-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1959d-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="1959d-181">Int32</span><span class="sxs-lookup"><span data-stu-id="1959d-181">Int32</span></span>|<span data-ttu-id="1959d-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="1959d-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1959d-183">Допустимые значения от 1 до 99, унаследованные от [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1959d-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1959d-184">subjectNameFormat</span></span>|[<span data-ttu-id="1959d-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1959d-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1959d-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1959d-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="1959d-187">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1959d-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="1959d-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1959d-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1959d-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1959d-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1959d-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="1959d-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="1959d-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1959d-192">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1959d-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="1959d-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="1959d-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1959d-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1959d-195">Int32</span><span class="sxs-lookup"><span data-stu-id="1959d-195">Int32</span></span>|<span data-ttu-id="1959d-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1959d-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="1959d-197">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1959d-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1959d-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1959d-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1959d-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="1959d-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="1959d-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1959d-201">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1959d-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="1959d-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1959d-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="1959d-203">extendedKeyUsages</span></span>|<span data-ttu-id="1959d-204">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="1959d-205">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="1959d-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="1959d-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1959d-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1959d-207">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="1959d-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1959d-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1959d-208">intendedPurpose</span></span>|[<span data-ttu-id="1959d-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1959d-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1959d-210">Предназначено для профиля сертификата, который может быть ненаназданным, SmimeEncryption, SmimeSigning и т.д. Возможные значения: `unassigned` `smimeEncryption` , , , `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="1959d-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1959d-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="1959d-211">Response</span></span>
<span data-ttu-id="1959d-212">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1959d-212">If successful, this method returns a `201 Created` response code and a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1959d-213">Пример</span><span class="sxs-lookup"><span data-stu-id="1959d-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="1959d-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="1959d-214">Request</span></span>
<span data-ttu-id="1959d-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1959d-215">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1959d-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="1959d-216">Response</span></span>
<span data-ttu-id="1959d-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1959d-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




