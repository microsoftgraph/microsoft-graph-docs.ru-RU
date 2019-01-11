---
title: Обновление iosPkcsCertificateProfile
description: Обновление свойства объекта iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1cd5426ad8d07984ff25209326d613add09cc000
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817803"
---
# <a name="update-iospkcscertificateprofile"></a><span data-ttu-id="605a0-103">Обновление iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="605a0-103">Update iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="605a0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="605a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="605a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="605a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="605a0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="605a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="605a0-107">Обновление свойства объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="605a0-107">Update the properties of a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="605a0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="605a0-108">Prerequisites</span></span>
<span data-ttu-id="605a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="605a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="605a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="605a0-111">Permission type</span></span>|<span data-ttu-id="605a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="605a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="605a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="605a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="605a0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="605a0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="605a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="605a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="605a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="605a0-116">Not supported.</span></span>|
|<span data-ttu-id="605a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="605a0-117">Application</span></span>|<span data-ttu-id="605a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="605a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="605a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="605a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="605a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="605a0-120">Request headers</span></span>
|<span data-ttu-id="605a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="605a0-121">Header</span></span>|<span data-ttu-id="605a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="605a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="605a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="605a0-123">Authorization</span></span>|<span data-ttu-id="605a0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="605a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="605a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="605a0-125">Accept</span></span>|<span data-ttu-id="605a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="605a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="605a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="605a0-127">Request body</span></span>
<span data-ttu-id="605a0-128">В тексте запроса укажите представление JSON для объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="605a0-128">In the request body, supply a JSON representation for the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="605a0-129">В следующей таблице показаны свойства, которые необходимы для создания [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-129">The following table shows the properties that are required when you create the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

|<span data-ttu-id="605a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="605a0-130">Property</span></span>|<span data-ttu-id="605a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="605a0-131">Type</span></span>|<span data-ttu-id="605a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="605a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="605a0-133">id</span><span class="sxs-lookup"><span data-stu-id="605a0-133">id</span></span>|<span data-ttu-id="605a0-134">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-134">String</span></span>|<span data-ttu-id="605a0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="605a0-135">Key of the entity.</span></span> <span data-ttu-id="605a0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="605a0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="605a0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="605a0-138">DateTimeOffset</span></span>|<span data-ttu-id="605a0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="605a0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="605a0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="605a0-141">roleScopeTagIds</span></span>|<span data-ttu-id="605a0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="605a0-142">String collection</span></span>|<span data-ttu-id="605a0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="605a0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="605a0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="605a0-145">supportsScopeTags</span></span>|<span data-ttu-id="605a0-146">Логический</span><span class="sxs-lookup"><span data-stu-id="605a0-146">Boolean</span></span>|<span data-ttu-id="605a0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="605a0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="605a0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="605a0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="605a0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="605a0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="605a0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="605a0-150">This property is read-only.</span></span> <span data-ttu-id="605a0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="605a0-152">createdDateTime</span></span>|<span data-ttu-id="605a0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="605a0-153">DateTimeOffset</span></span>|<span data-ttu-id="605a0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="605a0-154">DateTime the object was created.</span></span> <span data-ttu-id="605a0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-156">описание</span><span class="sxs-lookup"><span data-stu-id="605a0-156">description</span></span>|<span data-ttu-id="605a0-157">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-157">String</span></span>|<span data-ttu-id="605a0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="605a0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="605a0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="605a0-160">displayName</span></span>|<span data-ttu-id="605a0-161">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-161">String</span></span>|<span data-ttu-id="605a0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="605a0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="605a0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-164">version</span><span class="sxs-lookup"><span data-stu-id="605a0-164">version</span></span>|<span data-ttu-id="605a0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="605a0-165">Int32</span></span>|<span data-ttu-id="605a0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="605a0-166">Version of the device configuration.</span></span> <span data-ttu-id="605a0-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="605a0-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="605a0-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="605a0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="605a0-169">Int32</span></span>|<span data-ttu-id="605a0-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="605a0-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="605a0-171">Допустимые значения от 1 до 99 унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="605a0-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="605a0-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="605a0-172">subjectNameFormat</span></span>|[<span data-ttu-id="605a0-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="605a0-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="605a0-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="605a0-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="605a0-175">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="605a0-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="605a0-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="605a0-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="605a0-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="605a0-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="605a0-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="605a0-179">Тип имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="605a0-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="605a0-180">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="605a0-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="605a0-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="605a0-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="605a0-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="605a0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="605a0-183">Int32</span></span>|<span data-ttu-id="605a0-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="605a0-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="605a0-185">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="605a0-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="605a0-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="605a0-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="605a0-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="605a0-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="605a0-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="605a0-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="605a0-189">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="605a0-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="605a0-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="605a0-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="605a0-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="605a0-191">certificationAuthority</span></span>|<span data-ttu-id="605a0-192">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-192">String</span></span>|<span data-ttu-id="605a0-193">PKCS центром сертификации.</span><span class="sxs-lookup"><span data-stu-id="605a0-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="605a0-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="605a0-194">certificationAuthorityName</span></span>|<span data-ttu-id="605a0-195">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-195">String</span></span>|<span data-ttu-id="605a0-196">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="605a0-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="605a0-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="605a0-197">certificateTemplateName</span></span>|<span data-ttu-id="605a0-198">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-198">String</span></span>|<span data-ttu-id="605a0-199">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="605a0-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="605a0-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="605a0-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="605a0-201">Строка</span><span class="sxs-lookup"><span data-stu-id="605a0-201">String</span></span>|<span data-ttu-id="605a0-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="605a0-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="605a0-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="605a0-203">Response</span></span>
<span data-ttu-id="605a0-204">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="605a0-204">If successful, this method returns a `200 OK` response code and an updated [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="605a0-205">Пример</span><span class="sxs-lookup"><span data-stu-id="605a0-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="605a0-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="605a0-206">Request</span></span>
<span data-ttu-id="605a0-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="605a0-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 761

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="605a0-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="605a0-208">Response</span></span>
<span data-ttu-id="605a0-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="605a0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





