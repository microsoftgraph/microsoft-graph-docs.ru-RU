---
title: Обновление macOSScepCertificateProfile
description: Обновление свойств объекта macOSScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2da7148fb9cdba31dd055a2edd66d00542f4586a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518424"
---
# <a name="update-macosscepcertificateprofile"></a><span data-ttu-id="f1f30-103">Обновление macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f1f30-103">Update macOSScepCertificateProfile</span></span>

> <span data-ttu-id="f1f30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1f30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1f30-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1f30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1f30-106">Обновление свойств объекта [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f1f30-106">Update the properties of a [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1f30-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f1f30-107">Prerequisites</span></span>
<span data-ttu-id="f1f30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f30-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1f30-110">Permission type</span></span>|<span data-ttu-id="f1f30-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1f30-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1f30-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1f30-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1f30-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f30-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1f30-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1f30-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1f30-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1f30-115">Not supported.</span></span>|
|<span data-ttu-id="f1f30-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1f30-116">Application</span></span>|<span data-ttu-id="f1f30-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1f30-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1f30-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1f30-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1f30-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1f30-119">Request headers</span></span>
|<span data-ttu-id="f1f30-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1f30-120">Header</span></span>|<span data-ttu-id="f1f30-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f1f30-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1f30-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1f30-122">Authorization</span></span>|<span data-ttu-id="f1f30-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1f30-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1f30-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f1f30-124">Accept</span></span>|<span data-ttu-id="f1f30-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1f30-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f30-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1f30-126">Request body</span></span>
<span data-ttu-id="f1f30-127">В тексте запроса добавьте представление объекта [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1f30-127">In the request body, supply a JSON representation for the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="f1f30-128">В следующей таблице приведены свойства, необходимые при создании [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-128">The following table shows the properties that are required when you create the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md).</span></span>

|<span data-ttu-id="f1f30-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1f30-129">Property</span></span>|<span data-ttu-id="f1f30-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f1f30-130">Type</span></span>|<span data-ttu-id="f1f30-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f1f30-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1f30-132">id</span><span class="sxs-lookup"><span data-stu-id="f1f30-132">id</span></span>|<span data-ttu-id="f1f30-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f1f30-133">String</span></span>|<span data-ttu-id="f1f30-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1f30-134">Key of the entity.</span></span> <span data-ttu-id="f1f30-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1f30-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f1f30-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1f30-137">DateTimeOffset</span></span>|<span data-ttu-id="f1f30-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f1f30-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f1f30-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1f30-140">roleScopeTagIds</span></span>|<span data-ttu-id="f1f30-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f1f30-141">String collection</span></span>|<span data-ttu-id="f1f30-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f1f30-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1f30-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f1f30-144">supportsScopeTags</span></span>|<span data-ttu-id="f1f30-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f1f30-145">Boolean</span></span>|<span data-ttu-id="f1f30-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f1f30-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1f30-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f1f30-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1f30-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f1f30-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1f30-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f1f30-149">This property is read-only.</span></span> <span data-ttu-id="f1f30-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1f30-151">createdDateTime</span></span>|<span data-ttu-id="f1f30-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1f30-152">DateTimeOffset</span></span>|<span data-ttu-id="f1f30-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f1f30-153">DateTime the object was created.</span></span> <span data-ttu-id="f1f30-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-155">description</span><span class="sxs-lookup"><span data-stu-id="f1f30-155">description</span></span>|<span data-ttu-id="f1f30-156">String</span><span class="sxs-lookup"><span data-stu-id="f1f30-156">String</span></span>|<span data-ttu-id="f1f30-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1f30-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1f30-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f1f30-159">displayName</span></span>|<span data-ttu-id="f1f30-160">String</span><span class="sxs-lookup"><span data-stu-id="f1f30-160">String</span></span>|<span data-ttu-id="f1f30-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1f30-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1f30-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-163">version</span><span class="sxs-lookup"><span data-stu-id="f1f30-163">version</span></span>|<span data-ttu-id="f1f30-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f1f30-164">Int32</span></span>|<span data-ttu-id="f1f30-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f1f30-165">Version of the device configuration.</span></span> <span data-ttu-id="f1f30-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1f30-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="f1f30-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="f1f30-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f1f30-168">Int32</span></span>|<span data-ttu-id="f1f30-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1f30-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f1f30-170">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f1f30-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f1f30-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f1f30-171">subjectNameFormat</span></span>|[<span data-ttu-id="f1f30-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="f1f30-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="f1f30-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1f30-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="f1f30-174">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1f30-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="f1f30-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f1f30-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f1f30-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f1f30-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f1f30-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1f30-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f1f30-179">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1f30-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f1f30-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f1f30-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f1f30-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f1f30-182">Int32</span></span>|<span data-ttu-id="f1f30-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1f30-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f1f30-184">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f1f30-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f1f30-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f1f30-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f1f30-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f1f30-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f1f30-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f1f30-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f1f30-188">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f1f30-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="f1f30-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f1f30-190">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="f1f30-190">scepServerUrls</span></span>|<span data-ttu-id="f1f30-191">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f1f30-191">String collection</span></span>|<span data-ttu-id="f1f30-192">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="f1f30-192">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="f1f30-193">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="f1f30-193">subjectNameFormatString</span></span>|<span data-ttu-id="f1f30-194">String</span><span class="sxs-lookup"><span data-stu-id="f1f30-194">String</span></span>|<span data-ttu-id="f1f30-195">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="f1f30-195">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="f1f30-196">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="f1f30-196">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="f1f30-197">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="f1f30-197">keyUsage</span></span>|[<span data-ttu-id="f1f30-198">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="f1f30-198">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="f1f30-199">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="f1f30-199">SCEP Key Usage.</span></span> <span data-ttu-id="f1f30-200">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-200">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="f1f30-201">keySize</span><span class="sxs-lookup"><span data-stu-id="f1f30-201">keySize</span></span>|[<span data-ttu-id="f1f30-202">keySize</span><span class="sxs-lookup"><span data-stu-id="f1f30-202">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="f1f30-203">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="f1f30-203">SCEP Key Size.</span></span> <span data-ttu-id="f1f30-204">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-204">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="f1f30-205">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="f1f30-205">hashAlgorithm</span></span>|[<span data-ttu-id="f1f30-206">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="f1f30-206">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="f1f30-207">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="f1f30-207">SCEP Hash Algorithm.</span></span> <span data-ttu-id="f1f30-208">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-208">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="f1f30-209">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="f1f30-209">extendedKeyUsages</span></span>|<span data-ttu-id="f1f30-210">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f1f30-210">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f1f30-211">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="f1f30-211">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f1f30-212">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1f30-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f1f30-213">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f1f30-213">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f1f30-214">String</span><span class="sxs-lookup"><span data-stu-id="f1f30-214">String</span></span>|<span data-ttu-id="f1f30-215">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="f1f30-215">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="f1f30-216">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f1f30-216">certificateStore</span></span>|[<span data-ttu-id="f1f30-217">certificateStore</span><span class="sxs-lookup"><span data-stu-id="f1f30-217">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="f1f30-218">Сертификат целевого хранилища.</span><span class="sxs-lookup"><span data-stu-id="f1f30-218">Target store certificate.</span></span> <span data-ttu-id="f1f30-219">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="f1f30-219">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="f1f30-220">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="f1f30-220">customSubjectAlternativeNames</span></span>|<span data-ttu-id="f1f30-221">Коллекция [кустомсубжекталтернативенаме](../resources/intune-deviceconfig-customsubjectalternativename.md)</span><span class="sxs-lookup"><span data-stu-id="f1f30-221">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="f1f30-222">Настраиваемые параметры альтернативного имени субъекта.</span><span class="sxs-lookup"><span data-stu-id="f1f30-222">Custom Subject Alternative Name Settings.</span></span> <span data-ttu-id="f1f30-223">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1f30-223">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f1f30-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1f30-224">Response</span></span>
<span data-ttu-id="f1f30-225">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f1f30-225">If successful, this method returns a `200 OK` response code and an updated [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1f30-226">Пример</span><span class="sxs-lookup"><span data-stu-id="f1f30-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1f30-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1f30-227">Request</span></span>
<span data-ttu-id="f1f30-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1f30-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f1f30-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1f30-229">Response</span></span>
<span data-ttu-id="f1f30-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1f30-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





