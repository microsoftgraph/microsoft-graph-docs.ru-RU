---
title: Создание windows81SCEPCertificateProfile
description: Создайте новый объект Windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2b86004894978eb8e5eb6db6dd58b99e9486c23e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147338"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="b8e0f-103">Создание windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b8e0f-103">Create windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="b8e0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8e0f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8e0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e0f-107">Создайте [новый объект Windows81SCEPCertificateProfile.](../resources/intune-deviceconfig-windows81scepcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8e0f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8e0f-108">Prerequisites</span></span>
<span data-ttu-id="b8e0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8e0f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8e0f-111">Permission type</span></span>|<span data-ttu-id="b8e0f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8e0f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8e0f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e0f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8e0f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8e0f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-116">Not supported.</span></span>|
|<span data-ttu-id="b8e0f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8e0f-117">Application</span></span>|<span data-ttu-id="b8e0f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8e0f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8e0f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8e0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8e0f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b8e0f-120">Request headers</span></span>
|<span data-ttu-id="b8e0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8e0f-121">Header</span></span>|<span data-ttu-id="b8e0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b8e0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8e0f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8e0f-123">Authorization</span></span>|<span data-ttu-id="b8e0f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8e0f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b8e0f-125">Accept</span></span>|<span data-ttu-id="b8e0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8e0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8e0f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8e0f-127">Request body</span></span>
<span data-ttu-id="b8e0f-128">В теле запроса поставляем представление JSON для объекта Windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="b8e0f-129">В следующей таблице показаны свойства, необходимые при создании windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="b8e0f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8e0f-130">Property</span></span>|<span data-ttu-id="b8e0f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b8e0f-131">Type</span></span>|<span data-ttu-id="b8e0f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b8e0f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e0f-133">id</span><span class="sxs-lookup"><span data-stu-id="b8e0f-133">id</span></span>|<span data-ttu-id="b8e0f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b8e0f-134">String</span></span>|<span data-ttu-id="b8e0f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-135">Key of the entity.</span></span> <span data-ttu-id="b8e0f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8e0f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8e0f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8e0f-138">DateTimeOffset</span></span>|<span data-ttu-id="b8e0f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8e0f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8e0f-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8e0f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b8e0f-142">String collection</span></span>|<span data-ttu-id="b8e0f-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8e0f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8e0f-145">supportsScopeTags</span></span>|<span data-ttu-id="b8e0f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8e0f-146">Boolean</span></span>|<span data-ttu-id="b8e0f-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8e0f-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8e0f-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8e0f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-150">This property is read-only.</span></span> <span data-ttu-id="b8e0f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8e0f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b8e0f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8e0f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b8e0f-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b8e0f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8e0f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b8e0f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8e0f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b8e0f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b8e0f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8e0f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b8e0f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8e0f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b8e0f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b8e0f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8e0f-164">createdDateTime</span></span>|<span data-ttu-id="b8e0f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8e0f-165">DateTimeOffset</span></span>|<span data-ttu-id="b8e0f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-166">DateTime the object was created.</span></span> <span data-ttu-id="b8e0f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-168">description</span><span class="sxs-lookup"><span data-stu-id="b8e0f-168">description</span></span>|<span data-ttu-id="b8e0f-169">Строка</span><span class="sxs-lookup"><span data-stu-id="b8e0f-169">String</span></span>|<span data-ttu-id="b8e0f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8e0f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b8e0f-172">displayName</span></span>|<span data-ttu-id="b8e0f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b8e0f-173">String</span></span>|<span data-ttu-id="b8e0f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8e0f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-176">version</span><span class="sxs-lookup"><span data-stu-id="b8e0f-176">version</span></span>|<span data-ttu-id="b8e0f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e0f-177">Int32</span></span>|<span data-ttu-id="b8e0f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-178">Version of the device configuration.</span></span> <span data-ttu-id="b8e0f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8e0f-180">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="b8e0f-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="b8e0f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e0f-181">Int32</span></span>|<span data-ttu-id="b8e0f-182">Процент порогового значения обновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b8e0f-183">Допустимые значения от 1 до 99, унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8e0f-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="b8e0f-184">keyStorageProvider</span></span>|[<span data-ttu-id="b8e0f-185">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="b8e0f-185">keyStorageProviderOption</span></span>](../resources/intune-shared-keystorageprovideroption.md)|<span data-ttu-id="b8e0f-186">Поставщик ключей для хранения данных (KSP), унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b8e0f-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b8e0f-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b8e0f-188">subjectNameFormat</span></span>|[<span data-ttu-id="b8e0f-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b8e0f-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b8e0f-190">Формат имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b8e0f-191">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b8e0f-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b8e0f-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b8e0f-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b8e0f-193">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="b8e0f-194">Тип альтернативного имени субъекта сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b8e0f-195">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="b8e0f-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b8e0f-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b8e0f-197">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e0f-197">Int32</span></span>|<span data-ttu-id="b8e0f-198">Значение для периода действия сертификата, унаследованной от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8e0f-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b8e0f-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b8e0f-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b8e0f-200">certificateValidityPeriodScale</span></span>](../resources/intune-shared-certificatevalidityperiodscale.md)|<span data-ttu-id="b8e0f-201">Масштабировать период действия сертификата, унаследованный от [windowsCertificateProfileBase.](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b8e0f-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b8e0f-203">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="b8e0f-203">extendedKeyUsages</span></span>|<span data-ttu-id="b8e0f-204">[расширенная коллекцияKeyUsage](../resources/intune-shared-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-204">[extendedKeyUsage](../resources/intune-shared-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b8e0f-205">Параметры расширенного использования ключей (EKU).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b8e0f-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b8e0f-207">Унаследованный от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8e0f-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="b8e0f-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="b8e0f-209">[коллекция customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="b8e0f-210">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="b8e0f-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b8e0f-212">Унаследованный от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b8e0f-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="b8e0f-213">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="b8e0f-213">scepServerUrls</span></span>|<span data-ttu-id="b8e0f-214">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b8e0f-214">String collection</span></span>|<span data-ttu-id="b8e0f-215">URL-адрес сервера SCEP Server (s).</span><span class="sxs-lookup"><span data-stu-id="b8e0f-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="b8e0f-216">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b8e0f-216">subjectNameFormatString</span></span>|<span data-ttu-id="b8e0f-217">Строка</span><span class="sxs-lookup"><span data-stu-id="b8e0f-217">String</span></span>|<span data-ttu-id="b8e0f-218">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="b8e0f-219">Пример: CN={{EmailAddress}},E={EmailAddress}},OU=Enterprise Users,O=Contoso Corporation, L=Redmond,ST=WA,C=US</span><span class="sxs-lookup"><span data-stu-id="b8e0f-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="b8e0f-220">keyUsage</span><span class="sxs-lookup"><span data-stu-id="b8e0f-220">keyUsage</span></span>|[<span data-ttu-id="b8e0f-221">keyUsages</span><span class="sxs-lookup"><span data-stu-id="b8e0f-221">keyUsages</span></span>](../resources/intune-shared-keyusages.md)|<span data-ttu-id="b8e0f-222">Использование ключей SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-222">SCEP Key Usage.</span></span> <span data-ttu-id="b8e0f-223">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="b8e0f-224">keySize</span><span class="sxs-lookup"><span data-stu-id="b8e0f-224">keySize</span></span>|[<span data-ttu-id="b8e0f-225">keySize</span><span class="sxs-lookup"><span data-stu-id="b8e0f-225">keySize</span></span>](../resources/intune-shared-keysize.md)|<span data-ttu-id="b8e0f-226">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-226">SCEP Key Size.</span></span> <span data-ttu-id="b8e0f-227">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="b8e0f-228">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b8e0f-228">hashAlgorithm</span></span>|[<span data-ttu-id="b8e0f-229">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="b8e0f-229">hashAlgorithms</span></span>](../resources/intune-shared-hashalgorithms.md)|<span data-ttu-id="b8e0f-230">Алгоритм хаширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="b8e0f-231">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="b8e0f-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b8e0f-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b8e0f-233">Строка</span><span class="sxs-lookup"><span data-stu-id="b8e0f-233">String</span></span>|<span data-ttu-id="b8e0f-234">Настраиваемая строка, определяемая атрибутом AAD.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b8e0f-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b8e0f-235">certificateStore</span></span>|[<span data-ttu-id="b8e0f-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="b8e0f-236">certificateStore</span></span>](../resources/intune-shared-certificatestore.md)|<span data-ttu-id="b8e0f-237">Сертификат целевого магазина.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-237">Target store certificate.</span></span> <span data-ttu-id="b8e0f-238">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="b8e0f-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8e0f-239">Response</span></span>
<span data-ttu-id="b8e0f-240">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект Windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-240">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8e0f-241">Пример</span><span class="sxs-lookup"><span data-stu-id="b8e0f-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8e0f-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8e0f-242">Request</span></span>
<span data-ttu-id="b8e0f-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2024

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```

### <a name="response"></a><span data-ttu-id="b8e0f-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8e0f-244">Response</span></span>
<span data-ttu-id="b8e0f-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8e0f-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2196

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine"
}
```




