---
title: Создание iosPkcsCertificateProfile
description: Создание нового объекта iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb667dfc88e33bf6fc035624c1fb67f2bde2bf66
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989038"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="5df99-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5df99-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="5df99-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5df99-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5df99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5df99-106">Создание нового объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5df99-106">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5df99-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5df99-107">Prerequisites</span></span>
<span data-ttu-id="5df99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5df99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5df99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5df99-110">Permission type</span></span>|<span data-ttu-id="5df99-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5df99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5df99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5df99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5df99-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5df99-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5df99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5df99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5df99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df99-115">Not supported.</span></span>|
|<span data-ttu-id="5df99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5df99-116">Application</span></span>|<span data-ttu-id="5df99-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5df99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5df99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5df99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5df99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5df99-119">Request headers</span></span>
|<span data-ttu-id="5df99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5df99-120">Header</span></span>|<span data-ttu-id="5df99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5df99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5df99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5df99-122">Authorization</span></span>|<span data-ttu-id="5df99-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5df99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5df99-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5df99-124">Accept</span></span>|<span data-ttu-id="5df99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5df99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5df99-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5df99-126">Request body</span></span>
<span data-ttu-id="5df99-127">В тексте запроса добавьте представление объекта iosPkcsCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5df99-127">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="5df99-128">В следующей таблице приведены свойства, необходимые при создании iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5df99-128">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="5df99-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5df99-129">Property</span></span>|<span data-ttu-id="5df99-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5df99-130">Type</span></span>|<span data-ttu-id="5df99-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5df99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5df99-132">id</span><span class="sxs-lookup"><span data-stu-id="5df99-132">id</span></span>|<span data-ttu-id="5df99-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5df99-133">String</span></span>|<span data-ttu-id="5df99-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5df99-134">Key of the entity.</span></span> <span data-ttu-id="5df99-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5df99-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5df99-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df99-137">DateTimeOffset</span></span>|<span data-ttu-id="5df99-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5df99-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5df99-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5df99-140">roleScopeTagIds</span></span>|<span data-ttu-id="5df99-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5df99-141">String collection</span></span>|<span data-ttu-id="5df99-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5df99-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5df99-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5df99-144">supportsScopeTags</span></span>|<span data-ttu-id="5df99-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="5df99-145">Boolean</span></span>|<span data-ttu-id="5df99-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5df99-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5df99-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5df99-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5df99-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5df99-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5df99-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5df99-149">This property is read-only.</span></span> <span data-ttu-id="5df99-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5df99-151">createdDateTime</span></span>|<span data-ttu-id="5df99-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5df99-152">DateTimeOffset</span></span>|<span data-ttu-id="5df99-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5df99-153">DateTime the object was created.</span></span> <span data-ttu-id="5df99-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-155">description</span><span class="sxs-lookup"><span data-stu-id="5df99-155">description</span></span>|<span data-ttu-id="5df99-156">String</span><span class="sxs-lookup"><span data-stu-id="5df99-156">String</span></span>|<span data-ttu-id="5df99-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5df99-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5df99-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5df99-159">displayName</span></span>|<span data-ttu-id="5df99-160">String</span><span class="sxs-lookup"><span data-stu-id="5df99-160">String</span></span>|<span data-ttu-id="5df99-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5df99-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5df99-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-163">version</span><span class="sxs-lookup"><span data-stu-id="5df99-163">version</span></span>|<span data-ttu-id="5df99-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5df99-164">Int32</span></span>|<span data-ttu-id="5df99-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5df99-165">Version of the device configuration.</span></span> <span data-ttu-id="5df99-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5df99-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="5df99-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="5df99-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5df99-168">Int32</span></span>|<span data-ttu-id="5df99-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="5df99-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5df99-170">Допустимые значения — от 1 до 99, наСледуемые от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5df99-170">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5df99-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5df99-171">subjectNameFormat</span></span>|[<span data-ttu-id="5df99-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="5df99-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="5df99-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5df99-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="5df99-174">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-174">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5df99-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5df99-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="5df99-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5df99-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5df99-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5df99-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5df99-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="5df99-178">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="5df99-179">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-179">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5df99-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5df99-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5df99-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5df99-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5df99-182">Int32</span><span class="sxs-lookup"><span data-stu-id="5df99-182">Int32</span></span>|<span data-ttu-id="5df99-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5df99-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="5df99-184">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5df99-184">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5df99-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5df99-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5df99-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5df99-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5df99-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5df99-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5df99-188">НаСледуется от [используется](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5df99-188">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="5df99-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5df99-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5df99-190">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="5df99-190">certificationAuthority</span></span>|<span data-ttu-id="5df99-191">String</span><span class="sxs-lookup"><span data-stu-id="5df99-191">String</span></span>|<span data-ttu-id="5df99-192">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="5df99-192">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="5df99-193">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="5df99-193">certificationAuthorityName</span></span>|<span data-ttu-id="5df99-194">String</span><span class="sxs-lookup"><span data-stu-id="5df99-194">String</span></span>|<span data-ttu-id="5df99-195">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="5df99-195">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="5df99-196">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="5df99-196">certificateTemplateName</span></span>|<span data-ttu-id="5df99-197">String</span><span class="sxs-lookup"><span data-stu-id="5df99-197">String</span></span>|<span data-ttu-id="5df99-198">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="5df99-198">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="5df99-199">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="5df99-199">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="5df99-200">String</span><span class="sxs-lookup"><span data-stu-id="5df99-200">String</span></span>|<span data-ttu-id="5df99-201">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="5df99-201">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="5df99-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="5df99-202">Response</span></span>
<span data-ttu-id="5df99-203">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5df99-203">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5df99-204">Пример</span><span class="sxs-lookup"><span data-stu-id="5df99-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="5df99-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="5df99-205">Request</span></span>
<span data-ttu-id="5df99-206">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5df99-206">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5df99-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="5df99-207">Response</span></span>
<span data-ttu-id="5df99-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5df99-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




