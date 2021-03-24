---
title: Обновление androidScepCertificateProfile
description: Обновление свойств объекта AndroidScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa6a78252d7549b68b5498582bece1a96bd828a5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137758"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="c8089-103">Обновление androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c8089-103">Update androidScepCertificateProfile</span></span>

<span data-ttu-id="c8089-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8089-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8089-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8089-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8089-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8089-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8089-107">Обновление свойств объекта [AndroidScepCertificateProfile.](../resources/intune-deviceconfig-androidscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-107">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8089-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8089-108">Prerequisites</span></span>
<span data-ttu-id="c8089-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8089-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8089-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8089-111">Permission type</span></span>|<span data-ttu-id="c8089-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8089-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8089-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8089-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8089-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8089-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8089-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8089-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8089-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8089-116">Not supported.</span></span>|
|<span data-ttu-id="c8089-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8089-117">Application</span></span>|<span data-ttu-id="c8089-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8089-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8089-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8089-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c8089-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8089-120">Request headers</span></span>
|<span data-ttu-id="c8089-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8089-121">Header</span></span>|<span data-ttu-id="c8089-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8089-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8089-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8089-123">Authorization</span></span>|<span data-ttu-id="c8089-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8089-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8089-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8089-125">Accept</span></span>|<span data-ttu-id="c8089-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8089-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8089-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8089-127">Request body</span></span>
<span data-ttu-id="c8089-128">В теле запроса поставляем представление JSON для [объекта AndroidScepCertificateProfile.](../resources/intune-deviceconfig-androidscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-128">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="c8089-129">В следующей таблице показаны свойства, необходимые при создании [androidScepCertificateProfile.](../resources/intune-deviceconfig-androidscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-129">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="c8089-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8089-130">Property</span></span>|<span data-ttu-id="c8089-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8089-131">Type</span></span>|<span data-ttu-id="c8089-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8089-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8089-133">id</span><span class="sxs-lookup"><span data-stu-id="c8089-133">id</span></span>|<span data-ttu-id="c8089-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c8089-134">String</span></span>|<span data-ttu-id="c8089-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c8089-135">Key of the entity.</span></span> <span data-ttu-id="c8089-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8089-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c8089-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8089-138">DateTimeOffset</span></span>|<span data-ttu-id="c8089-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c8089-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c8089-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8089-141">roleScopeTagIds</span></span>|<span data-ttu-id="c8089-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8089-142">String collection</span></span>|<span data-ttu-id="c8089-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="c8089-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c8089-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c8089-145">supportsScopeTags</span></span>|<span data-ttu-id="c8089-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8089-146">Boolean</span></span>|<span data-ttu-id="c8089-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c8089-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c8089-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="c8089-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c8089-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c8089-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c8089-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8089-150">This property is read-only.</span></span> <span data-ttu-id="c8089-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8089-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c8089-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c8089-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c8089-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8089-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c8089-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8089-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c8089-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c8089-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c8089-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8089-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c8089-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8089-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c8089-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c8089-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c8089-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c8089-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c8089-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8089-164">createdDateTime</span></span>|<span data-ttu-id="c8089-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8089-165">DateTimeOffset</span></span>|<span data-ttu-id="c8089-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c8089-166">DateTime the object was created.</span></span> <span data-ttu-id="c8089-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-168">description</span><span class="sxs-lookup"><span data-stu-id="c8089-168">description</span></span>|<span data-ttu-id="c8089-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c8089-169">String</span></span>|<span data-ttu-id="c8089-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8089-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c8089-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c8089-172">displayName</span></span>|<span data-ttu-id="c8089-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c8089-173">String</span></span>|<span data-ttu-id="c8089-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8089-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c8089-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-176">version</span><span class="sxs-lookup"><span data-stu-id="c8089-176">version</span></span>|<span data-ttu-id="c8089-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c8089-177">Int32</span></span>|<span data-ttu-id="c8089-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c8089-178">Version of the device configuration.</span></span> <span data-ttu-id="c8089-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c8089-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c8089-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="c8089-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c8089-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c8089-181">Int32</span></span>|<span data-ttu-id="c8089-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c8089-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c8089-183">Допустимые значения от 1 до 99, унаследованные от [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8089-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8089-184">subjectNameFormat</span></span>|[<span data-ttu-id="c8089-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c8089-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c8089-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c8089-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="c8089-187">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8089-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c8089-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c8089-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8089-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c8089-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c8089-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="c8089-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c8089-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c8089-192">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8089-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="c8089-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="c8089-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c8089-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c8089-195">Int32</span><span class="sxs-lookup"><span data-stu-id="c8089-195">Int32</span></span>|<span data-ttu-id="c8089-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c8089-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c8089-197">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8089-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8089-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c8089-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c8089-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="c8089-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c8089-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c8089-201">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="c8089-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c8089-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c8089-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="c8089-203">extendedKeyUsages</span></span>|<span data-ttu-id="c8089-204">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c8089-205">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="c8089-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c8089-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c8089-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c8089-207">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c8089-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c8089-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="c8089-208">scepServerUrls</span></span>|<span data-ttu-id="c8089-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8089-209">String collection</span></span>|<span data-ttu-id="c8089-210">URL-адрес сервера SCEP Server (s)</span><span class="sxs-lookup"><span data-stu-id="c8089-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="c8089-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c8089-211">subjectNameFormatString</span></span>|<span data-ttu-id="c8089-212">Строка</span><span class="sxs-lookup"><span data-stu-id="c8089-212">String</span></span>|<span data-ttu-id="c8089-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c8089-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c8089-214">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="c8089-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c8089-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="c8089-215">keyUsage</span></span>|[<span data-ttu-id="c8089-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="c8089-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="c8089-217">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8089-217">SCEP Key Usage.</span></span> <span data-ttu-id="c8089-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c8089-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c8089-219">keySize</span><span class="sxs-lookup"><span data-stu-id="c8089-219">keySize</span></span>|[<span data-ttu-id="c8089-220">keySize</span><span class="sxs-lookup"><span data-stu-id="c8089-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="c8089-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8089-221">SCEP Key Size.</span></span> <span data-ttu-id="c8089-222">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="c8089-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="c8089-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c8089-223">hashAlgorithm</span></span>|[<span data-ttu-id="c8089-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="c8089-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="c8089-225">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="c8089-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c8089-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c8089-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c8089-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c8089-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c8089-228">Строка</span><span class="sxs-lookup"><span data-stu-id="c8089-228">String</span></span>|<span data-ttu-id="c8089-229">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="c8089-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c8089-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8089-230">Response</span></span>
<span data-ttu-id="c8089-231">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8089-231">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8089-232">Пример</span><span class="sxs-lookup"><span data-stu-id="c8089-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8089-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8089-233">Request</span></span>
<span data-ttu-id="c8089-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8089-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="c8089-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8089-235">Response</span></span>
<span data-ttu-id="c8089-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8089-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1919

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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




