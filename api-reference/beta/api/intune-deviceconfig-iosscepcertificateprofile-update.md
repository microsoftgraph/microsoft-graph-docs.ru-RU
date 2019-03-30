---
title: Обновление iosScepCertificateProfile
description: Обновление свойств объекта iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2416c3006e007d10bfa1489eb24c94d244261926
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986063"
---
# <a name="update-iosscepcertificateprofile"></a><span data-ttu-id="fc732-103">Обновление iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="fc732-103">Update iosScepCertificateProfile</span></span>

> <span data-ttu-id="fc732-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc732-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc732-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc732-106">Обновление свойств объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fc732-106">Update the properties of a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc732-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc732-107">Prerequisites</span></span>
<span data-ttu-id="fc732-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc732-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc732-110">Permission type</span></span>|<span data-ttu-id="fc732-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc732-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc732-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc732-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc732-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc732-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc732-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc732-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc732-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc732-115">Not supported.</span></span>|
|<span data-ttu-id="fc732-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc732-116">Application</span></span>|<span data-ttu-id="fc732-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc732-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc732-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc732-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fc732-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc732-119">Request headers</span></span>
|<span data-ttu-id="fc732-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc732-120">Header</span></span>|<span data-ttu-id="fc732-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fc732-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc732-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc732-122">Authorization</span></span>|<span data-ttu-id="fc732-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc732-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc732-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fc732-124">Accept</span></span>|<span data-ttu-id="fc732-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc732-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc732-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc732-126">Request body</span></span>
<span data-ttu-id="fc732-127">В тексте запроса добавьте представление объекта [IosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc732-127">In the request body, supply a JSON representation for the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="fc732-128">В следующей таблице приведены свойства, необходимые при создании [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-128">The following table shows the properties that are required when you create the [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="fc732-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc732-129">Property</span></span>|<span data-ttu-id="fc732-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fc732-130">Type</span></span>|<span data-ttu-id="fc732-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fc732-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc732-132">id</span><span class="sxs-lookup"><span data-stu-id="fc732-132">id</span></span>|<span data-ttu-id="fc732-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fc732-133">String</span></span>|<span data-ttu-id="fc732-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc732-134">Key of the entity.</span></span> <span data-ttu-id="fc732-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc732-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fc732-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc732-137">DateTimeOffset</span></span>|<span data-ttu-id="fc732-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fc732-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fc732-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fc732-140">roleScopeTagIds</span></span>|<span data-ttu-id="fc732-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc732-141">String collection</span></span>|<span data-ttu-id="fc732-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fc732-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fc732-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fc732-144">supportsScopeTags</span></span>|<span data-ttu-id="fc732-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc732-145">Boolean</span></span>|<span data-ttu-id="fc732-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fc732-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fc732-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fc732-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fc732-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fc732-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fc732-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc732-149">This property is read-only.</span></span> <span data-ttu-id="fc732-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc732-151">createdDateTime</span></span>|<span data-ttu-id="fc732-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc732-152">DateTimeOffset</span></span>|<span data-ttu-id="fc732-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fc732-153">DateTime the object was created.</span></span> <span data-ttu-id="fc732-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-155">description</span><span class="sxs-lookup"><span data-stu-id="fc732-155">description</span></span>|<span data-ttu-id="fc732-156">String</span><span class="sxs-lookup"><span data-stu-id="fc732-156">String</span></span>|<span data-ttu-id="fc732-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc732-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fc732-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fc732-159">displayName</span></span>|<span data-ttu-id="fc732-160">String</span><span class="sxs-lookup"><span data-stu-id="fc732-160">String</span></span>|<span data-ttu-id="fc732-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc732-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fc732-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-163">version</span><span class="sxs-lookup"><span data-stu-id="fc732-163">version</span></span>|<span data-ttu-id="fc732-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fc732-164">Int32</span></span>|<span data-ttu-id="fc732-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fc732-165">Version of the device configuration.</span></span> <span data-ttu-id="fc732-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fc732-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="fc732-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="fc732-168">Int32</span><span class="sxs-lookup"><span data-stu-id="fc732-168">Int32</span></span>|<span data-ttu-id="fc732-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc732-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="fc732-170">Допустимые значения — от 1 до 99, наСледуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fc732-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fc732-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fc732-171">subjectNameFormat</span></span>|[<span data-ttu-id="fc732-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="fc732-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="fc732-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc732-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="fc732-174">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fc732-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="fc732-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="fc732-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fc732-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="fc732-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fc732-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fc732-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc732-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="fc732-179">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fc732-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="fc732-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fc732-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="fc732-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="fc732-182">Int32</span><span class="sxs-lookup"><span data-stu-id="fc732-182">Int32</span></span>|<span data-ttu-id="fc732-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc732-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="fc732-184">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fc732-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="fc732-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fc732-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="fc732-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fc732-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fc732-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc732-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="fc732-188">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fc732-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="fc732-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="fc732-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fc732-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="fc732-190">scepServerUrls</span></span>|<span data-ttu-id="fc732-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc732-191">String collection</span></span>|<span data-ttu-id="fc732-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="fc732-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="fc732-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="fc732-193">subjectNameFormatString</span></span>|<span data-ttu-id="fc732-194">String</span><span class="sxs-lookup"><span data-stu-id="fc732-194">String</span></span>|<span data-ttu-id="fc732-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="fc732-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="fc732-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="fc732-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="fc732-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="fc732-197">keyUsage</span></span>|[<span data-ttu-id="fc732-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="fc732-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="fc732-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="fc732-199">SCEP Key Usage.</span></span> <span data-ttu-id="fc732-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="fc732-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="fc732-201">keySize</span><span class="sxs-lookup"><span data-stu-id="fc732-201">keySize</span></span>|[<span data-ttu-id="fc732-202">keySize</span><span class="sxs-lookup"><span data-stu-id="fc732-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="fc732-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="fc732-203">SCEP Key Size.</span></span> <span data-ttu-id="fc732-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="fc732-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="fc732-205">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="fc732-205">extendedKeyUsages</span></span>|<span data-ttu-id="fc732-206">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="fc732-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="fc732-207">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="fc732-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="fc732-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc732-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fc732-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fc732-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fc732-210">String</span><span class="sxs-lookup"><span data-stu-id="fc732-210">String</span></span>|<span data-ttu-id="fc732-211">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="fc732-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="fc732-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fc732-212">certificateStore</span></span>|[<span data-ttu-id="fc732-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="fc732-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="fc732-214">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc732-214">Target store certificate.</span></span> <span data-ttu-id="fc732-215">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="fc732-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="fc732-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="fc732-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="fc732-217">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="fc732-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="fc732-218">Настраиваемые параметры имени субъекта Алтерантиве.</span><span class="sxs-lookup"><span data-stu-id="fc732-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="fc732-219">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="fc732-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fc732-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc732-220">Response</span></span>
<span data-ttu-id="fc732-221">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc732-221">If successful, this method returns a `200 OK` response code and an updated [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc732-222">Пример</span><span class="sxs-lookup"><span data-stu-id="fc732-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc732-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc732-223">Request</span></span>
<span data-ttu-id="fc732-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc732-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc732-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc732-225">Response</span></span>
<span data-ttu-id="fc732-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc732-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




