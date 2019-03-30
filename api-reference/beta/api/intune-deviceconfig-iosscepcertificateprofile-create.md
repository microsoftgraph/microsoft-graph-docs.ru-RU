---
title: Создание iosScepCertificateProfile
description: Создание нового объекта iosScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd52508ef7ffd5581edc988356edbce2eba2d4e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988051"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="186ff-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="186ff-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="186ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="186ff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="186ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186ff-106">Создание нового объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="186ff-106">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="186ff-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="186ff-107">Prerequisites</span></span>
<span data-ttu-id="186ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="186ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="186ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="186ff-110">Permission type</span></span>|<span data-ttu-id="186ff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="186ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="186ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="186ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="186ff-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186ff-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="186ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="186ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="186ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186ff-115">Not supported.</span></span>|
|<span data-ttu-id="186ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="186ff-116">Application</span></span>|<span data-ttu-id="186ff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="186ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="186ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="186ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="186ff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="186ff-119">Request headers</span></span>
|<span data-ttu-id="186ff-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="186ff-120">Header</span></span>|<span data-ttu-id="186ff-121">Значение</span><span class="sxs-lookup"><span data-stu-id="186ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="186ff-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="186ff-122">Authorization</span></span>|<span data-ttu-id="186ff-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="186ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="186ff-124">Accept</span><span class="sxs-lookup"><span data-stu-id="186ff-124">Accept</span></span>|<span data-ttu-id="186ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="186ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="186ff-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="186ff-126">Request body</span></span>
<span data-ttu-id="186ff-127">В тексте запроса добавьте представление объекта iosScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="186ff-127">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="186ff-128">В следующей таблице приведены свойства, необходимые при создании iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="186ff-128">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="186ff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="186ff-129">Property</span></span>|<span data-ttu-id="186ff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="186ff-130">Type</span></span>|<span data-ttu-id="186ff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="186ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186ff-132">id</span><span class="sxs-lookup"><span data-stu-id="186ff-132">id</span></span>|<span data-ttu-id="186ff-133">Строка</span><span class="sxs-lookup"><span data-stu-id="186ff-133">String</span></span>|<span data-ttu-id="186ff-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="186ff-134">Key of the entity.</span></span> <span data-ttu-id="186ff-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="186ff-136">lastModifiedDateTime</span></span>|<span data-ttu-id="186ff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ff-137">DateTimeOffset</span></span>|<span data-ttu-id="186ff-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="186ff-138">DateTime the object was last modified.</span></span> <span data-ttu-id="186ff-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="186ff-140">roleScopeTagIds</span></span>|<span data-ttu-id="186ff-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="186ff-141">String collection</span></span>|<span data-ttu-id="186ff-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="186ff-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="186ff-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="186ff-144">supportsScopeTags</span></span>|<span data-ttu-id="186ff-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="186ff-145">Boolean</span></span>|<span data-ttu-id="186ff-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="186ff-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="186ff-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="186ff-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="186ff-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="186ff-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="186ff-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="186ff-149">This property is read-only.</span></span> <span data-ttu-id="186ff-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="186ff-151">createdDateTime</span></span>|<span data-ttu-id="186ff-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186ff-152">DateTimeOffset</span></span>|<span data-ttu-id="186ff-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="186ff-153">DateTime the object was created.</span></span> <span data-ttu-id="186ff-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-155">description</span><span class="sxs-lookup"><span data-stu-id="186ff-155">description</span></span>|<span data-ttu-id="186ff-156">String</span><span class="sxs-lookup"><span data-stu-id="186ff-156">String</span></span>|<span data-ttu-id="186ff-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="186ff-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="186ff-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-159">displayName</span><span class="sxs-lookup"><span data-stu-id="186ff-159">displayName</span></span>|<span data-ttu-id="186ff-160">String</span><span class="sxs-lookup"><span data-stu-id="186ff-160">String</span></span>|<span data-ttu-id="186ff-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="186ff-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="186ff-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-163">version</span><span class="sxs-lookup"><span data-stu-id="186ff-163">version</span></span>|<span data-ttu-id="186ff-164">Int32</span><span class="sxs-lookup"><span data-stu-id="186ff-164">Int32</span></span>|<span data-ttu-id="186ff-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="186ff-165">Version of the device configuration.</span></span> <span data-ttu-id="186ff-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="186ff-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="186ff-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="186ff-168">Int32</span><span class="sxs-lookup"><span data-stu-id="186ff-168">Int32</span></span>|<span data-ttu-id="186ff-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="186ff-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="186ff-170">Допустимые значения — от 1 до 99, наСледуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="186ff-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="186ff-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="186ff-171">subjectNameFormat</span></span>|[<span data-ttu-id="186ff-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="186ff-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="186ff-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="186ff-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="186ff-174">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="186ff-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="186ff-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="186ff-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="186ff-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="186ff-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="186ff-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="186ff-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="186ff-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="186ff-179">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="186ff-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="186ff-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="186ff-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="186ff-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="186ff-182">Int32</span><span class="sxs-lookup"><span data-stu-id="186ff-182">Int32</span></span>|<span data-ttu-id="186ff-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="186ff-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="186ff-184">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="186ff-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="186ff-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="186ff-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="186ff-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="186ff-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="186ff-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="186ff-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="186ff-188">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="186ff-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="186ff-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="186ff-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="186ff-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="186ff-190">scepServerUrls</span></span>|<span data-ttu-id="186ff-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="186ff-191">String collection</span></span>|<span data-ttu-id="186ff-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="186ff-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="186ff-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="186ff-193">subjectNameFormatString</span></span>|<span data-ttu-id="186ff-194">String</span><span class="sxs-lookup"><span data-stu-id="186ff-194">String</span></span>|<span data-ttu-id="186ff-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="186ff-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="186ff-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="186ff-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="186ff-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="186ff-197">keyUsage</span></span>|[<span data-ttu-id="186ff-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="186ff-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="186ff-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="186ff-199">SCEP Key Usage.</span></span> <span data-ttu-id="186ff-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="186ff-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="186ff-201">keySize</span><span class="sxs-lookup"><span data-stu-id="186ff-201">keySize</span></span>|[<span data-ttu-id="186ff-202">keySize</span><span class="sxs-lookup"><span data-stu-id="186ff-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="186ff-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="186ff-203">SCEP Key Size.</span></span> <span data-ttu-id="186ff-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="186ff-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="186ff-205">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="186ff-205">extendedKeyUsages</span></span>|<span data-ttu-id="186ff-206">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="186ff-206">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="186ff-207">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="186ff-207">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="186ff-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="186ff-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="186ff-209">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="186ff-209">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="186ff-210">String</span><span class="sxs-lookup"><span data-stu-id="186ff-210">String</span></span>|<span data-ttu-id="186ff-211">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="186ff-211">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="186ff-212">certificateStore</span><span class="sxs-lookup"><span data-stu-id="186ff-212">certificateStore</span></span>|[<span data-ttu-id="186ff-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="186ff-213">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="186ff-214">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="186ff-214">Target store certificate.</span></span> <span data-ttu-id="186ff-215">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="186ff-215">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="186ff-216">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="186ff-216">customSubjectAlternativeNames</span></span>|<span data-ttu-id="186ff-217">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="186ff-217">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="186ff-218">Настраиваемые параметры имени субъекта Алтерантиве.</span><span class="sxs-lookup"><span data-stu-id="186ff-218">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="186ff-219">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="186ff-219">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="186ff-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="186ff-220">Response</span></span>
<span data-ttu-id="186ff-221">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="186ff-221">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186ff-222">Пример</span><span class="sxs-lookup"><span data-stu-id="186ff-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="186ff-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="186ff-223">Request</span></span>
<span data-ttu-id="186ff-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="186ff-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="186ff-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="186ff-225">Response</span></span>
<span data-ttu-id="186ff-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="186ff-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




