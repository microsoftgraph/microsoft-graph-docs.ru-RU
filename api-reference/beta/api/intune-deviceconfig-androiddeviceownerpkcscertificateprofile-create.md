---
title: Создание androidDeviceOwnerPkcsCertificateProfile
description: Создайте новый объект androidDeviceOwnerPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 455bbec4eaabc4945e9b36451ceb70483aa8dd04
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128455"
---
# <a name="create-androiddeviceownerpkcscertificateprofile"></a><span data-ttu-id="4255f-103">Создание androidDeviceOwnerPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="4255f-103">Create androidDeviceOwnerPkcsCertificateProfile</span></span>

<span data-ttu-id="4255f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4255f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4255f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4255f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4255f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4255f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4255f-107">Создайте новый [объект androidDeviceOwnerPkcsCertificateProfile.](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-107">Create a new [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4255f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4255f-108">Prerequisites</span></span>
<span data-ttu-id="4255f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4255f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4255f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4255f-111">Permission type</span></span>|<span data-ttu-id="4255f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4255f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4255f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4255f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4255f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4255f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4255f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4255f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4255f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4255f-116">Not supported.</span></span>|
|<span data-ttu-id="4255f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4255f-117">Application</span></span>|<span data-ttu-id="4255f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4255f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4255f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4255f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4255f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4255f-120">Request headers</span></span>
|<span data-ttu-id="4255f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4255f-121">Header</span></span>|<span data-ttu-id="4255f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4255f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4255f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4255f-123">Authorization</span></span>|<span data-ttu-id="4255f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4255f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4255f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4255f-125">Accept</span></span>|<span data-ttu-id="4255f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4255f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4255f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4255f-127">Request body</span></span>
<span data-ttu-id="4255f-128">В теле запроса поставляем представление JSON для объекта AndroidDeviceOwnerPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4255f-128">In the request body, supply a JSON representation for the androidDeviceOwnerPkcsCertificateProfile object.</span></span>

<span data-ttu-id="4255f-129">В следующей таблице показаны свойства, необходимые при создании androidDeviceOwnerPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="4255f-129">The following table shows the properties that are required when you create the androidDeviceOwnerPkcsCertificateProfile.</span></span>

|<span data-ttu-id="4255f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4255f-130">Property</span></span>|<span data-ttu-id="4255f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4255f-131">Type</span></span>|<span data-ttu-id="4255f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4255f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4255f-133">id</span><span class="sxs-lookup"><span data-stu-id="4255f-133">id</span></span>|<span data-ttu-id="4255f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-134">String</span></span>|<span data-ttu-id="4255f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4255f-135">Key of the entity.</span></span> <span data-ttu-id="4255f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4255f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4255f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4255f-138">DateTimeOffset</span></span>|<span data-ttu-id="4255f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4255f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4255f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4255f-141">roleScopeTagIds</span></span>|<span data-ttu-id="4255f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4255f-142">String collection</span></span>|<span data-ttu-id="4255f-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4255f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4255f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4255f-145">supportsScopeTags</span></span>|<span data-ttu-id="4255f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4255f-146">Boolean</span></span>|<span data-ttu-id="4255f-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4255f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4255f-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="4255f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4255f-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4255f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4255f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4255f-150">This property is read-only.</span></span> <span data-ttu-id="4255f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4255f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4255f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4255f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4255f-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4255f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4255f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4255f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4255f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4255f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4255f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4255f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4255f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4255f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4255f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4255f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4255f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4255f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4255f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4255f-164">createdDateTime</span></span>|<span data-ttu-id="4255f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4255f-165">DateTimeOffset</span></span>|<span data-ttu-id="4255f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4255f-166">DateTime the object was created.</span></span> <span data-ttu-id="4255f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-168">description</span><span class="sxs-lookup"><span data-stu-id="4255f-168">description</span></span>|<span data-ttu-id="4255f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-169">String</span></span>|<span data-ttu-id="4255f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4255f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4255f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4255f-172">displayName</span></span>|<span data-ttu-id="4255f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-173">String</span></span>|<span data-ttu-id="4255f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4255f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4255f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-176">version</span><span class="sxs-lookup"><span data-stu-id="4255f-176">version</span></span>|<span data-ttu-id="4255f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4255f-177">Int32</span></span>|<span data-ttu-id="4255f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4255f-178">Version of the device configuration.</span></span> <span data-ttu-id="4255f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4255f-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="4255f-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="4255f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4255f-181">Int32</span></span>|<span data-ttu-id="4255f-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="4255f-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="4255f-183">Допустимые значения от 1 до 99, унаследованные от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-183">Valid values 1 to 99 Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4255f-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4255f-184">subjectNameFormat</span></span>|[<span data-ttu-id="4255f-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="4255f-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="4255f-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="4255f-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="4255f-187">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-187">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="4255f-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="4255f-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="4255f-189">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="4255f-189">certificateValidityPeriodValue</span></span>|<span data-ttu-id="4255f-190">Int32</span><span class="sxs-lookup"><span data-stu-id="4255f-190">Int32</span></span>|<span data-ttu-id="4255f-191">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="4255f-191">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="4255f-192">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-192">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4255f-193">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4255f-193">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="4255f-194">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="4255f-194">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="4255f-195">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="4255f-195">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="4255f-196">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-196">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="4255f-197">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="4255f-197">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="4255f-198">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="4255f-198">extendedKeyUsages</span></span>|<span data-ttu-id="4255f-199">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-199">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="4255f-200">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="4255f-200">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="4255f-201">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4255f-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4255f-202">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-202">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)</span></span>|
|<span data-ttu-id="4255f-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4255f-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="4255f-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="4255f-204">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="4255f-205">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="4255f-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="4255f-206">Унаследованный от [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="4255f-206">Inherited from [androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md).</span></span> <span data-ttu-id="4255f-207">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="4255f-207">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="4255f-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="4255f-208">certificationAuthority</span></span>|<span data-ttu-id="4255f-209">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-209">String</span></span>|<span data-ttu-id="4255f-210">Сертификационный орган PKCS</span><span class="sxs-lookup"><span data-stu-id="4255f-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="4255f-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="4255f-211">certificationAuthorityName</span></span>|<span data-ttu-id="4255f-212">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-212">String</span></span>|<span data-ttu-id="4255f-213">Имя органа сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="4255f-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="4255f-214">certificationAuthorityType</span><span class="sxs-lookup"><span data-stu-id="4255f-214">certificationAuthorityType</span></span>|[<span data-ttu-id="4255f-215">deviceManagementCertificationAuthority</span><span class="sxs-lookup"><span data-stu-id="4255f-215">deviceManagementCertificationAuthority</span></span>](../resources/intune-deviceconfig-devicemanagementcertificationauthority.md)|<span data-ttu-id="4255f-216">Тип органа сертификации.</span><span class="sxs-lookup"><span data-stu-id="4255f-216">Certification authority type.</span></span> <span data-ttu-id="4255f-217">Возможные значения: `notConfigured`, `microsoft`, `digiCert`.</span><span class="sxs-lookup"><span data-stu-id="4255f-217">Possible values are: `notConfigured`, `microsoft`, `digiCert`.</span></span>|
|<span data-ttu-id="4255f-218">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="4255f-218">certificateTemplateName</span></span>|<span data-ttu-id="4255f-219">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-219">String</span></span>|<span data-ttu-id="4255f-220">Имя шаблона шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="4255f-220">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="4255f-221">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4255f-221">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="4255f-222">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-222">String</span></span>|<span data-ttu-id="4255f-223">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="4255f-223">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="4255f-224">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="4255f-224">subjectNameFormatString</span></span>|<span data-ttu-id="4255f-225">Строка</span><span class="sxs-lookup"><span data-stu-id="4255f-225">String</span></span>|<span data-ttu-id="4255f-226">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="4255f-226">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="4255f-227">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="4255f-227">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="4255f-228">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4255f-228">certificateStore</span></span>|[<span data-ttu-id="4255f-229">certificateStore</span><span class="sxs-lookup"><span data-stu-id="4255f-229">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="4255f-230">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="4255f-230">Target store certificate.</span></span> <span data-ttu-id="4255f-231">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="4255f-231">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="4255f-232">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="4255f-232">customSubjectAlternativeNames</span></span>|<span data-ttu-id="4255f-233">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="4255f-233">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="4255f-234">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="4255f-234">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="4255f-235">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4255f-235">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4255f-236">Ответ</span><span class="sxs-lookup"><span data-stu-id="4255f-236">Response</span></span>
<span data-ttu-id="4255f-237">В случае успеха этот метод возвращает код отклика и `201 Created` [объект androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4255f-237">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerPkcsCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4255f-238">Пример</span><span class="sxs-lookup"><span data-stu-id="4255f-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="4255f-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="4255f-239">Request</span></span>
<span data-ttu-id="4255f-240">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4255f-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2078

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificationAuthorityType": "microsoft",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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

### <a name="response"></a><span data-ttu-id="4255f-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="4255f-241">Response</span></span>
<span data-ttu-id="4255f-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4255f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2250

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerPkcsCertificateProfile",
  "id": "5e86a0e6-a0e6-5e86-e6a0-865ee6a0865e",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificationAuthorityType": "microsoft",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
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




