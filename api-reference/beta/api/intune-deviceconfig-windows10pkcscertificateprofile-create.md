---
title: Создание windows10PkcsCertificateProfile
description: Создание нового объекта windows10PkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0297eb08e3a44ab1d0746a99ddf89a2b0cb197e1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807002"
---
# <a name="create-windows10pkcscertificateprofile"></a><span data-ttu-id="c97a9-103">Создание windows10PkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c97a9-103">Create windows10PkcsCertificateProfile</span></span>

> <span data-ttu-id="c97a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c97a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c97a9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c97a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97a9-106">Создание нового объекта [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c97a9-106">Create a new [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c97a9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c97a9-107">Prerequisites</span></span>
<span data-ttu-id="c97a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c97a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c97a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c97a9-110">Permission type</span></span>|<span data-ttu-id="c97a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c97a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c97a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c97a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c97a9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c97a9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c97a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c97a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c97a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c97a9-115">Not supported.</span></span>|
|<span data-ttu-id="c97a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c97a9-116">Application</span></span>|<span data-ttu-id="c97a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c97a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c97a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c97a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c97a9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c97a9-119">Request headers</span></span>
|<span data-ttu-id="c97a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c97a9-120">Header</span></span>|<span data-ttu-id="c97a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c97a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c97a9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c97a9-122">Authorization</span></span>|<span data-ttu-id="c97a9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c97a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c97a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c97a9-124">Accept</span></span>|<span data-ttu-id="c97a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c97a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c97a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c97a9-126">Request body</span></span>
<span data-ttu-id="c97a9-127">В тексте запроса добавьте представление объекта windows10PkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c97a9-127">In the request body, supply a JSON representation for the windows10PkcsCertificateProfile object.</span></span>

<span data-ttu-id="c97a9-128">В следующей таблице приведены свойства, необходимые при создании windows10PkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="c97a9-128">The following table shows the properties that are required when you create the windows10PkcsCertificateProfile.</span></span>

|<span data-ttu-id="c97a9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c97a9-129">Property</span></span>|<span data-ttu-id="c97a9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c97a9-130">Type</span></span>|<span data-ttu-id="c97a9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c97a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97a9-132">id</span><span class="sxs-lookup"><span data-stu-id="c97a9-132">id</span></span>|<span data-ttu-id="c97a9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a9-133">String</span></span>|<span data-ttu-id="c97a9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c97a9-134">Key of the entity.</span></span> <span data-ttu-id="c97a9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c97a9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c97a9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c97a9-137">DateTimeOffset</span></span>|<span data-ttu-id="c97a9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c97a9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c97a9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c97a9-140">roleScopeTagIds</span></span>|<span data-ttu-id="c97a9-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c97a9-141">String collection</span></span>|<span data-ttu-id="c97a9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c97a9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c97a9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c97a9-144">supportsScopeTags</span></span>|<span data-ttu-id="c97a9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c97a9-145">Boolean</span></span>|<span data-ttu-id="c97a9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c97a9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c97a9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c97a9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c97a9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c97a9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c97a9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c97a9-149">This property is read-only.</span></span> <span data-ttu-id="c97a9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c97a9-151">createdDateTime</span></span>|<span data-ttu-id="c97a9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c97a9-152">DateTimeOffset</span></span>|<span data-ttu-id="c97a9-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c97a9-153">DateTime the object was created.</span></span> <span data-ttu-id="c97a9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-155">description</span><span class="sxs-lookup"><span data-stu-id="c97a9-155">description</span></span>|<span data-ttu-id="c97a9-156">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-156">String</span></span>|<span data-ttu-id="c97a9-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c97a9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c97a9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c97a9-159">displayName</span></span>|<span data-ttu-id="c97a9-160">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-160">String</span></span>|<span data-ttu-id="c97a9-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c97a9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c97a9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-163">version</span><span class="sxs-lookup"><span data-stu-id="c97a9-163">version</span></span>|<span data-ttu-id="c97a9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c97a9-164">Int32</span></span>|<span data-ttu-id="c97a9-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c97a9-165">Version of the device configuration.</span></span> <span data-ttu-id="c97a9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c97a9-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c97a9-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c97a9-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c97a9-168">Int32</span></span>|<span data-ttu-id="c97a9-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c97a9-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c97a9-170">Допустимые значения — от 1 до 99, наСледуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c97a9-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c97a9-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="c97a9-171">keyStorageProvider</span></span>|[<span data-ttu-id="c97a9-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="c97a9-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="c97a9-173">Поставщик хранилища ключей (KSP), наСледуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c97a9-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="c97a9-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="c97a9-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c97a9-175">subjectNameFormat</span></span>|[<span data-ttu-id="c97a9-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c97a9-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="c97a9-177">Формат имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c97a9-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="c97a9-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="c97a9-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c97a9-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c97a9-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c97a9-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c97a9-181">Тип альтернативного имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c97a9-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c97a9-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c97a9-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c97a9-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c97a9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c97a9-184">Int32</span></span>|<span data-ttu-id="c97a9-185">Значение срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c97a9-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c97a9-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c97a9-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c97a9-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c97a9-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c97a9-188">Масштаб срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c97a9-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="c97a9-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c97a9-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c97a9-190">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="c97a9-190">certificationAuthority</span></span>|<span data-ttu-id="c97a9-191">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-191">String</span></span>|<span data-ttu-id="c97a9-192">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c97a9-192">PKCS Certification Authority</span></span>|
|<span data-ttu-id="c97a9-193">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="c97a9-193">certificationAuthorityName</span></span>|<span data-ttu-id="c97a9-194">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-194">String</span></span>|<span data-ttu-id="c97a9-195">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="c97a9-195">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="c97a9-196">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="c97a9-196">certificateTemplateName</span></span>|<span data-ttu-id="c97a9-197">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-197">String</span></span>|<span data-ttu-id="c97a9-198">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="c97a9-198">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="c97a9-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="c97a9-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="c97a9-200">String</span><span class="sxs-lookup"><span data-stu-id="c97a9-200">String</span></span>|<span data-ttu-id="c97a9-201">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="c97a9-201">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="c97a9-202">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="c97a9-202">extendedKeyUsages</span></span>|<span data-ttu-id="c97a9-203">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="c97a9-203">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="c97a9-204">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="c97a9-204">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="c97a9-205">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c97a9-205">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c97a9-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="c97a9-206">Response</span></span>
<span data-ttu-id="c97a9-207">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c97a9-207">If successful, this method returns a `201 Created` response code and a [windows10PkcsCertificateProfile](../resources/intune-deviceconfig-windows10pkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c97a9-208">Пример</span><span class="sxs-lookup"><span data-stu-id="c97a9-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="c97a9-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="c97a9-209">Request</span></span>
<span data-ttu-id="c97a9-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c97a9-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c97a9-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="c97a9-211">Response</span></span>
<span data-ttu-id="c97a9-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c97a9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





