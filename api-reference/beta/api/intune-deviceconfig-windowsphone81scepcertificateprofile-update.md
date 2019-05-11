---
title: Обновление windowsPhone81SCEPCertificateProfile
description: Обновление свойств объекта windowsPhone81SCEPCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b5761b0376ca62c64bfaa582a1384773f062297
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917648"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="ee522-103">Обновление windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ee522-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="ee522-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee522-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee522-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee522-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee522-106">Обновление свойств объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ee522-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee522-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee522-107">Prerequisites</span></span>
<span data-ttu-id="ee522-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee522-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee522-110">Permission type</span></span>|<span data-ttu-id="ee522-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee522-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee522-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee522-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee522-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee522-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee522-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee522-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee522-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee522-115">Not supported.</span></span>|
|<span data-ttu-id="ee522-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee522-116">Application</span></span>|<span data-ttu-id="ee522-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee522-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee522-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee522-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee522-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee522-119">Request headers</span></span>
|<span data-ttu-id="ee522-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee522-120">Header</span></span>|<span data-ttu-id="ee522-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee522-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee522-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee522-122">Authorization</span></span>|<span data-ttu-id="ee522-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee522-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee522-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee522-124">Accept</span></span>|<span data-ttu-id="ee522-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee522-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee522-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee522-126">Request body</span></span>
<span data-ttu-id="ee522-127">В тексте запроса добавьте представление объекта [WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee522-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="ee522-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="ee522-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee522-129">Property</span></span>|<span data-ttu-id="ee522-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ee522-130">Type</span></span>|<span data-ttu-id="ee522-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee522-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee522-132">id</span><span class="sxs-lookup"><span data-stu-id="ee522-132">id</span></span>|<span data-ttu-id="ee522-133">String</span><span class="sxs-lookup"><span data-stu-id="ee522-133">String</span></span>|<span data-ttu-id="ee522-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ee522-134">Key of the entity.</span></span> <span data-ttu-id="ee522-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee522-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ee522-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee522-137">DateTimeOffset</span></span>|<span data-ttu-id="ee522-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ee522-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ee522-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ee522-140">roleScopeTagIds</span></span>|<span data-ttu-id="ee522-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ee522-141">String collection</span></span>|<span data-ttu-id="ee522-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ee522-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ee522-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ee522-144">supportsScopeTags</span></span>|<span data-ttu-id="ee522-145">Логический</span><span class="sxs-lookup"><span data-stu-id="ee522-145">Boolean</span></span>|<span data-ttu-id="ee522-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ee522-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ee522-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ee522-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ee522-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ee522-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ee522-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee522-149">This property is read-only.</span></span> <span data-ttu-id="ee522-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ee522-151">createdDateTime</span></span>|<span data-ttu-id="ee522-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee522-152">DateTimeOffset</span></span>|<span data-ttu-id="ee522-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ee522-153">DateTime the object was created.</span></span> <span data-ttu-id="ee522-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-155">description</span><span class="sxs-lookup"><span data-stu-id="ee522-155">description</span></span>|<span data-ttu-id="ee522-156">String</span><span class="sxs-lookup"><span data-stu-id="ee522-156">String</span></span>|<span data-ttu-id="ee522-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee522-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ee522-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ee522-159">displayName</span></span>|<span data-ttu-id="ee522-160">Строка</span><span class="sxs-lookup"><span data-stu-id="ee522-160">String</span></span>|<span data-ttu-id="ee522-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee522-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ee522-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-163">version</span><span class="sxs-lookup"><span data-stu-id="ee522-163">version</span></span>|<span data-ttu-id="ee522-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ee522-164">Int32</span></span>|<span data-ttu-id="ee522-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ee522-165">Version of the device configuration.</span></span> <span data-ttu-id="ee522-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ee522-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="ee522-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="ee522-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ee522-168">Int32</span></span>|<span data-ttu-id="ee522-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee522-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ee522-170">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ee522-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ee522-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ee522-171">keyStorageProvider</span></span>|[<span data-ttu-id="ee522-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="ee522-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ee522-173">Поставщик хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="ee522-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="ee522-174">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ee522-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ee522-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ee522-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ee522-176">subjectNameFormat</span></span>|[<span data-ttu-id="ee522-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ee522-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ee522-178">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee522-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="ee522-179">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ee522-180">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="ee522-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ee522-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ee522-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ee522-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ee522-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ee522-183">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee522-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="ee522-184">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ee522-185">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ee522-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ee522-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ee522-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ee522-187">Int32</span><span class="sxs-lookup"><span data-stu-id="ee522-187">Int32</span></span>|<span data-ttu-id="ee522-188">Значение периода Валидтий для сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee522-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="ee522-189">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ee522-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ee522-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ee522-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ee522-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ee522-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ee522-192">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="ee522-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="ee522-193">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ee522-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="ee522-194">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ee522-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ee522-195">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="ee522-195">extendedKeyUsages</span></span>|<span data-ttu-id="ee522-196">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="ee522-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="ee522-197">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="ee522-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="ee522-198">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ee522-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ee522-199">Наследуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ee522-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="ee522-200">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="ee522-200">scepServerUrls</span></span>|<span data-ttu-id="ee522-201">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ee522-201">String collection</span></span>|<span data-ttu-id="ee522-202">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="ee522-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="ee522-203">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="ee522-203">subjectNameFormatString</span></span>|<span data-ttu-id="ee522-204">Строка</span><span class="sxs-lookup"><span data-stu-id="ee522-204">String</span></span>|<span data-ttu-id="ee522-205">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="ee522-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="ee522-206">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="ee522-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="ee522-207">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="ee522-207">keyUsage</span></span>|[<span data-ttu-id="ee522-208">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="ee522-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="ee522-209">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="ee522-209">SCEP Key Usage.</span></span> <span data-ttu-id="ee522-210">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="ee522-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="ee522-211">keySize</span><span class="sxs-lookup"><span data-stu-id="ee522-211">keySize</span></span>|[<span data-ttu-id="ee522-212">keySize</span><span class="sxs-lookup"><span data-stu-id="ee522-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="ee522-213">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="ee522-213">SCEP Key Size.</span></span> <span data-ttu-id="ee522-214">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="ee522-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="ee522-215">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="ee522-215">hashAlgorithm</span></span>|[<span data-ttu-id="ee522-216">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="ee522-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="ee522-217">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="ee522-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="ee522-218">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="ee522-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="ee522-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="ee522-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="ee522-220">Строка</span><span class="sxs-lookup"><span data-stu-id="ee522-220">String</span></span>|<span data-ttu-id="ee522-221">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="ee522-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="ee522-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee522-222">Response</span></span>
<span data-ttu-id="ee522-223">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee522-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee522-224">Пример</span><span class="sxs-lookup"><span data-stu-id="ee522-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee522-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee522-225">Request</span></span>
<span data-ttu-id="ee522-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee522-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="ee522-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee522-227">Response</span></span>
<span data-ttu-id="ee522-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee522-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
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




