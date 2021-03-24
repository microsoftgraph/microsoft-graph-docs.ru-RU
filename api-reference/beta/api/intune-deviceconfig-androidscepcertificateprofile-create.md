---
title: Создание androidScepCertificateProfile
description: Создайте новый объект AndroidScepCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 659467321509abe7662ba6c61a7f89f2ae9fa00e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137821"
---
# <a name="create-androidscepcertificateprofile"></a><span data-ttu-id="950af-103">Создание androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="950af-103">Create androidScepCertificateProfile</span></span>

<span data-ttu-id="950af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="950af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="950af-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="950af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="950af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950af-107">Создайте новый [объект AndroidScepCertificateProfile.](../resources/intune-deviceconfig-androidscepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="950af-107">Create a new [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="950af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="950af-108">Prerequisites</span></span>
<span data-ttu-id="950af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="950af-111">Permission type</span></span>|<span data-ttu-id="950af-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="950af-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="950af-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="950af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="950af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="950af-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="950af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="950af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950af-116">Not supported.</span></span>|
|<span data-ttu-id="950af-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="950af-117">Application</span></span>|<span data-ttu-id="950af-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950af-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="950af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="950af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="950af-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="950af-120">Request headers</span></span>
|<span data-ttu-id="950af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="950af-121">Header</span></span>|<span data-ttu-id="950af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="950af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="950af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="950af-123">Authorization</span></span>|<span data-ttu-id="950af-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="950af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="950af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="950af-125">Accept</span></span>|<span data-ttu-id="950af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="950af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="950af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="950af-127">Request body</span></span>
<span data-ttu-id="950af-128">В теле запроса поставляем представление JSON для объекта AndroidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="950af-128">In the request body, supply a JSON representation for the androidScepCertificateProfile object.</span></span>

<span data-ttu-id="950af-129">В следующей таблице показаны свойства, необходимые при создании androidScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="950af-129">The following table shows the properties that are required when you create the androidScepCertificateProfile.</span></span>

|<span data-ttu-id="950af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="950af-130">Property</span></span>|<span data-ttu-id="950af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="950af-131">Type</span></span>|<span data-ttu-id="950af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="950af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950af-133">id</span><span class="sxs-lookup"><span data-stu-id="950af-133">id</span></span>|<span data-ttu-id="950af-134">Строка</span><span class="sxs-lookup"><span data-stu-id="950af-134">String</span></span>|<span data-ttu-id="950af-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="950af-135">Key of the entity.</span></span> <span data-ttu-id="950af-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="950af-137">lastModifiedDateTime</span></span>|<span data-ttu-id="950af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950af-138">DateTimeOffset</span></span>|<span data-ttu-id="950af-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="950af-139">DateTime the object was last modified.</span></span> <span data-ttu-id="950af-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="950af-141">roleScopeTagIds</span></span>|<span data-ttu-id="950af-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="950af-142">String collection</span></span>|<span data-ttu-id="950af-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="950af-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="950af-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="950af-145">supportsScopeTags</span></span>|<span data-ttu-id="950af-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="950af-146">Boolean</span></span>|<span data-ttu-id="950af-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="950af-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="950af-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="950af-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="950af-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="950af-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="950af-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="950af-150">This property is read-only.</span></span> <span data-ttu-id="950af-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="950af-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="950af-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="950af-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="950af-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="950af-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="950af-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="950af-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="950af-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="950af-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="950af-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="950af-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="950af-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="950af-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="950af-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="950af-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="950af-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="950af-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="950af-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="950af-164">createdDateTime</span></span>|<span data-ttu-id="950af-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="950af-165">DateTimeOffset</span></span>|<span data-ttu-id="950af-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="950af-166">DateTime the object was created.</span></span> <span data-ttu-id="950af-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-168">description</span><span class="sxs-lookup"><span data-stu-id="950af-168">description</span></span>|<span data-ttu-id="950af-169">Строка</span><span class="sxs-lookup"><span data-stu-id="950af-169">String</span></span>|<span data-ttu-id="950af-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="950af-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="950af-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-172">displayName</span><span class="sxs-lookup"><span data-stu-id="950af-172">displayName</span></span>|<span data-ttu-id="950af-173">Строка</span><span class="sxs-lookup"><span data-stu-id="950af-173">String</span></span>|<span data-ttu-id="950af-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="950af-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="950af-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-176">version</span><span class="sxs-lookup"><span data-stu-id="950af-176">version</span></span>|<span data-ttu-id="950af-177">Int32</span><span class="sxs-lookup"><span data-stu-id="950af-177">Int32</span></span>|<span data-ttu-id="950af-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="950af-178">Version of the device configuration.</span></span> <span data-ttu-id="950af-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="950af-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="950af-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="950af-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="950af-181">Int32</span><span class="sxs-lookup"><span data-stu-id="950af-181">Int32</span></span>|<span data-ttu-id="950af-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="950af-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="950af-183">Допустимые значения от 1 до 99, унаследованные от [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="950af-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="950af-184">subjectNameFormat</span></span>|[<span data-ttu-id="950af-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="950af-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="950af-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="950af-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="950af-187">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="950af-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="950af-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="950af-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="950af-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="950af-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="950af-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="950af-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="950af-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="950af-192">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="950af-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="950af-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="950af-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="950af-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="950af-195">Int32</span><span class="sxs-lookup"><span data-stu-id="950af-195">Int32</span></span>|<span data-ttu-id="950af-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="950af-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="950af-197">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="950af-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="950af-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="950af-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="950af-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="950af-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="950af-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="950af-201">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="950af-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="950af-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="950af-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="950af-203">extendedKeyUsages</span></span>|<span data-ttu-id="950af-204">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="950af-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="950af-205">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="950af-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="950af-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="950af-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="950af-207">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="950af-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="950af-208">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="950af-208">scepServerUrls</span></span>|<span data-ttu-id="950af-209">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="950af-209">String collection</span></span>|<span data-ttu-id="950af-210">URL-адрес сервера SCEP Server (s)</span><span class="sxs-lookup"><span data-stu-id="950af-210">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="950af-211">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="950af-211">subjectNameFormatString</span></span>|<span data-ttu-id="950af-212">Строка</span><span class="sxs-lookup"><span data-stu-id="950af-212">String</span></span>|<span data-ttu-id="950af-213">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="950af-213">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="950af-214">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="950af-214">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="950af-215">keyUsage</span><span class="sxs-lookup"><span data-stu-id="950af-215">keyUsage</span></span>|[<span data-ttu-id="950af-216">keyUsages</span><span class="sxs-lookup"><span data-stu-id="950af-216">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="950af-217">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="950af-217">SCEP Key Usage.</span></span> <span data-ttu-id="950af-218">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="950af-218">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="950af-219">keySize</span><span class="sxs-lookup"><span data-stu-id="950af-219">keySize</span></span>|[<span data-ttu-id="950af-220">keySize</span><span class="sxs-lookup"><span data-stu-id="950af-220">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="950af-221">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="950af-221">SCEP Key Size.</span></span> <span data-ttu-id="950af-222">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="950af-222">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="950af-223">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="950af-223">hashAlgorithm</span></span>|[<span data-ttu-id="950af-224">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="950af-224">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="950af-225">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="950af-225">SCEP Hash Algorithm.</span></span> <span data-ttu-id="950af-226">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="950af-226">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="950af-227">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="950af-227">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="950af-228">Строка</span><span class="sxs-lookup"><span data-stu-id="950af-228">String</span></span>|<span data-ttu-id="950af-229">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="950af-229">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="950af-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="950af-230">Response</span></span>
<span data-ttu-id="950af-231">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="950af-231">If successful, this method returns a `201 Created` response code and a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950af-232">Пример</span><span class="sxs-lookup"><span data-stu-id="950af-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="950af-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="950af-233">Request</span></span>
<span data-ttu-id="950af-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="950af-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="950af-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="950af-235">Response</span></span>
<span data-ttu-id="950af-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="950af-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




