---
title: Создание windows81SCEPCertificateProfile
description: Создание нового объекта windows81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c5bd467c022ac2fc41d89436eb03ddea1633f40
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48014751"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="a06d5-103">Создание windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="a06d5-103">Create windows81SCEPCertificateProfile</span></span>

<span data-ttu-id="a06d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a06d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a06d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a06d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a06d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a06d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a06d5-107">Создание нового объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a06d5-107">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a06d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a06d5-108">Prerequisites</span></span>
<span data-ttu-id="a06d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a06d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a06d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a06d5-111">Permission type</span></span>|<span data-ttu-id="a06d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a06d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a06d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a06d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a06d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a06d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a06d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a06d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a06d5-116">Not supported.</span></span>|
|<span data-ttu-id="a06d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a06d5-117">Application</span></span>|<span data-ttu-id="a06d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a06d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a06d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a06d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a06d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a06d5-120">Request headers</span></span>
|<span data-ttu-id="a06d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a06d5-121">Header</span></span>|<span data-ttu-id="a06d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a06d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a06d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a06d5-123">Authorization</span></span>|<span data-ttu-id="a06d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a06d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a06d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a06d5-125">Accept</span></span>|<span data-ttu-id="a06d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a06d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a06d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a06d5-127">Request body</span></span>
<span data-ttu-id="a06d5-128">В тексте запроса добавьте представление объекта windows81SCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a06d5-128">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="a06d5-129">В следующей таблице приведены свойства, необходимые при создании windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="a06d5-129">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="a06d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a06d5-130">Property</span></span>|<span data-ttu-id="a06d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a06d5-131">Type</span></span>|<span data-ttu-id="a06d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a06d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a06d5-133">id</span><span class="sxs-lookup"><span data-stu-id="a06d5-133">id</span></span>|<span data-ttu-id="a06d5-134">String</span><span class="sxs-lookup"><span data-stu-id="a06d5-134">String</span></span>|<span data-ttu-id="a06d5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a06d5-135">Key of the entity.</span></span> <span data-ttu-id="a06d5-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a06d5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a06d5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a06d5-138">DateTimeOffset</span></span>|<span data-ttu-id="a06d5-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a06d5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a06d5-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a06d5-141">roleScopeTagIds</span></span>|<span data-ttu-id="a06d5-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a06d5-142">String collection</span></span>|<span data-ttu-id="a06d5-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a06d5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a06d5-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a06d5-145">supportsScopeTags</span></span>|<span data-ttu-id="a06d5-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a06d5-146">Boolean</span></span>|<span data-ttu-id="a06d5-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a06d5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a06d5-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a06d5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a06d5-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a06d5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a06d5-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a06d5-150">This property is read-only.</span></span> <span data-ttu-id="a06d5-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a06d5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a06d5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a06d5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a06d5-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a06d5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a06d5-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a06d5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a06d5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a06d5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a06d5-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a06d5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a06d5-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a06d5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a06d5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a06d5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a06d5-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a06d5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a06d5-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a06d5-164">createdDateTime</span></span>|<span data-ttu-id="a06d5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a06d5-165">DateTimeOffset</span></span>|<span data-ttu-id="a06d5-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a06d5-166">DateTime the object was created.</span></span> <span data-ttu-id="a06d5-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-168">description</span><span class="sxs-lookup"><span data-stu-id="a06d5-168">description</span></span>|<span data-ttu-id="a06d5-169">String</span><span class="sxs-lookup"><span data-stu-id="a06d5-169">String</span></span>|<span data-ttu-id="a06d5-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a06d5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a06d5-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a06d5-172">displayName</span></span>|<span data-ttu-id="a06d5-173">String</span><span class="sxs-lookup"><span data-stu-id="a06d5-173">String</span></span>|<span data-ttu-id="a06d5-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a06d5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a06d5-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-176">version</span><span class="sxs-lookup"><span data-stu-id="a06d5-176">version</span></span>|<span data-ttu-id="a06d5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a06d5-177">Int32</span></span>|<span data-ttu-id="a06d5-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a06d5-178">Version of the device configuration.</span></span> <span data-ttu-id="a06d5-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a06d5-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="a06d5-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="a06d5-181">Int32</span><span class="sxs-lookup"><span data-stu-id="a06d5-181">Int32</span></span>|<span data-ttu-id="a06d5-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="a06d5-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a06d5-183">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-183">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a06d5-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="a06d5-184">keyStorageProvider</span></span>|[<span data-ttu-id="a06d5-185">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="a06d5-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="a06d5-186">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-186">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a06d5-187">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-187">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="a06d5-188">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a06d5-188">subjectNameFormat</span></span>|[<span data-ttu-id="a06d5-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a06d5-189">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="a06d5-190">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-190">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a06d5-191">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-191">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="a06d5-192">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a06d5-192">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a06d5-193">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a06d5-193">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a06d5-194">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-194">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a06d5-195">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-195">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a06d5-196">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a06d5-196">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a06d5-197">Int32</span><span class="sxs-lookup"><span data-stu-id="a06d5-197">Int32</span></span>|<span data-ttu-id="a06d5-198">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-198">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a06d5-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a06d5-199">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a06d5-200">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a06d5-200">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a06d5-201">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a06d5-201">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="a06d5-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a06d5-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="a06d5-203">extendedKeyUsages</span></span>|<span data-ttu-id="a06d5-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="a06d5-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="a06d5-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="a06d5-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a06d5-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a06d5-207">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-207">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a06d5-208">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="a06d5-208">customSubjectAlternativeNames</span></span>|<span data-ttu-id="a06d5-209">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-209">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="a06d5-210">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="a06d5-210">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="a06d5-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a06d5-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a06d5-212">Наследуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a06d5-212">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="a06d5-213">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="a06d5-213">scepServerUrls</span></span>|<span data-ttu-id="a06d5-214">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a06d5-214">String collection</span></span>|<span data-ttu-id="a06d5-215">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="a06d5-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="a06d5-216">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="a06d5-216">subjectNameFormatString</span></span>|<span data-ttu-id="a06d5-217">String</span><span class="sxs-lookup"><span data-stu-id="a06d5-217">String</span></span>|<span data-ttu-id="a06d5-218">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="a06d5-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="a06d5-219">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="a06d5-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="a06d5-220">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="a06d5-220">keyUsage</span></span>|[<span data-ttu-id="a06d5-221">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="a06d5-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="a06d5-222">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="a06d5-222">SCEP Key Usage.</span></span> <span data-ttu-id="a06d5-223">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="a06d5-224">keySize</span><span class="sxs-lookup"><span data-stu-id="a06d5-224">keySize</span></span>|[<span data-ttu-id="a06d5-225">keySize</span><span class="sxs-lookup"><span data-stu-id="a06d5-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="a06d5-226">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="a06d5-226">SCEP Key Size.</span></span> <span data-ttu-id="a06d5-227">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="a06d5-228">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="a06d5-228">hashAlgorithm</span></span>|[<span data-ttu-id="a06d5-229">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="a06d5-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="a06d5-230">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="a06d5-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="a06d5-231">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="a06d5-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="a06d5-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="a06d5-233">String</span><span class="sxs-lookup"><span data-stu-id="a06d5-233">String</span></span>|<span data-ttu-id="a06d5-234">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="a06d5-234">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="a06d5-235">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a06d5-235">certificateStore</span></span>|[<span data-ttu-id="a06d5-236">certificateStore</span><span class="sxs-lookup"><span data-stu-id="a06d5-236">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="a06d5-237">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="a06d5-237">Target store certificate.</span></span> <span data-ttu-id="a06d5-238">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="a06d5-238">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="a06d5-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="a06d5-239">Response</span></span>
<span data-ttu-id="a06d5-240">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a06d5-240">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a06d5-241">Пример</span><span class="sxs-lookup"><span data-stu-id="a06d5-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="a06d5-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="a06d5-242">Request</span></span>
<span data-ttu-id="a06d5-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a06d5-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a06d5-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="a06d5-244">Response</span></span>
<span data-ttu-id="a06d5-p125">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a06d5-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






