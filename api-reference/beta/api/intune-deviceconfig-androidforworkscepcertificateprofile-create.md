---
title: Создание androidForWorkScepCertificateProfile
description: Создайте новый объект AndroidForWorkScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b7a999266c8725fea37ea980be522521cb2eba3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138360"
---
# <a name="create-androidforworkscepcertificateprofile"></a><span data-ttu-id="87986-103">Создание androidForWorkScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="87986-103">Create androidForWorkScepCertificateProfile</span></span>

<span data-ttu-id="87986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87986-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87986-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87986-107">Создайте новый [объект AndroidForWorkScepCertificateProfile.](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="87986-107">Create a new [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87986-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87986-108">Prerequisites</span></span>
<span data-ttu-id="87986-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87986-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87986-111">Permission type</span></span>|<span data-ttu-id="87986-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87986-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87986-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87986-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87986-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87986-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87986-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87986-116">Not supported.</span></span>|
|<span data-ttu-id="87986-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="87986-117">Application</span></span>|<span data-ttu-id="87986-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87986-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87986-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87986-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87986-120">Request headers</span></span>
|<span data-ttu-id="87986-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87986-121">Header</span></span>|<span data-ttu-id="87986-122">Значение</span><span class="sxs-lookup"><span data-stu-id="87986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87986-123">Authorization</span></span>|<span data-ttu-id="87986-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87986-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87986-125">Accept</span></span>|<span data-ttu-id="87986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87986-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87986-127">Request body</span></span>
<span data-ttu-id="87986-128">В теле запроса поставляем представление JSON для объекта AndroidForWorkScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="87986-128">In the request body, supply a JSON representation for the androidForWorkScepCertificateProfile object.</span></span>

<span data-ttu-id="87986-129">В следующей таблице показаны свойства, необходимые при создании androidForWorkScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="87986-129">The following table shows the properties that are required when you create the androidForWorkScepCertificateProfile.</span></span>

|<span data-ttu-id="87986-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="87986-130">Property</span></span>|<span data-ttu-id="87986-131">Тип</span><span class="sxs-lookup"><span data-stu-id="87986-131">Type</span></span>|<span data-ttu-id="87986-132">Описание</span><span class="sxs-lookup"><span data-stu-id="87986-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87986-133">id</span><span class="sxs-lookup"><span data-stu-id="87986-133">id</span></span>|<span data-ttu-id="87986-134">Строка</span><span class="sxs-lookup"><span data-stu-id="87986-134">String</span></span>|<span data-ttu-id="87986-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87986-135">Key of the entity.</span></span> <span data-ttu-id="87986-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87986-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87986-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87986-138">DateTimeOffset</span></span>|<span data-ttu-id="87986-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="87986-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87986-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87986-141">roleScopeTagIds</span></span>|<span data-ttu-id="87986-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87986-142">String collection</span></span>|<span data-ttu-id="87986-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="87986-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87986-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87986-145">supportsScopeTags</span></span>|<span data-ttu-id="87986-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="87986-146">Boolean</span></span>|<span data-ttu-id="87986-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="87986-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87986-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="87986-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87986-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="87986-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87986-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="87986-150">This property is read-only.</span></span> <span data-ttu-id="87986-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87986-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="87986-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87986-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="87986-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87986-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="87986-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87986-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="87986-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87986-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="87986-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87986-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="87986-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87986-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="87986-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87986-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="87986-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="87986-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="87986-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87986-164">createdDateTime</span></span>|<span data-ttu-id="87986-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87986-165">DateTimeOffset</span></span>|<span data-ttu-id="87986-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="87986-166">DateTime the object was created.</span></span> <span data-ttu-id="87986-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-168">description</span><span class="sxs-lookup"><span data-stu-id="87986-168">description</span></span>|<span data-ttu-id="87986-169">Строка</span><span class="sxs-lookup"><span data-stu-id="87986-169">String</span></span>|<span data-ttu-id="87986-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87986-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87986-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-172">displayName</span><span class="sxs-lookup"><span data-stu-id="87986-172">displayName</span></span>|<span data-ttu-id="87986-173">Строка</span><span class="sxs-lookup"><span data-stu-id="87986-173">String</span></span>|<span data-ttu-id="87986-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87986-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87986-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-176">version</span><span class="sxs-lookup"><span data-stu-id="87986-176">version</span></span>|<span data-ttu-id="87986-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87986-177">Int32</span></span>|<span data-ttu-id="87986-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="87986-178">Version of the device configuration.</span></span> <span data-ttu-id="87986-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87986-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87986-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="87986-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="87986-181">Int32</span><span class="sxs-lookup"><span data-stu-id="87986-181">Int32</span></span>|<span data-ttu-id="87986-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="87986-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="87986-183">Допустимые значения от 1 до 99, унаследованные от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="87986-183">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="87986-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="87986-184">subjectNameFormat</span></span>|[<span data-ttu-id="87986-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="87986-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="87986-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="87986-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="87986-187">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="87986-187">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="87986-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="87986-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="87986-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="87986-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="87986-190">Int32</span><span class="sxs-lookup"><span data-stu-id="87986-190">Int32</span></span>|<span data-ttu-id="87986-191">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="87986-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="87986-192">Унаследованный от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="87986-192">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="87986-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="87986-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="87986-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="87986-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="87986-195">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="87986-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="87986-196">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="87986-196">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="87986-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="87986-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="87986-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="87986-198">extendedKeyUsages</span></span>|<span data-ttu-id="87986-199">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="87986-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="87986-200">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="87986-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="87986-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="87986-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="87986-202">Унаследованный от [AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="87986-202">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="87986-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="87986-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="87986-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="87986-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="87986-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="87986-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="87986-206">Наследуется [от AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="87986-206">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="87986-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="87986-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="87986-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="87986-208">scepServerUrls</span></span>|<span data-ttu-id="87986-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87986-209">String collection</span></span>|<span data-ttu-id="87986-210">URL-адрес сервера SCEP Server (s)</span><span class="sxs-lookup"><span data-stu-id="87986-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="87986-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="87986-211">subjectNameFormatString</span></span>|<span data-ttu-id="87986-212">Строка</span><span class="sxs-lookup"><span data-stu-id="87986-212">String</span></span>|<span data-ttu-id="87986-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="87986-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="87986-214">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="87986-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="87986-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="87986-215">keyUsage</span></span>|[<span data-ttu-id="87986-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="87986-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="87986-217">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="87986-217">SCEP Key Usage.</span></span> <span data-ttu-id="87986-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="87986-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="87986-219">keySize</span><span class="sxs-lookup"><span data-stu-id="87986-219">keySize</span></span>|[<span data-ttu-id="87986-220">keySize</span><span class="sxs-lookup"><span data-stu-id="87986-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="87986-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="87986-221">SCEP Key Size.</span></span> <span data-ttu-id="87986-222">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="87986-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="87986-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="87986-223">hashAlgorithm</span></span>|[<span data-ttu-id="87986-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="87986-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="87986-225">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="87986-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="87986-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="87986-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="87986-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="87986-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="87986-228">Строка</span><span class="sxs-lookup"><span data-stu-id="87986-228">String</span></span>|<span data-ttu-id="87986-229">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="87986-229">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="87986-230">certificateStore</span><span class="sxs-lookup"><span data-stu-id="87986-230">certificateStore</span></span>|[<span data-ttu-id="87986-231">certificateStore</span><span class="sxs-lookup"><span data-stu-id="87986-231">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="87986-232">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="87986-232">Target store certificate.</span></span> <span data-ttu-id="87986-233">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="87986-233">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="87986-234">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="87986-234">customSubjectAlternativeNames</span></span>|<span data-ttu-id="87986-235">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="87986-235">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="87986-236">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="87986-236">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="87986-237">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="87986-237">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="87986-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="87986-238">Response</span></span>
<span data-ttu-id="87986-239">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="87986-239">If successful, this method returns a `201 Created` response code and a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87986-240">Пример</span><span class="sxs-lookup"><span data-stu-id="87986-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="87986-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="87986-241">Request</span></span>
<span data-ttu-id="87986-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87986-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1978

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="87986-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="87986-243">Response</span></span>
<span data-ttu-id="87986-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87986-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2150

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




