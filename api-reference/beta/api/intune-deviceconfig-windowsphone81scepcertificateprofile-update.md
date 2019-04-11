---
title: Обновление windowsPhone81SCEPCertificateProfile
description: Обновление свойств объекта windowsPhone81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a9cd03cd789d496bfe8fc1f04e03743c606fac7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794311"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="e381f-103">Обновление windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e381f-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="e381f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e381f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e381f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e381f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e381f-106">Обновление свойств объекта [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e381f-106">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e381f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e381f-107">Prerequisites</span></span>
<span data-ttu-id="e381f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e381f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e381f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e381f-110">Permission type</span></span>|<span data-ttu-id="e381f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e381f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e381f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e381f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e381f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e381f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e381f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e381f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e381f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e381f-115">Not supported.</span></span>|
|<span data-ttu-id="e381f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e381f-116">Application</span></span>|<span data-ttu-id="e381f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e381f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e381f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e381f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e381f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e381f-119">Request headers</span></span>
|<span data-ttu-id="e381f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e381f-120">Header</span></span>|<span data-ttu-id="e381f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e381f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e381f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e381f-122">Authorization</span></span>|<span data-ttu-id="e381f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e381f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e381f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e381f-124">Accept</span></span>|<span data-ttu-id="e381f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e381f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e381f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e381f-126">Request body</span></span>
<span data-ttu-id="e381f-127">В тексте запроса добавьте представление объекта [WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e381f-127">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="e381f-128">В следующей таблице приведены свойства, необходимые при создании [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-128">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="e381f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e381f-129">Property</span></span>|<span data-ttu-id="e381f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e381f-130">Type</span></span>|<span data-ttu-id="e381f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e381f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e381f-132">id</span><span class="sxs-lookup"><span data-stu-id="e381f-132">id</span></span>|<span data-ttu-id="e381f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e381f-133">String</span></span>|<span data-ttu-id="e381f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e381f-134">Key of the entity.</span></span> <span data-ttu-id="e381f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e381f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e381f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e381f-137">DateTimeOffset</span></span>|<span data-ttu-id="e381f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e381f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e381f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e381f-140">roleScopeTagIds</span></span>|<span data-ttu-id="e381f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e381f-141">String collection</span></span>|<span data-ttu-id="e381f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e381f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e381f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e381f-144">supportsScopeTags</span></span>|<span data-ttu-id="e381f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e381f-145">Boolean</span></span>|<span data-ttu-id="e381f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e381f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e381f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e381f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e381f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e381f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e381f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e381f-149">This property is read-only.</span></span> <span data-ttu-id="e381f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e381f-151">createdDateTime</span></span>|<span data-ttu-id="e381f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e381f-152">DateTimeOffset</span></span>|<span data-ttu-id="e381f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e381f-153">DateTime the object was created.</span></span> <span data-ttu-id="e381f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-155">description</span><span class="sxs-lookup"><span data-stu-id="e381f-155">description</span></span>|<span data-ttu-id="e381f-156">String</span><span class="sxs-lookup"><span data-stu-id="e381f-156">String</span></span>|<span data-ttu-id="e381f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e381f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e381f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e381f-159">displayName</span></span>|<span data-ttu-id="e381f-160">String</span><span class="sxs-lookup"><span data-stu-id="e381f-160">String</span></span>|<span data-ttu-id="e381f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e381f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e381f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-163">version</span><span class="sxs-lookup"><span data-stu-id="e381f-163">version</span></span>|<span data-ttu-id="e381f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e381f-164">Int32</span></span>|<span data-ttu-id="e381f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e381f-165">Version of the device configuration.</span></span> <span data-ttu-id="e381f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e381f-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="e381f-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="e381f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="e381f-168">Int32</span></span>|<span data-ttu-id="e381f-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="e381f-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="e381f-170">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e381f-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e381f-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e381f-171">keyStorageProvider</span></span>|[<span data-ttu-id="e381f-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="e381f-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e381f-173">Поставщик хранилища ключей (KSP).</span><span class="sxs-lookup"><span data-stu-id="e381f-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="e381f-174">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e381f-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="e381f-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="e381f-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e381f-176">subjectNameFormat</span></span>|[<span data-ttu-id="e381f-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="e381f-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="e381f-178">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e381f-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="e381f-179">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e381f-180">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="e381f-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="e381f-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e381f-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="e381f-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="e381f-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="e381f-183">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="e381f-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="e381f-184">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e381f-185">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="e381f-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="e381f-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="e381f-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="e381f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="e381f-187">Int32</span></span>|<span data-ttu-id="e381f-188">Значение периода Валидтий для сертификата.</span><span class="sxs-lookup"><span data-stu-id="e381f-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="e381f-189">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e381f-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e381f-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e381f-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="e381f-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="e381f-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="e381f-192">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="e381f-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="e381f-193">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="e381f-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="e381f-194">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="e381f-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="e381f-195">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="e381f-195">extendedKeyUsages</span></span>|<span data-ttu-id="e381f-196">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="e381f-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="e381f-197">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="e381f-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="e381f-198">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e381f-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e381f-199">НаСледуется от [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e381f-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="e381f-200">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="e381f-200">scepServerUrls</span></span>|<span data-ttu-id="e381f-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e381f-201">String collection</span></span>|<span data-ttu-id="e381f-202">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="e381f-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="e381f-203">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="e381f-203">subjectNameFormatString</span></span>|<span data-ttu-id="e381f-204">String</span><span class="sxs-lookup"><span data-stu-id="e381f-204">String</span></span>|<span data-ttu-id="e381f-205">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="e381f-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="e381f-206">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="e381f-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="e381f-207">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="e381f-207">keyUsage</span></span>|[<span data-ttu-id="e381f-208">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="e381f-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="e381f-209">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="e381f-209">SCEP Key Usage.</span></span> <span data-ttu-id="e381f-210">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="e381f-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="e381f-211">keySize</span><span class="sxs-lookup"><span data-stu-id="e381f-211">keySize</span></span>|[<span data-ttu-id="e381f-212">keySize</span><span class="sxs-lookup"><span data-stu-id="e381f-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="e381f-213">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="e381f-213">SCEP Key Size.</span></span> <span data-ttu-id="e381f-214">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="e381f-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="e381f-215">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="e381f-215">hashAlgorithm</span></span>|[<span data-ttu-id="e381f-216">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="e381f-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="e381f-217">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="e381f-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="e381f-218">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="e381f-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="e381f-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="e381f-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="e381f-220">String</span><span class="sxs-lookup"><span data-stu-id="e381f-220">String</span></span>|<span data-ttu-id="e381f-221">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="e381f-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="e381f-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="e381f-222">Response</span></span>
<span data-ttu-id="e381f-223">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e381f-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e381f-224">Пример</span><span class="sxs-lookup"><span data-stu-id="e381f-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="e381f-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="e381f-225">Request</span></span>
<span data-ttu-id="e381f-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e381f-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e381f-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="e381f-227">Response</span></span>
<span data-ttu-id="e381f-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e381f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





