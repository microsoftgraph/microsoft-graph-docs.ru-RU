---
title: Создание windows10PkcsCertificateProfile
description: Создание нового объекта windows10PkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eca0bc52b4bccb2e6e572f6b7db15949cd5748fc
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918530"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="b4a00-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b4a00-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="b4a00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4a00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4a00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4a00-106">Создание нового объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b4a00-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4a00-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4a00-107">Prerequisites</span></span>
<span data-ttu-id="b4a00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4a00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4a00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4a00-110">Permission type</span></span>|<span data-ttu-id="b4a00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4a00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4a00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4a00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4a00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4a00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4a00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4a00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4a00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a00-115">Not supported.</span></span>|
|<span data-ttu-id="b4a00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4a00-116">Application</span></span>|<span data-ttu-id="b4a00-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4a00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4a00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4a00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4a00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4a00-119">Request headers</span></span>
|<span data-ttu-id="b4a00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4a00-120">Header</span></span>|<span data-ttu-id="b4a00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4a00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4a00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4a00-122">Authorization</span></span>|<span data-ttu-id="b4a00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4a00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4a00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4a00-124">Accept</span></span>|<span data-ttu-id="b4a00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4a00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4a00-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4a00-126">Request body</span></span>
<span data-ttu-id="b4a00-127">В тексте запроса добавьте представление объекта windows10PkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4a00-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="b4a00-128">В следующей таблице приведены свойства, необходимые при создании windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="b4a00-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="b4a00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4a00-129">Property</span></span>|<span data-ttu-id="b4a00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4a00-130">Type</span></span>|<span data-ttu-id="b4a00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4a00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a00-132">id</span><span class="sxs-lookup"><span data-stu-id="b4a00-132">id</span></span>|<span data-ttu-id="b4a00-133">String</span><span class="sxs-lookup"><span data-stu-id="b4a00-133">String</span></span>|<span data-ttu-id="b4a00-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4a00-134">Key of the entity.</span></span> <span data-ttu-id="b4a00-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4a00-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b4a00-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4a00-137">DateTimeOffset</span></span>|<span data-ttu-id="b4a00-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b4a00-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b4a00-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4a00-140">roleScopeTagIds</span></span>|<span data-ttu-id="b4a00-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b4a00-141">String collection</span></span>|<span data-ttu-id="b4a00-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b4a00-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4a00-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b4a00-144">supportsScopeTags</span></span>|<span data-ttu-id="b4a00-145">Логический</span><span class="sxs-lookup"><span data-stu-id="b4a00-145">Boolean</span></span>|<span data-ttu-id="b4a00-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b4a00-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4a00-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b4a00-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4a00-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b4a00-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4a00-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4a00-149">This property is read-only.</span></span> <span data-ttu-id="b4a00-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4a00-151">createdDateTime</span></span>|<span data-ttu-id="b4a00-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4a00-152">DateTimeOffset</span></span>|<span data-ttu-id="b4a00-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b4a00-153">DateTime the object was created.</span></span> <span data-ttu-id="b4a00-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-155">description</span><span class="sxs-lookup"><span data-stu-id="b4a00-155">description</span></span>|<span data-ttu-id="b4a00-156">String</span><span class="sxs-lookup"><span data-stu-id="b4a00-156">String</span></span>|<span data-ttu-id="b4a00-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4a00-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4a00-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b4a00-159">displayName</span></span>|<span data-ttu-id="b4a00-160">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a00-160">String</span></span>|<span data-ttu-id="b4a00-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4a00-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4a00-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-163">version</span><span class="sxs-lookup"><span data-stu-id="b4a00-163">version</span></span>|<span data-ttu-id="b4a00-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b4a00-164">Int32</span></span>|<span data-ttu-id="b4a00-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4a00-165">Version of the device configuration.</span></span> <span data-ttu-id="b4a00-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4a00-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="b4a00-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="b4a00-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b4a00-168">Int32</span></span>|<span data-ttu-id="b4a00-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="b4a00-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="b4a00-170">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4a00-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4a00-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="b4a00-171">keyStorageProvider</span></span>|[<span data-ttu-id="b4a00-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="b4a00-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="b4a00-173">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b4a00-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="b4a00-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="b4a00-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4a00-175">subjectNameFormat</span></span>|[<span data-ttu-id="b4a00-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b4a00-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="b4a00-177">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b4a00-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="b4a00-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="b4a00-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4a00-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="b4a00-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="b4a00-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="b4a00-181">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b4a00-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="b4a00-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="b4a00-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="b4a00-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="b4a00-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b4a00-184">Int32</span></span>|<span data-ttu-id="b4a00-185">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b4a00-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="b4a00-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4a00-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="b4a00-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="b4a00-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="b4a00-188">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b4a00-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="b4a00-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="b4a00-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="b4a00-190">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="b4a00-190">certificationAuthority</span></span>|<span data-ttu-id="b4a00-191">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a00-191">String</span></span>|<span data-ttu-id="b4a00-192">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="b4a00-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="b4a00-193">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="b4a00-193">certificationAuthorityName</span></span>|<span data-ttu-id="b4a00-194">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a00-194">String</span></span>|<span data-ttu-id="b4a00-195">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="b4a00-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="b4a00-196">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="b4a00-196">certificateTemplateName</span></span>|<span data-ttu-id="b4a00-197">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a00-197">String</span></span>|<span data-ttu-id="b4a00-198">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="b4a00-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="b4a00-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="b4a00-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="b4a00-200">Строка</span><span class="sxs-lookup"><span data-stu-id="b4a00-200">String</span></span>|<span data-ttu-id="b4a00-201">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="b4a00-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="b4a00-202">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="b4a00-202">extendedKeyUsages</span></span>|<span data-ttu-id="b4a00-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="b4a00-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="b4a00-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="b4a00-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="b4a00-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b4a00-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b4a00-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4a00-206">Response</span></span>
<span data-ttu-id="b4a00-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4a00-207">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4a00-208">Пример</span><span class="sxs-lookup"><span data-stu-id="b4a00-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4a00-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4a00-209">Request</span></span>
<span data-ttu-id="b4a00-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a00-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1011

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b4a00-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4a00-211">Response</span></span>
<span data-ttu-id="b4a00-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4a00-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1183

{
  "@odata.type": "#microsoft.graph.windows10PkcsCertificateProfile",
  "id": "414c69c0-69c0-414c-c069-4c41c0694c41",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ]
}
```




