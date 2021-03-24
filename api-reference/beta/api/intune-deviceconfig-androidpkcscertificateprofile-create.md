---
title: Создание androidPkcsCertificateProfile
description: Создайте новый объект AndroidPkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f4b6d34520bcfd80895c880afdb5db3c923ea16
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137870"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="f5793-103">Создание androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f5793-103">Create androidPkcsCertificateProfile</span></span>

<span data-ttu-id="f5793-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5793-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5793-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5793-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5793-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5793-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5793-107">Создайте новый [объект AndroidPkcsCertificateProfile.](../resources/intune-deviceconfig-androidpkcscertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5793-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f5793-108">Prerequisites</span></span>
<span data-ttu-id="f5793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5793-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5793-111">Permission type</span></span>|<span data-ttu-id="f5793-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5793-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5793-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5793-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5793-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5793-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5793-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5793-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5793-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5793-116">Not supported.</span></span>|
|<span data-ttu-id="f5793-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f5793-117">Application</span></span>|<span data-ttu-id="f5793-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5793-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5793-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5793-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5793-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f5793-120">Request headers</span></span>
|<span data-ttu-id="f5793-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f5793-121">Header</span></span>|<span data-ttu-id="f5793-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f5793-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5793-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5793-123">Authorization</span></span>|<span data-ttu-id="f5793-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5793-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5793-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f5793-125">Accept</span></span>|<span data-ttu-id="f5793-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5793-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5793-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5793-127">Request body</span></span>
<span data-ttu-id="f5793-128">В теле запроса поставляем представление JSON для объекта AndroidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f5793-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="f5793-129">В следующей таблице показаны свойства, необходимые при создании androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="f5793-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="f5793-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5793-130">Property</span></span>|<span data-ttu-id="f5793-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f5793-131">Type</span></span>|<span data-ttu-id="f5793-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f5793-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5793-133">id</span><span class="sxs-lookup"><span data-stu-id="f5793-133">id</span></span>|<span data-ttu-id="f5793-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-134">String</span></span>|<span data-ttu-id="f5793-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f5793-135">Key of the entity.</span></span> <span data-ttu-id="f5793-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5793-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f5793-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5793-138">DateTimeOffset</span></span>|<span data-ttu-id="f5793-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f5793-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f5793-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5793-141">roleScopeTagIds</span></span>|<span data-ttu-id="f5793-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f5793-142">String collection</span></span>|<span data-ttu-id="f5793-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="f5793-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5793-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f5793-145">supportsScopeTags</span></span>|<span data-ttu-id="f5793-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5793-146">Boolean</span></span>|<span data-ttu-id="f5793-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f5793-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f5793-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="f5793-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f5793-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f5793-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f5793-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5793-150">This property is read-only.</span></span> <span data-ttu-id="f5793-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5793-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f5793-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5793-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f5793-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f5793-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f5793-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5793-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f5793-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5793-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f5793-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f5793-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f5793-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5793-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f5793-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5793-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f5793-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f5793-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f5793-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5793-164">createdDateTime</span></span>|<span data-ttu-id="f5793-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5793-165">DateTimeOffset</span></span>|<span data-ttu-id="f5793-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f5793-166">DateTime the object was created.</span></span> <span data-ttu-id="f5793-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-168">description</span><span class="sxs-lookup"><span data-stu-id="f5793-168">description</span></span>|<span data-ttu-id="f5793-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-169">String</span></span>|<span data-ttu-id="f5793-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f5793-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5793-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f5793-172">displayName</span></span>|<span data-ttu-id="f5793-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-173">String</span></span>|<span data-ttu-id="f5793-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f5793-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5793-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-176">version</span><span class="sxs-lookup"><span data-stu-id="f5793-176">version</span></span>|<span data-ttu-id="f5793-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f5793-177">Int32</span></span>|<span data-ttu-id="f5793-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f5793-178">Version of the device configuration.</span></span> <span data-ttu-id="f5793-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5793-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5793-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="f5793-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="f5793-181">Int32</span><span class="sxs-lookup"><span data-stu-id="f5793-181">Int32</span></span>|<span data-ttu-id="f5793-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5793-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f5793-183">Допустимые значения от 1 до 99, унаследованные от [AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f5793-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f5793-184">subjectNameFormat</span></span>|[<span data-ttu-id="f5793-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f5793-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f5793-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5793-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="f5793-187">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f5793-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f5793-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f5793-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f5793-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f5793-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f5793-190">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="f5793-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5793-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f5793-192">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f5793-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="f5793-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="f5793-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f5793-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f5793-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f5793-195">Int32</span></span>|<span data-ttu-id="f5793-196">Значение для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5793-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f5793-197">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f5793-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f5793-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f5793-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f5793-199">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="f5793-200">Масштаб для срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f5793-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f5793-201">Унаследовано от [androidCertificateProfileBase.](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f5793-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f5793-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f5793-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="f5793-203">extendedKeyUsages</span></span>|<span data-ttu-id="f5793-204">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f5793-205">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="f5793-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f5793-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f5793-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f5793-207">Унаследованный от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f5793-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f5793-208">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="f5793-208">certificationAuthority</span></span>|<span data-ttu-id="f5793-209">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-209">String</span></span>|<span data-ttu-id="f5793-210">Сертификационный орган PKCS</span><span class="sxs-lookup"><span data-stu-id="f5793-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="f5793-211">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="f5793-211">certificationAuthorityName</span></span>|<span data-ttu-id="f5793-212">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-212">String</span></span>|<span data-ttu-id="f5793-213">Имя органа сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="f5793-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="f5793-214">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="f5793-214">certificateTemplateName</span></span>|<span data-ttu-id="f5793-215">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-215">String</span></span>|<span data-ttu-id="f5793-216">Имя шаблона шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="f5793-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="f5793-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f5793-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f5793-218">Строка</span><span class="sxs-lookup"><span data-stu-id="f5793-218">String</span></span>|<span data-ttu-id="f5793-219">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="f5793-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f5793-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5793-220">Response</span></span>
<span data-ttu-id="f5793-221">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f5793-221">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5793-222">Пример</span><span class="sxs-lookup"><span data-stu-id="f5793-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5793-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5793-223">Request</span></span>
<span data-ttu-id="f5793-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5793-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1731

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="f5793-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5793-225">Response</span></span>
<span data-ttu-id="f5793-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f5793-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1903

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




