---
title: Обновление iosScepCertificateProfile
description: Обновление свойств объекта iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b1b4209a76a07d713cd05201fc0a4dfd616f6c9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143255"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="7fe13-103">Обновление iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7fe13-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="7fe13-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fe13-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7fe13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fe13-106">Обновление свойств объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7fe13-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7fe13-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7fe13-107">Prerequisites</span></span>
<span data-ttu-id="7fe13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7fe13-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fe13-110">Permission type</span></span>|<span data-ttu-id="7fe13-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fe13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fe13-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fe13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7fe13-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe13-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7fe13-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fe13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fe13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe13-115">Not supported.</span></span>|
|<span data-ttu-id="7fe13-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fe13-116">Application</span></span>|<span data-ttu-id="7fe13-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fe13-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe13-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fe13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7fe13-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fe13-119">Request headers</span></span>
|<span data-ttu-id="7fe13-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fe13-120">Header</span></span>|<span data-ttu-id="7fe13-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7fe13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fe13-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fe13-122">Authorization</span></span>|<span data-ttu-id="7fe13-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7fe13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fe13-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7fe13-124">Accept</span></span>|<span data-ttu-id="7fe13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7fe13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fe13-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fe13-126">Request body</span></span>
<span data-ttu-id="7fe13-127">В тексте запроса добавьте представление объекта [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fe13-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="7fe13-128">В следующей таблице приведены свойства, необходимые при создании [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="7fe13-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fe13-129">Property</span></span>|<span data-ttu-id="7fe13-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7fe13-130">Type</span></span>|<span data-ttu-id="7fe13-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7fe13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fe13-132">id</span><span class="sxs-lookup"><span data-stu-id="7fe13-132">id</span></span>|<span data-ttu-id="7fe13-133">String</span><span class="sxs-lookup"><span data-stu-id="7fe13-133">String</span></span>|<span data-ttu-id="7fe13-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7fe13-134">Key of the entity.</span></span> <span data-ttu-id="7fe13-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7fe13-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7fe13-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fe13-137">DateTimeOffset</span></span>|<span data-ttu-id="7fe13-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7fe13-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7fe13-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7fe13-140">roleScopeTagIds</span></span>|<span data-ttu-id="7fe13-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7fe13-141">String collection</span></span>|<span data-ttu-id="7fe13-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7fe13-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7fe13-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7fe13-144">supportsScopeTags</span></span>|<span data-ttu-id="7fe13-145">Логический</span><span class="sxs-lookup"><span data-stu-id="7fe13-145">Boolean</span></span>|<span data-ttu-id="7fe13-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7fe13-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7fe13-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7fe13-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7fe13-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7fe13-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7fe13-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fe13-149">This property is read-only.</span></span> <span data-ttu-id="7fe13-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fe13-151">createdDateTime</span></span>|<span data-ttu-id="7fe13-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fe13-152">DateTimeOffset</span></span>|<span data-ttu-id="7fe13-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7fe13-153">DateTime the object was created.</span></span> <span data-ttu-id="7fe13-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-155">description</span><span class="sxs-lookup"><span data-stu-id="7fe13-155">description</span></span>|<span data-ttu-id="7fe13-156">String</span><span class="sxs-lookup"><span data-stu-id="7fe13-156">String</span></span>|<span data-ttu-id="7fe13-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7fe13-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7fe13-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7fe13-159">displayName</span></span>|<span data-ttu-id="7fe13-160">String</span><span class="sxs-lookup"><span data-stu-id="7fe13-160">String</span></span>|<span data-ttu-id="7fe13-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7fe13-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7fe13-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-163">version</span><span class="sxs-lookup"><span data-stu-id="7fe13-163">version</span></span>|<span data-ttu-id="7fe13-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe13-164">Int32</span></span>|<span data-ttu-id="7fe13-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7fe13-165">Version of the device configuration.</span></span> <span data-ttu-id="7fe13-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7fe13-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="7fe13-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="7fe13-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe13-168">Int32</span></span>|<span data-ttu-id="7fe13-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="7fe13-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7fe13-170">Допустимые значения — от 1 до 99, наСледуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7fe13-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7fe13-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7fe13-171">subjectNameFormat</span></span>|[<span data-ttu-id="7fe13-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="7fe13-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="7fe13-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7fe13-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="7fe13-174">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7fe13-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="7fe13-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7fe13-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7fe13-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7fe13-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7fe13-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7fe13-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="7fe13-179">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7fe13-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7fe13-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7fe13-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7fe13-182">Int32</span><span class="sxs-lookup"><span data-stu-id="7fe13-182">Int32</span></span>|<span data-ttu-id="7fe13-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7fe13-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7fe13-184">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7fe13-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7fe13-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7fe13-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7fe13-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7fe13-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7fe13-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7fe13-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7fe13-188">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7fe13-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="7fe13-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7fe13-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="7fe13-190">scepServerUrls</span></span>|<span data-ttu-id="7fe13-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7fe13-191">String collection</span></span>|<span data-ttu-id="7fe13-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="7fe13-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="7fe13-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="7fe13-193">subjectNameFormatString</span></span>|<span data-ttu-id="7fe13-194">String</span><span class="sxs-lookup"><span data-stu-id="7fe13-194">String</span></span>|<span data-ttu-id="7fe13-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="7fe13-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7fe13-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="7fe13-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7fe13-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="7fe13-197">keyUsage</span></span>|[<span data-ttu-id="7fe13-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="7fe13-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7fe13-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7fe13-199">SCEP Key Usage.</span></span> <span data-ttu-id="7fe13-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7fe13-201">keySize</span><span class="sxs-lookup"><span data-stu-id="7fe13-201">keySize</span></span>|[<span data-ttu-id="7fe13-202">keySize</span><span class="sxs-lookup"><span data-stu-id="7fe13-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7fe13-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7fe13-203">SCEP Key Size.</span></span> <span data-ttu-id="7fe13-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7fe13-205">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="7fe13-205">extendedKeyUsages</span></span>|<span data-ttu-id="7fe13-206">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="7fe13-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7fe13-207">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="7fe13-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7fe13-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7fe13-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7fe13-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7fe13-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7fe13-210">String</span><span class="sxs-lookup"><span data-stu-id="7fe13-210">String</span></span>|<span data-ttu-id="7fe13-211">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="7fe13-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="7fe13-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7fe13-212">certificateStore</span></span>|[<span data-ttu-id="7fe13-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="7fe13-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="7fe13-214">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="7fe13-214">Target store certificate.</span></span> <span data-ttu-id="7fe13-215">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="7fe13-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="7fe13-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="7fe13-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="7fe13-217">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="7fe13-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="7fe13-218">Настраиваемые параметры имени субъекта Алтерантиве.</span><span class="sxs-lookup"><span data-stu-id="7fe13-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="7fe13-219">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7fe13-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7fe13-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fe13-220">Response</span></span>
<span data-ttu-id="7fe13-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7fe13-221">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fe13-222">Пример</span><span class="sxs-lookup"><span data-stu-id="7fe13-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe13-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fe13-223">Request</span></span>
<span data-ttu-id="7fe13-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fe13-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7fe13-225">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fe13-225">Response</span></span>
<span data-ttu-id="7fe13-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7fe13-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.iosScepCertificateProfile",
  "id": "0deb8dbf-8dbf-0deb-bf8d-eb0dbf8deb0d",
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
  "subjectNameFormat": "commonNameAsEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ]
}
```




