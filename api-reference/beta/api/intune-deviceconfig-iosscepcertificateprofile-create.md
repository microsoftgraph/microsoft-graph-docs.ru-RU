---
title: Создание iosScepCertificateProfile
description: Создайте новый объект iosScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 297e2ca51b4df2735065d4ca556a8ba1d0c94ece
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441643"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="8ae27-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8ae27-103">Create iosScepCertificateProfile</span></span>

<span data-ttu-id="8ae27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ae27-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ae27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ae27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae27-107">Создайте новый [объект iosScepCertificateProfile.](../resources/intune-deviceconfig-iosscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8ae27-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ae27-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8ae27-108">Prerequisites</span></span>
<span data-ttu-id="8ae27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae27-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ae27-111">Permission type</span></span>|<span data-ttu-id="8ae27-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ae27-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae27-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ae27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae27-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ae27-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ae27-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ae27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae27-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ae27-116">Not supported.</span></span>|
|<span data-ttu-id="8ae27-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ae27-117">Application</span></span>|<span data-ttu-id="8ae27-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ae27-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae27-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ae27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ae27-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8ae27-120">Request headers</span></span>
|<span data-ttu-id="8ae27-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ae27-121">Header</span></span>|<span data-ttu-id="8ae27-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8ae27-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae27-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae27-123">Authorization</span></span>|<span data-ttu-id="8ae27-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ae27-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae27-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ae27-125">Accept</span></span>|<span data-ttu-id="8ae27-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae27-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae27-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ae27-127">Request body</span></span>
<span data-ttu-id="8ae27-128">В теле запроса поставляем представление JSON для объекта iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8ae27-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="8ae27-129">В следующей таблице показаны свойства, необходимые при создании iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8ae27-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="8ae27-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ae27-130">Property</span></span>|<span data-ttu-id="8ae27-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8ae27-131">Type</span></span>|<span data-ttu-id="8ae27-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae27-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae27-133">id</span><span class="sxs-lookup"><span data-stu-id="8ae27-133">id</span></span>|<span data-ttu-id="8ae27-134">String</span><span class="sxs-lookup"><span data-stu-id="8ae27-134">String</span></span>|<span data-ttu-id="8ae27-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae27-135">Key of the entity.</span></span> <span data-ttu-id="8ae27-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae27-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ae27-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae27-138">DateTimeOffset</span></span>|<span data-ttu-id="8ae27-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae27-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ae27-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ae27-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ae27-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8ae27-142">String collection</span></span>|<span data-ttu-id="8ae27-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="8ae27-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ae27-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ae27-145">supportsScopeTags</span></span>|<span data-ttu-id="8ae27-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ae27-146">Boolean</span></span>|<span data-ttu-id="8ae27-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8ae27-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ae27-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="8ae27-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ae27-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8ae27-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ae27-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ae27-150">This property is read-only.</span></span> <span data-ttu-id="8ae27-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ae27-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ae27-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ae27-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ae27-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ae27-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ae27-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ae27-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ae27-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ae27-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ae27-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ae27-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ae27-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ae27-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ae27-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ae27-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ae27-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ae27-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ae27-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ae27-164">createdDateTime</span></span>|<span data-ttu-id="8ae27-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ae27-165">DateTimeOffset</span></span>|<span data-ttu-id="8ae27-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ae27-166">DateTime the object was created.</span></span> <span data-ttu-id="8ae27-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-168">description</span><span class="sxs-lookup"><span data-stu-id="8ae27-168">description</span></span>|<span data-ttu-id="8ae27-169">String</span><span class="sxs-lookup"><span data-stu-id="8ae27-169">String</span></span>|<span data-ttu-id="8ae27-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae27-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ae27-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8ae27-172">displayName</span></span>|<span data-ttu-id="8ae27-173">String</span><span class="sxs-lookup"><span data-stu-id="8ae27-173">String</span></span>|<span data-ttu-id="8ae27-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae27-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ae27-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-176">version</span><span class="sxs-lookup"><span data-stu-id="8ae27-176">version</span></span>|<span data-ttu-id="8ae27-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae27-177">Int32</span></span>|<span data-ttu-id="8ae27-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ae27-178">Version of the device configuration.</span></span> <span data-ttu-id="8ae27-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ae27-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="8ae27-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="8ae27-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae27-181">Int32</span></span>|<span data-ttu-id="8ae27-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ae27-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8ae27-183">Допустимые значения от 1 до 99, унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8ae27-183">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8ae27-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8ae27-184">subjectNameFormat</span></span>|[<span data-ttu-id="8ae27-185">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8ae27-185">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="8ae27-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ae27-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="8ae27-187">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-187">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8ae27-188">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-188">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="8ae27-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8ae27-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8ae27-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8ae27-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="8ae27-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ae27-191">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="8ae27-192">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-192">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8ae27-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="8ae27-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8ae27-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8ae27-195">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae27-195">Int32</span></span>|<span data-ttu-id="8ae27-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ae27-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="8ae27-197">Унаследованный от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8ae27-197">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8ae27-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8ae27-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8ae27-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8ae27-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="8ae27-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="8ae27-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="8ae27-201">Наследуется [от iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8ae27-201">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="8ae27-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8ae27-203">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="8ae27-203">scepServerUrls</span></span>|<span data-ttu-id="8ae27-204">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8ae27-204">String collection</span></span>|<span data-ttu-id="8ae27-205">URL-адрес сервера SCEP Server (s).</span><span class="sxs-lookup"><span data-stu-id="8ae27-205">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="8ae27-206">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8ae27-206">subjectNameFormatString</span></span>|<span data-ttu-id="8ae27-207">String</span><span class="sxs-lookup"><span data-stu-id="8ae27-207">String</span></span>|<span data-ttu-id="8ae27-208">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="8ae27-208">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8ae27-209">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="8ae27-209">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8ae27-210">keyUsage</span><span class="sxs-lookup"><span data-stu-id="8ae27-210">keyUsage</span></span>|[<span data-ttu-id="8ae27-211">keyUsages</span><span class="sxs-lookup"><span data-stu-id="8ae27-211">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="8ae27-212">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="8ae27-212">SCEP Key Usage.</span></span> <span data-ttu-id="8ae27-213">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-213">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="8ae27-214">keySize</span><span class="sxs-lookup"><span data-stu-id="8ae27-214">keySize</span></span>|[<span data-ttu-id="8ae27-215">keySize</span><span class="sxs-lookup"><span data-stu-id="8ae27-215">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="8ae27-216">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="8ae27-216">SCEP Key Size.</span></span> <span data-ttu-id="8ae27-217">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-217">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="8ae27-218">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="8ae27-218">extendedKeyUsages</span></span>|<span data-ttu-id="8ae27-219">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="8ae27-219">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8ae27-220">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="8ae27-220">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8ae27-221">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ae27-221">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ae27-222">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8ae27-222">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8ae27-223">String</span><span class="sxs-lookup"><span data-stu-id="8ae27-223">String</span></span>|<span data-ttu-id="8ae27-224">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="8ae27-224">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8ae27-225">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8ae27-225">certificateStore</span></span>|[<span data-ttu-id="8ae27-226">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8ae27-226">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="8ae27-227">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="8ae27-227">Target store certificate.</span></span> <span data-ttu-id="8ae27-228">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="8ae27-228">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="8ae27-229">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8ae27-229">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8ae27-230">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="8ae27-230">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8ae27-231">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="8ae27-231">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="8ae27-232">Переменная OnPremisesUserPrincipalName является поддержкой, а также другими, задокументированными здесь: http://go.microsoft.com/fwlink/?LinkId=2027630 .</span><span class="sxs-lookup"><span data-stu-id="8ae27-232">The OnPremisesUserPrincipalName variable is support as well as others documented here: http://go.microsoft.com/fwlink/?LinkId=2027630.</span></span> <span data-ttu-id="8ae27-233">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ae27-233">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8ae27-234">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ae27-234">Response</span></span>
<span data-ttu-id="8ae27-235">В случае успеха этот метод возвращает код отклика и `201 Created` [объект iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8ae27-235">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae27-236">Пример</span><span class="sxs-lookup"><span data-stu-id="8ae27-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ae27-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ae27-237">Request</span></span>
<span data-ttu-id="8ae27-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ae27-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1932

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="8ae27-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ae27-239">Response</span></span>
<span data-ttu-id="8ae27-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ae27-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2104

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
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




