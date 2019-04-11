---
title: Создание macOSScepCertificateProfile
description: Создание нового объекта macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc2f24a37c3c4cda0efbff722b771aa097975963
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776488"
---
# <a name="create-macosscepcertificateprofile"></a><span data-ttu-id="5ec7a-103">Создание macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5ec7a-103">Create macOSScepCertificateProfile</span></span>

> <span data-ttu-id="5ec7a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ec7a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ec7a-106">Создание нового объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5ec7a-106">Create a new [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ec7a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5ec7a-107">Prerequisites</span></span>
<span data-ttu-id="5ec7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ec7a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ec7a-110">Permission type</span></span>|<span data-ttu-id="5ec7a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ec7a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ec7a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec7a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ec7a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ec7a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-115">Not supported.</span></span>|
|<span data-ttu-id="5ec7a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ec7a-116">Application</span></span>|<span data-ttu-id="5ec7a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ec7a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ec7a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5ec7a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ec7a-119">Request headers</span></span>
|<span data-ttu-id="5ec7a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ec7a-120">Header</span></span>|<span data-ttu-id="5ec7a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5ec7a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ec7a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ec7a-122">Authorization</span></span>|<span data-ttu-id="5ec7a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ec7a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5ec7a-124">Accept</span></span>|<span data-ttu-id="5ec7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ec7a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ec7a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ec7a-126">Request body</span></span>
<span data-ttu-id="5ec7a-127">В тексте запроса добавьте представление объекта macOSScepCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-127">In the request body, supply a JSON representation for the macOSScepCertificateProfile object.</span></span>

<span data-ttu-id="5ec7a-128">В следующей таблице приведены свойства, необходимые при создании macOSScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-128">The following table shows the properties that are required when you create the macOSScepCertificateProfile.</span></span>

|<span data-ttu-id="5ec7a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ec7a-129">Property</span></span>|<span data-ttu-id="5ec7a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5ec7a-130">Type</span></span>|<span data-ttu-id="5ec7a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5ec7a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec7a-132">id</span><span class="sxs-lookup"><span data-stu-id="5ec7a-132">id</span></span>|<span data-ttu-id="5ec7a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5ec7a-133">String</span></span>|<span data-ttu-id="5ec7a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-134">Key of the entity.</span></span> <span data-ttu-id="5ec7a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec7a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ec7a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec7a-137">DateTimeOffset</span></span>|<span data-ttu-id="5ec7a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ec7a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ec7a-140">roleScopeTagIds</span></span>|<span data-ttu-id="5ec7a-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-141">String collection</span></span>|<span data-ttu-id="5ec7a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ec7a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5ec7a-144">supportsScopeTags</span></span>|<span data-ttu-id="5ec7a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ec7a-145">Boolean</span></span>|<span data-ttu-id="5ec7a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ec7a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ec7a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ec7a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-149">This property is read-only.</span></span> <span data-ttu-id="5ec7a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec7a-151">createdDateTime</span></span>|<span data-ttu-id="5ec7a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec7a-152">DateTimeOffset</span></span>|<span data-ttu-id="5ec7a-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-153">DateTime the object was created.</span></span> <span data-ttu-id="5ec7a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-155">description</span><span class="sxs-lookup"><span data-stu-id="5ec7a-155">description</span></span>|<span data-ttu-id="5ec7a-156">String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-156">String</span></span>|<span data-ttu-id="5ec7a-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ec7a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5ec7a-159">displayName</span></span>|<span data-ttu-id="5ec7a-160">String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-160">String</span></span>|<span data-ttu-id="5ec7a-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ec7a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-163">version</span><span class="sxs-lookup"><span data-stu-id="5ec7a-163">version</span></span>|<span data-ttu-id="5ec7a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec7a-164">Int32</span></span>|<span data-ttu-id="5ec7a-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-165">Version of the device configuration.</span></span> <span data-ttu-id="5ec7a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ec7a-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="5ec7a-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5ec7a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec7a-168">Int32</span></span>|<span data-ttu-id="5ec7a-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5ec7a-170">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ec7a-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5ec7a-171">subjectNameFormat</span></span>|[<span data-ttu-id="5ec7a-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="5ec7a-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5ec7a-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="5ec7a-174">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5ec7a-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5ec7a-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ec7a-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5ec7a-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5ec7a-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5ec7a-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="5ec7a-179">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5ec7a-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5ec7a-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5ec7a-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5ec7a-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5ec7a-182">Int32</span></span>|<span data-ttu-id="5ec7a-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5ec7a-184">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5ec7a-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ec7a-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5ec7a-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5ec7a-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5ec7a-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5ec7a-188">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="5ec7a-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5ec7a-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="5ec7a-190">scepServerUrls</span></span>|<span data-ttu-id="5ec7a-191">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-191">String collection</span></span>|<span data-ttu-id="5ec7a-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="5ec7a-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="5ec7a-193">subjectNameFormatString</span></span>|<span data-ttu-id="5ec7a-194">String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-194">String</span></span>|<span data-ttu-id="5ec7a-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="5ec7a-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="5ec7a-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="5ec7a-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="5ec7a-197">keyUsage</span></span>|[<span data-ttu-id="5ec7a-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="5ec7a-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="5ec7a-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-199">SCEP Key Usage.</span></span> <span data-ttu-id="5ec7a-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="5ec7a-201">keySize</span><span class="sxs-lookup"><span data-stu-id="5ec7a-201">keySize</span></span>|[<span data-ttu-id="5ec7a-202">keySize</span><span class="sxs-lookup"><span data-stu-id="5ec7a-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="5ec7a-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-203">SCEP Key Size.</span></span> <span data-ttu-id="5ec7a-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="5ec7a-205">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="5ec7a-205">hashAlgorithm</span></span>|[<span data-ttu-id="5ec7a-206">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="5ec7a-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="5ec7a-207">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="5ec7a-208">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="5ec7a-209">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="5ec7a-209">extendedKeyUsages</span></span>|<span data-ttu-id="5ec7a-210">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="5ec7a-211">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="5ec7a-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="5ec7a-212">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5ec7a-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5ec7a-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5ec7a-214">String</span><span class="sxs-lookup"><span data-stu-id="5ec7a-214">String</span></span>|<span data-ttu-id="5ec7a-215">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="5ec7a-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5ec7a-216">certificateStore</span></span>|[<span data-ttu-id="5ec7a-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="5ec7a-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="5ec7a-218">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-218">Target store certificate.</span></span> <span data-ttu-id="5ec7a-219">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="5ec7a-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="5ec7a-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="5ec7a-221">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="5ec7a-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="5ec7a-222">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="5ec7a-223">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5ec7a-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ec7a-224">Response</span></span>
<span data-ttu-id="5ec7a-225">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-225">If successful, this method returns a `201 Created` response code and a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ec7a-226">Пример</span><span class="sxs-lookup"><span data-stu-id="5ec7a-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ec7a-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ec7a-227">Request</span></span>
<span data-ttu-id="5ec7a-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
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
  "hashAlgorithm": "sha2",
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

### <a name="response"></a><span data-ttu-id="5ec7a-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ec7a-229">Response</span></span>
<span data-ttu-id="5ec7a-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ec7a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
  "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
  "hashAlgorithm": "sha2",
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





