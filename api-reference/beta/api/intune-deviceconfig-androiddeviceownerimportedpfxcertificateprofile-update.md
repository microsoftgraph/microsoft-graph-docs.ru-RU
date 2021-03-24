---
title: Обновление androidDeviceOwnerImportedPFXCertificateProfile
description: Обновление свойств объекта androidDeviceOwnerImportedPFXCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c7e152720c1de2259d923999c9ae8477c0df4123
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138559"
---
# <a name="update-androiddeviceownerimportedpfxcertificateprofile"></a><span data-ttu-id="c7ebe-103">Обновление androidDeviceOwnerImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c7ebe-103">Update androidDeviceOwnerImportedPFXCertificateProfile</span></span>

<span data-ttu-id="c7ebe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7ebe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7ebe-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7ebe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7ebe-107">Обновление свойств объекта [androidDeviceOwnerImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-107">Update the properties of a [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7ebe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7ebe-108">Prerequisites</span></span>
<span data-ttu-id="c7ebe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7ebe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ebe-111">Permission type</span></span>|<span data-ttu-id="c7ebe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7ebe-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7ebe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ebe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7ebe-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7ebe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-116">Not supported.</span></span>|
|<span data-ttu-id="c7ebe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7ebe-117">Application</span></span>|<span data-ttu-id="c7ebe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7ebe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7ebe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ebe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c7ebe-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7ebe-120">Request headers</span></span>
|<span data-ttu-id="c7ebe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7ebe-121">Header</span></span>|<span data-ttu-id="c7ebe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7ebe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7ebe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ebe-123">Authorization</span></span>|<span data-ttu-id="c7ebe-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7ebe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7ebe-125">Accept</span></span>|<span data-ttu-id="c7ebe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7ebe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7ebe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ebe-127">Request body</span></span>
<span data-ttu-id="c7ebe-128">В теле запроса поставляем представление JSON для [объекта AndroidDeviceOwnerImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-128">In the request body, supply a JSON representation for the [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="c7ebe-129">В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerImportedPFXCertificateProfile.](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-129">The following table shows the properties that are required when you create the [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="c7ebe-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7ebe-130">Property</span></span>|<span data-ttu-id="c7ebe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ebe-131">Type</span></span>|<span data-ttu-id="c7ebe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ebe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ebe-133">id</span><span class="sxs-lookup"><span data-stu-id="c7ebe-133">id</span></span>|<span data-ttu-id="c7ebe-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c7ebe-134">String</span></span>|<span data-ttu-id="c7ebe-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-135">Key of the entity.</span></span> <span data-ttu-id="c7ebe-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7ebe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c7ebe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7ebe-138">DateTimeOffset</span></span>|<span data-ttu-id="c7ebe-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c7ebe-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7ebe-141">roleScopeTagIds</span></span>|<span data-ttu-id="c7ebe-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7ebe-142">String collection</span></span>|<span data-ttu-id="c7ebe-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7ebe-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c7ebe-145">supportsScopeTags</span></span>|<span data-ttu-id="c7ebe-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7ebe-146">Boolean</span></span>|<span data-ttu-id="c7ebe-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c7ebe-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c7ebe-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c7ebe-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-150">This property is read-only.</span></span> <span data-ttu-id="c7ebe-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7ebe-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c7ebe-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7ebe-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c7ebe-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c7ebe-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7ebe-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c7ebe-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7ebe-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c7ebe-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c7ebe-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7ebe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c7ebe-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7ebe-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c7ebe-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c7ebe-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7ebe-164">createdDateTime</span></span>|<span data-ttu-id="c7ebe-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7ebe-165">DateTimeOffset</span></span>|<span data-ttu-id="c7ebe-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-166">DateTime the object was created.</span></span> <span data-ttu-id="c7ebe-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-168">description</span><span class="sxs-lookup"><span data-stu-id="c7ebe-168">description</span></span>|<span data-ttu-id="c7ebe-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c7ebe-169">String</span></span>|<span data-ttu-id="c7ebe-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7ebe-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c7ebe-172">displayName</span></span>|<span data-ttu-id="c7ebe-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c7ebe-173">String</span></span>|<span data-ttu-id="c7ebe-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7ebe-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-176">version</span><span class="sxs-lookup"><span data-stu-id="c7ebe-176">version</span></span>|<span data-ttu-id="c7ebe-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ebe-177">Int32</span></span>|<span data-ttu-id="c7ebe-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-178">Version of the device configuration.</span></span> <span data-ttu-id="c7ebe-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7ebe-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c7ebe-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c7ebe-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ebe-181">Int32</span></span>|<span data-ttu-id="c7ebe-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c7ebe-183">Допустимые значения от 1 до 99, унаследованные от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7ebe-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c7ebe-184">subjectNameFormat</span></span>|[<span data-ttu-id="c7ebe-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c7ebe-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c7ebe-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="c7ebe-187">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="c7ebe-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c7ebe-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c7ebe-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c7ebe-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c7ebe-190">Int32</span></span>|<span data-ttu-id="c7ebe-191">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c7ebe-192">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7ebe-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c7ebe-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c7ebe-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c7ebe-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="c7ebe-195">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c7ebe-196">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="c7ebe-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c7ebe-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c7ebe-198">extendedKeyUsages</span></span>|<span data-ttu-id="c7ebe-199">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c7ebe-200">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c7ebe-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c7ebe-202">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7ebe-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7ebe-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c7ebe-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c7ebe-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c7ebe-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="c7ebe-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c7ebe-206">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7ebe-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="c7ebe-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="c7ebe-208">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c7ebe-208">intendedPurpose</span></span>|[<span data-ttu-id="c7ebe-209">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c7ebe-209">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c7ebe-210">Предназначено для профиля сертификата, который может быть ненаназданным, SmimeEncryption, SmimeSigning и т.д. Возможные значения: `unassigned` `smimeEncryption` , , , `smimeSigning` `vpn` `wifi` .</span><span class="sxs-lookup"><span data-stu-id="c7ebe-210">Intended Purpose of the Certificate Profile - which could be Unassigned, SmimeEncryption, SmimeSigning etc. Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c7ebe-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ebe-211">Response</span></span>
<span data-ttu-id="c7ebe-212">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-212">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7ebe-213">Пример</span><span class="sxs-lookup"><span data-stu-id="c7ebe-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7ebe-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ebe-214">Request</span></span>
<span data-ttu-id="c7ebe-215">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1503

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="c7ebe-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ebe-216">Response</span></span>
<span data-ttu-id="c7ebe-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7ebe-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1675

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
  "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress",
  "intendedPurpose": "smimeEncryption"
}
```




