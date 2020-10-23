---
title: Создание windowsPhone81SCEPCertificateProfile
description: Создание нового объекта windowsPhone81SCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 921d5f90c495bbaa7bf05e30340fe786f74de87b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698878"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="c7c90-103">Создание windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c7c90-103">Create windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="c7c90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7c90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7c90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7c90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c90-107">Создание нового объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c7c90-107">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c90-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c7c90-108">Prerequisites</span></span>
<span data-ttu-id="c7c90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7c90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c90-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7c90-111">Permission type</span></span>|<span data-ttu-id="c7c90-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7c90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c90-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7c90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c90-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7c90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c90-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7c90-116">Not supported.</span></span>|
|<span data-ttu-id="c7c90-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7c90-117">Application</span></span>|<span data-ttu-id="c7c90-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c90-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c90-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7c90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c7c90-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c7c90-120">Request headers</span></span>
|<span data-ttu-id="c7c90-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7c90-121">Header</span></span>|<span data-ttu-id="c7c90-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7c90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c90-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7c90-123">Authorization</span></span>|<span data-ttu-id="c7c90-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7c90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c90-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7c90-125">Accept</span></span>|<span data-ttu-id="c7c90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c90-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7c90-127">Request body</span></span>
<span data-ttu-id="c7c90-128">В тексте запроса добавьте представление объекта windowsPhone81SCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7c90-128">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="c7c90-129">В следующей таблице приведены свойства, необходимые при создании windowsPhone81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c7c90-129">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="c7c90-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7c90-130">Property</span></span>|<span data-ttu-id="c7c90-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7c90-131">Type</span></span>|<span data-ttu-id="c7c90-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7c90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c90-133">id</span><span class="sxs-lookup"><span data-stu-id="c7c90-133">id</span></span>|<span data-ttu-id="c7c90-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c7c90-134">String</span></span>|<span data-ttu-id="c7c90-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7c90-135">Key of the entity.</span></span> <span data-ttu-id="c7c90-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c90-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c7c90-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c90-138">DateTimeOffset</span></span>|<span data-ttu-id="c7c90-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c7c90-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c7c90-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7c90-141">roleScopeTagIds</span></span>|<span data-ttu-id="c7c90-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c7c90-142">String collection</span></span>|<span data-ttu-id="c7c90-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c7c90-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c7c90-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c7c90-145">supportsScopeTags</span></span>|<span data-ttu-id="c7c90-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c7c90-146">Boolean</span></span>|<span data-ttu-id="c7c90-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c7c90-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c7c90-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c7c90-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c7c90-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c7c90-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c7c90-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c7c90-150">This property is read-only.</span></span> <span data-ttu-id="c7c90-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7c90-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c7c90-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c7c90-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c7c90-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7c90-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c7c90-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7c90-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c7c90-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c7c90-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c7c90-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7c90-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c7c90-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7c90-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c7c90-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c7c90-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c7c90-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c7c90-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c7c90-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c90-164">createdDateTime</span></span>|<span data-ttu-id="c7c90-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c90-165">DateTimeOffset</span></span>|<span data-ttu-id="c7c90-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c7c90-166">DateTime the object was created.</span></span> <span data-ttu-id="c7c90-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-168">description</span><span class="sxs-lookup"><span data-stu-id="c7c90-168">description</span></span>|<span data-ttu-id="c7c90-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c7c90-169">String</span></span>|<span data-ttu-id="c7c90-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7c90-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c7c90-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c7c90-172">displayName</span></span>|<span data-ttu-id="c7c90-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c7c90-173">String</span></span>|<span data-ttu-id="c7c90-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7c90-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c7c90-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-176">version</span><span class="sxs-lookup"><span data-stu-id="c7c90-176">version</span></span>|<span data-ttu-id="c7c90-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c7c90-177">Int32</span></span>|<span data-ttu-id="c7c90-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c7c90-178">Version of the device configuration.</span></span> <span data-ttu-id="c7c90-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c7c90-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c7c90-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="c7c90-181">Int32</span><span class="sxs-lookup"><span data-stu-id="c7c90-181">Int32</span></span>|<span data-ttu-id="c7c90-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7c90-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c7c90-183">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7c90-183">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7c90-184">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="c7c90-184">keyStorageProvider</span></span>|[<span data-ttu-id="c7c90-185">кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="c7c90-185">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c7c90-186">Поставщик хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="c7c90-186">Key Storage Provider (KSP).</span></span> <span data-ttu-id="c7c90-187">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-187">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="c7c90-188">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-188">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c7c90-189">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c7c90-189">subjectNameFormat</span></span>|[<span data-ttu-id="c7c90-190">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c7c90-190">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c7c90-191">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7c90-191">Certificate Subject Name Format.</span></span> <span data-ttu-id="c7c90-192">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-192">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="c7c90-193">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-193">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c7c90-194">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c7c90-194">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c7c90-195">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c7c90-195">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c7c90-196">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7c90-196">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c7c90-197">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-197">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="c7c90-198">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-198">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="c7c90-199">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c7c90-199">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c7c90-200">Int32</span><span class="sxs-lookup"><span data-stu-id="c7c90-200">Int32</span></span>|<span data-ttu-id="c7c90-201">Значение периода Валидтий для сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7c90-201">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="c7c90-202">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7c90-202">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7c90-203">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c7c90-203">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c7c90-204">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c7c90-204">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c7c90-205">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c7c90-205">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c7c90-206">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c7c90-206">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="c7c90-207">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-207">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c7c90-208">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c7c90-208">extendedKeyUsages</span></span>|<span data-ttu-id="c7c90-209">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c7c90-209">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c7c90-210">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c7c90-210">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c7c90-211">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c7c90-211">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c7c90-212">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c7c90-212">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="c7c90-213">сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="c7c90-213">scepServerUrls</span></span>|<span data-ttu-id="c7c90-214">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c7c90-214">String collection</span></span>|<span data-ttu-id="c7c90-215">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="c7c90-215">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="c7c90-216">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="c7c90-216">subjectNameFormatString</span></span>|<span data-ttu-id="c7c90-217">Строка</span><span class="sxs-lookup"><span data-stu-id="c7c90-217">String</span></span>|<span data-ttu-id="c7c90-218">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="c7c90-218">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="c7c90-219">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="c7c90-219">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="c7c90-220">кэйусаже</span><span class="sxs-lookup"><span data-stu-id="c7c90-220">keyUsage</span></span>|[<span data-ttu-id="c7c90-221">кэйусажес</span><span class="sxs-lookup"><span data-stu-id="c7c90-221">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="c7c90-222">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c7c90-222">SCEP Key Usage.</span></span> <span data-ttu-id="c7c90-223">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-223">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="c7c90-224">keySize</span><span class="sxs-lookup"><span data-stu-id="c7c90-224">keySize</span></span>|[<span data-ttu-id="c7c90-225">keySize</span><span class="sxs-lookup"><span data-stu-id="c7c90-225">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="c7c90-226">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="c7c90-226">SCEP Key Size.</span></span> <span data-ttu-id="c7c90-227">Возможные значения: `size1024`, `size2048`, `size4096`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-227">Possible values are: `size1024`, `size2048`, `size4096`.</span></span>|
|<span data-ttu-id="c7c90-228">хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="c7c90-228">hashAlgorithm</span></span>|[<span data-ttu-id="c7c90-229">хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="c7c90-229">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="c7c90-230">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="c7c90-230">SCEP Hash Algorithm.</span></span> <span data-ttu-id="c7c90-231">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="c7c90-231">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="c7c90-232">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c7c90-232">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c7c90-233">Строка</span><span class="sxs-lookup"><span data-stu-id="c7c90-233">String</span></span>|<span data-ttu-id="c7c90-234">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c7c90-234">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="c7c90-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7c90-235">Response</span></span>
<span data-ttu-id="c7c90-236">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7c90-236">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c90-237">Пример</span><span class="sxs-lookup"><span data-stu-id="c7c90-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c90-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7c90-238">Request</span></span>
<span data-ttu-id="c7c90-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7c90-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1805

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="c7c90-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7c90-240">Response</span></span>
<span data-ttu-id="c7c90-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7c90-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1977

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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





