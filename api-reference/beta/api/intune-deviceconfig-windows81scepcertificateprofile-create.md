---
title: Создание windows81SCEPCertificateProfile
description: Создание нового объекта windows81SCEPCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 327bf03b2927e3b45555e10c0b3322e153d26526
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165585"
---
# <a name="create-windows81scepcertificateprofile"></a><span data-ttu-id="8d454-103">Создание windows81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="8d454-103">Create windows81SCEPCertificateProfile</span></span>

> <span data-ttu-id="8d454-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d454-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d454-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d454-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d454-106">Создание нового объекта [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8d454-106">Create a new [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d454-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8d454-107">Prerequisites</span></span>
<span data-ttu-id="8d454-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d454-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d454-110">Permission type</span></span>|<span data-ttu-id="8d454-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d454-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d454-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d454-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d454-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d454-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d454-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d454-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d454-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d454-115">Not supported.</span></span>|
|<span data-ttu-id="8d454-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d454-116">Application</span></span>|<span data-ttu-id="8d454-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d454-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d454-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d454-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d454-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d454-119">Request headers</span></span>
|<span data-ttu-id="8d454-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d454-120">Header</span></span>|<span data-ttu-id="8d454-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d454-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d454-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d454-122">Authorization</span></span>|<span data-ttu-id="8d454-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8d454-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d454-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8d454-124">Accept</span></span>|<span data-ttu-id="8d454-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d454-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d454-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d454-126">Request body</span></span>
<span data-ttu-id="8d454-127">В тексте запроса добавьте представление объекта windows81SCEPCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d454-127">In the request body, supply a JSON representation for the windows81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="8d454-128">В следующей таблице приведены свойства, необходимые при создании windows81SCEPCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="8d454-128">The following table shows the properties that are required when you create the windows81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="8d454-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d454-129">Property</span></span>|<span data-ttu-id="8d454-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8d454-130">Type</span></span>|<span data-ttu-id="8d454-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8d454-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d454-132">id</span><span class="sxs-lookup"><span data-stu-id="8d454-132">id</span></span>|<span data-ttu-id="8d454-133">String</span><span class="sxs-lookup"><span data-stu-id="8d454-133">String</span></span>|<span data-ttu-id="8d454-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8d454-134">Key of the entity.</span></span> <span data-ttu-id="8d454-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d454-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8d454-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d454-137">DateTimeOffset</span></span>|<span data-ttu-id="8d454-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8d454-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8d454-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d454-140">roleScopeTagIds</span></span>|<span data-ttu-id="8d454-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d454-141">String collection</span></span>|<span data-ttu-id="8d454-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8d454-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d454-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8d454-144">supportsScopeTags</span></span>|<span data-ttu-id="8d454-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8d454-145">Boolean</span></span>|<span data-ttu-id="8d454-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8d454-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d454-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8d454-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d454-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8d454-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d454-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d454-149">This property is read-only.</span></span> <span data-ttu-id="8d454-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d454-151">createdDateTime</span></span>|<span data-ttu-id="8d454-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d454-152">DateTimeOffset</span></span>|<span data-ttu-id="8d454-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8d454-153">DateTime the object was created.</span></span> <span data-ttu-id="8d454-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-155">description</span><span class="sxs-lookup"><span data-stu-id="8d454-155">description</span></span>|<span data-ttu-id="8d454-156">String</span><span class="sxs-lookup"><span data-stu-id="8d454-156">String</span></span>|<span data-ttu-id="8d454-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d454-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d454-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8d454-159">displayName</span></span>|<span data-ttu-id="8d454-160">String</span><span class="sxs-lookup"><span data-stu-id="8d454-160">String</span></span>|<span data-ttu-id="8d454-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d454-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d454-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-163">version</span><span class="sxs-lookup"><span data-stu-id="8d454-163">version</span></span>|<span data-ttu-id="8d454-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8d454-164">Int32</span></span>|<span data-ttu-id="8d454-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8d454-165">Version of the device configuration.</span></span> <span data-ttu-id="8d454-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d454-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="8d454-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="8d454-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8d454-168">Int32</span></span>|<span data-ttu-id="8d454-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="8d454-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="8d454-170">Допустимые значения — от 1 до 99, наСледуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d454-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="8d454-171">keyStorageProvider</span></span>|[<span data-ttu-id="8d454-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="8d454-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="8d454-173">Поставщик хранилища ключей (KSP), наСледуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="8d454-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="8d454-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="8d454-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8d454-175">subjectNameFormat</span></span>|[<span data-ttu-id="8d454-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="8d454-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="8d454-177">Формат имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="8d454-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="8d454-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="8d454-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8d454-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="8d454-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="8d454-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="8d454-181">Тип альтернативного имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="8d454-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="8d454-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="8d454-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="8d454-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="8d454-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8d454-184">Int32</span></span>|<span data-ttu-id="8d454-185">Значение срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d454-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8d454-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="8d454-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="8d454-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="8d454-188">Масштаб срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="8d454-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="8d454-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="8d454-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="8d454-190">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="8d454-190">extendedKeyUsages</span></span>|<span data-ttu-id="8d454-191">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="8d454-192">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="8d454-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="8d454-193">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8d454-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8d454-194">НаСледуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-194">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d454-195">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="8d454-195">customSubjectAlternativeNames</span></span>|<span data-ttu-id="8d454-196">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-196">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="8d454-197">Настраиваемые параметры имени субъекта Алтерантиве.</span><span class="sxs-lookup"><span data-stu-id="8d454-197">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="8d454-198">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8d454-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8d454-199">НаСледуется от [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="8d454-199">Inherited from [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="8d454-200">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="8d454-200">scepServerUrls</span></span>|<span data-ttu-id="8d454-201">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d454-201">String collection</span></span>|<span data-ttu-id="8d454-202">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="8d454-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="8d454-203">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="8d454-203">subjectNameFormatString</span></span>|<span data-ttu-id="8d454-204">String</span><span class="sxs-lookup"><span data-stu-id="8d454-204">String</span></span>|<span data-ttu-id="8d454-205">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="8d454-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="8d454-206">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="8d454-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="8d454-207">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="8d454-207">keyUsage</span></span>|[<span data-ttu-id="8d454-208">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="8d454-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="8d454-209">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="8d454-209">SCEP Key Usage.</span></span> <span data-ttu-id="8d454-210">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="8d454-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="8d454-211">keySize</span><span class="sxs-lookup"><span data-stu-id="8d454-211">keySize</span></span>|[<span data-ttu-id="8d454-212">keySize</span><span class="sxs-lookup"><span data-stu-id="8d454-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="8d454-213">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="8d454-213">SCEP Key Size.</span></span> <span data-ttu-id="8d454-214">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="8d454-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="8d454-215">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="8d454-215">hashAlgorithm</span></span>|[<span data-ttu-id="8d454-216">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="8d454-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="8d454-217">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="8d454-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="8d454-218">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="8d454-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="8d454-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="8d454-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="8d454-220">String</span><span class="sxs-lookup"><span data-stu-id="8d454-220">String</span></span>|<span data-ttu-id="8d454-221">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="8d454-221">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="8d454-222">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8d454-222">certificateStore</span></span>|[<span data-ttu-id="8d454-223">certificateStore</span><span class="sxs-lookup"><span data-stu-id="8d454-223">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="8d454-224">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="8d454-224">Target store certificate.</span></span> <span data-ttu-id="8d454-225">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="8d454-225">Possible values are: `user`, `machine`.</span></span>|



## <a name="response"></a><span data-ttu-id="8d454-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d454-226">Response</span></span>
<span data-ttu-id="8d454-227">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d454-227">If successful, this method returns a `201 Created` response code and a [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d454-228">Пример</span><span class="sxs-lookup"><span data-stu-id="8d454-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d454-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d454-229">Request</span></span>
<span data-ttu-id="8d454-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d454-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1251

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="8d454-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d454-231">Response</span></span>
<span data-ttu-id="8d454-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d454-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1423

{
  "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
  "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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




