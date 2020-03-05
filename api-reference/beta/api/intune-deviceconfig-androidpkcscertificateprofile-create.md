---
title: Создание androidPkcsCertificateProfile
description: Создание нового объекта androidPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c295fba08c78676edcd24530ea965c5f300ae137
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449686"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="137bc-103">Создание androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="137bc-103">Create androidPkcsCertificateProfile</span></span>

<span data-ttu-id="137bc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="137bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="137bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="137bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="137bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="137bc-107">Создание нового объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="137bc-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="137bc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="137bc-108">Prerequisites</span></span>
<span data-ttu-id="137bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="137bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="137bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="137bc-111">Permission type</span></span>|<span data-ttu-id="137bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="137bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="137bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="137bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="137bc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="137bc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="137bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="137bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="137bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137bc-116">Not supported.</span></span>|
|<span data-ttu-id="137bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="137bc-117">Application</span></span>|<span data-ttu-id="137bc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="137bc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="137bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="137bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="137bc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="137bc-120">Request headers</span></span>
|<span data-ttu-id="137bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="137bc-121">Header</span></span>|<span data-ttu-id="137bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="137bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="137bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="137bc-123">Authorization</span></span>|<span data-ttu-id="137bc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="137bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="137bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="137bc-125">Accept</span></span>|<span data-ttu-id="137bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="137bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="137bc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="137bc-127">Request body</span></span>
<span data-ttu-id="137bc-128">В тексте запроса добавьте представление объекта androidPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="137bc-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="137bc-129">В следующей таблице приведены свойства, необходимые при создании androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="137bc-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="137bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="137bc-130">Property</span></span>|<span data-ttu-id="137bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="137bc-131">Type</span></span>|<span data-ttu-id="137bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="137bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="137bc-133">id</span><span class="sxs-lookup"><span data-stu-id="137bc-133">id</span></span>|<span data-ttu-id="137bc-134">String</span><span class="sxs-lookup"><span data-stu-id="137bc-134">String</span></span>|<span data-ttu-id="137bc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="137bc-135">Key of the entity.</span></span> <span data-ttu-id="137bc-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="137bc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="137bc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="137bc-138">DateTimeOffset</span></span>|<span data-ttu-id="137bc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="137bc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="137bc-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="137bc-141">roleScopeTagIds</span></span>|<span data-ttu-id="137bc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="137bc-142">String collection</span></span>|<span data-ttu-id="137bc-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="137bc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="137bc-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="137bc-145">supportsScopeTags</span></span>|<span data-ttu-id="137bc-146">Логический</span><span class="sxs-lookup"><span data-stu-id="137bc-146">Boolean</span></span>|<span data-ttu-id="137bc-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="137bc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="137bc-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="137bc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="137bc-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="137bc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="137bc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="137bc-150">This property is read-only.</span></span> <span data-ttu-id="137bc-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="137bc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="137bc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="137bc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="137bc-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="137bc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="137bc-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="137bc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="137bc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="137bc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="137bc-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="137bc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="137bc-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="137bc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="137bc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="137bc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="137bc-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="137bc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="137bc-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="137bc-164">createdDateTime</span></span>|<span data-ttu-id="137bc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="137bc-165">DateTimeOffset</span></span>|<span data-ttu-id="137bc-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="137bc-166">DateTime the object was created.</span></span> <span data-ttu-id="137bc-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-168">description</span><span class="sxs-lookup"><span data-stu-id="137bc-168">description</span></span>|<span data-ttu-id="137bc-169">String</span><span class="sxs-lookup"><span data-stu-id="137bc-169">String</span></span>|<span data-ttu-id="137bc-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="137bc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="137bc-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="137bc-172">displayName</span></span>|<span data-ttu-id="137bc-173">Строка</span><span class="sxs-lookup"><span data-stu-id="137bc-173">String</span></span>|<span data-ttu-id="137bc-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="137bc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="137bc-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-176">version</span><span class="sxs-lookup"><span data-stu-id="137bc-176">version</span></span>|<span data-ttu-id="137bc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="137bc-177">Int32</span></span>|<span data-ttu-id="137bc-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="137bc-178">Version of the device configuration.</span></span> <span data-ttu-id="137bc-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="137bc-180">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="137bc-180">renewalThresholdPercentage</span></span>|<span data-ttu-id="137bc-181">Int32</span><span class="sxs-lookup"><span data-stu-id="137bc-181">Int32</span></span>|<span data-ttu-id="137bc-182">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="137bc-182">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="137bc-183">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="137bc-183">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="137bc-184">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="137bc-184">subjectNameFormat</span></span>|[<span data-ttu-id="137bc-185">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="137bc-185">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="137bc-186">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="137bc-186">Certificate Subject Name Format.</span></span> <span data-ttu-id="137bc-187">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-187">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="137bc-188">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="137bc-188">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="137bc-189">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="137bc-189">subjectAlternativeNameType</span></span>|[<span data-ttu-id="137bc-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="137bc-190">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="137bc-191">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="137bc-191">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="137bc-192">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-192">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="137bc-193">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="137bc-193">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="137bc-194">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="137bc-194">certificateValidityPeriodValue</span></span>|<span data-ttu-id="137bc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="137bc-195">Int32</span></span>|<span data-ttu-id="137bc-196">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="137bc-196">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="137bc-197">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="137bc-197">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="137bc-198">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="137bc-198">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="137bc-199">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="137bc-199">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="137bc-200">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="137bc-200">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="137bc-201">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="137bc-201">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="137bc-202">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="137bc-202">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="137bc-203">екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="137bc-203">extendedKeyUsages</span></span>|<span data-ttu-id="137bc-204">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="137bc-204">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="137bc-205">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="137bc-205">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="137bc-206">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="137bc-206">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="137bc-207">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="137bc-207">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="137bc-208">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="137bc-208">certificationAuthority</span></span>|<span data-ttu-id="137bc-209">String</span><span class="sxs-lookup"><span data-stu-id="137bc-209">String</span></span>|<span data-ttu-id="137bc-210">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="137bc-210">PKCS Certification Authority</span></span>|
|<span data-ttu-id="137bc-211">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="137bc-211">certificationAuthorityName</span></span>|<span data-ttu-id="137bc-212">String</span><span class="sxs-lookup"><span data-stu-id="137bc-212">String</span></span>|<span data-ttu-id="137bc-213">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="137bc-213">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="137bc-214">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="137bc-214">certificateTemplateName</span></span>|<span data-ttu-id="137bc-215">String</span><span class="sxs-lookup"><span data-stu-id="137bc-215">String</span></span>|<span data-ttu-id="137bc-216">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="137bc-216">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="137bc-217">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="137bc-217">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="137bc-218">String</span><span class="sxs-lookup"><span data-stu-id="137bc-218">String</span></span>|<span data-ttu-id="137bc-219">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="137bc-219">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="137bc-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="137bc-220">Response</span></span>
<span data-ttu-id="137bc-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="137bc-221">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="137bc-222">Пример</span><span class="sxs-lookup"><span data-stu-id="137bc-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="137bc-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="137bc-223">Request</span></span>
<span data-ttu-id="137bc-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="137bc-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="137bc-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="137bc-225">Response</span></span>
<span data-ttu-id="137bc-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="137bc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





