---
title: Создание iosPkcsCertificateProfile
description: Создание нового объекта iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce6be924f8db052b400b403af4eea44ac27d10d3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796971"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="82eca-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="82eca-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="82eca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82eca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82eca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82eca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82eca-106">Создание нового объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="82eca-106">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82eca-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82eca-107">Prerequisites</span></span>
<span data-ttu-id="82eca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82eca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82eca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82eca-110">Permission type</span></span>|<span data-ttu-id="82eca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82eca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82eca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82eca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82eca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82eca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82eca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82eca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82eca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82eca-115">Not supported.</span></span>|
|<span data-ttu-id="82eca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82eca-116">Application</span></span>|<span data-ttu-id="82eca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82eca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82eca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82eca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82eca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82eca-119">Request headers</span></span>
|<span data-ttu-id="82eca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82eca-120">Header</span></span>|<span data-ttu-id="82eca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82eca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82eca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82eca-122">Authorization</span></span>|<span data-ttu-id="82eca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82eca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82eca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82eca-124">Accept</span></span>|<span data-ttu-id="82eca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82eca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82eca-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82eca-126">Request body</span></span>
<span data-ttu-id="82eca-127">В тексте запроса добавьте представление объекта iosPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82eca-127">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="82eca-128">В следующей таблице приведены свойства, необходимые при создании iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="82eca-128">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="82eca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82eca-129">Property</span></span>|<span data-ttu-id="82eca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82eca-130">Type</span></span>|<span data-ttu-id="82eca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82eca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82eca-132">id</span><span class="sxs-lookup"><span data-stu-id="82eca-132">id</span></span>|<span data-ttu-id="82eca-133">Строка</span><span class="sxs-lookup"><span data-stu-id="82eca-133">String</span></span>|<span data-ttu-id="82eca-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82eca-134">Key of the entity.</span></span> <span data-ttu-id="82eca-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82eca-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82eca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82eca-137">DateTimeOffset</span></span>|<span data-ttu-id="82eca-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82eca-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82eca-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82eca-140">roleScopeTagIds</span></span>|<span data-ttu-id="82eca-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="82eca-141">String collection</span></span>|<span data-ttu-id="82eca-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="82eca-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82eca-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="82eca-144">supportsScopeTags</span></span>|<span data-ttu-id="82eca-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="82eca-145">Boolean</span></span>|<span data-ttu-id="82eca-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="82eca-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82eca-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="82eca-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82eca-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="82eca-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82eca-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82eca-149">This property is read-only.</span></span> <span data-ttu-id="82eca-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82eca-151">createdDateTime</span></span>|<span data-ttu-id="82eca-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82eca-152">DateTimeOffset</span></span>|<span data-ttu-id="82eca-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82eca-153">DateTime the object was created.</span></span> <span data-ttu-id="82eca-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-155">description</span><span class="sxs-lookup"><span data-stu-id="82eca-155">description</span></span>|<span data-ttu-id="82eca-156">String</span><span class="sxs-lookup"><span data-stu-id="82eca-156">String</span></span>|<span data-ttu-id="82eca-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82eca-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82eca-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-159">displayName</span><span class="sxs-lookup"><span data-stu-id="82eca-159">displayName</span></span>|<span data-ttu-id="82eca-160">String</span><span class="sxs-lookup"><span data-stu-id="82eca-160">String</span></span>|<span data-ttu-id="82eca-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82eca-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82eca-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-163">version</span><span class="sxs-lookup"><span data-stu-id="82eca-163">version</span></span>|<span data-ttu-id="82eca-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82eca-164">Int32</span></span>|<span data-ttu-id="82eca-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82eca-165">Version of the device configuration.</span></span> <span data-ttu-id="82eca-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82eca-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="82eca-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="82eca-168">Int32</span><span class="sxs-lookup"><span data-stu-id="82eca-168">Int32</span></span>|<span data-ttu-id="82eca-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="82eca-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="82eca-170">Допустимые значения — от 1 до 99, наСледуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="82eca-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="82eca-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="82eca-171">subjectNameFormat</span></span>|[<span data-ttu-id="82eca-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="82eca-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="82eca-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="82eca-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="82eca-174">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="82eca-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="82eca-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="82eca-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="82eca-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="82eca-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="82eca-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="82eca-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="82eca-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="82eca-179">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="82eca-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="82eca-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="82eca-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="82eca-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="82eca-182">Int32</span><span class="sxs-lookup"><span data-stu-id="82eca-182">Int32</span></span>|<span data-ttu-id="82eca-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="82eca-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="82eca-184">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="82eca-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="82eca-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="82eca-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="82eca-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="82eca-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="82eca-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="82eca-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="82eca-188">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="82eca-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="82eca-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="82eca-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="82eca-190">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="82eca-190">certificationAuthority</span></span>|<span data-ttu-id="82eca-191">String</span><span class="sxs-lookup"><span data-stu-id="82eca-191">String</span></span>|<span data-ttu-id="82eca-192">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="82eca-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="82eca-193">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="82eca-193">certificationAuthorityName</span></span>|<span data-ttu-id="82eca-194">String</span><span class="sxs-lookup"><span data-stu-id="82eca-194">String</span></span>|<span data-ttu-id="82eca-195">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="82eca-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="82eca-196">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="82eca-196">certificateTemplateName</span></span>|<span data-ttu-id="82eca-197">String</span><span class="sxs-lookup"><span data-stu-id="82eca-197">String</span></span>|<span data-ttu-id="82eca-198">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="82eca-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="82eca-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="82eca-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="82eca-200">String</span><span class="sxs-lookup"><span data-stu-id="82eca-200">String</span></span>|<span data-ttu-id="82eca-201">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="82eca-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="82eca-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="82eca-202">Response</span></span>
<span data-ttu-id="82eca-203">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82eca-203">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82eca-204">Пример</span><span class="sxs-lookup"><span data-stu-id="82eca-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="82eca-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="82eca-205">Request</span></span>
<span data-ttu-id="82eca-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82eca-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="82eca-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="82eca-207">Response</span></span>
<span data-ttu-id="82eca-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82eca-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 933

{
  "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
  "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





