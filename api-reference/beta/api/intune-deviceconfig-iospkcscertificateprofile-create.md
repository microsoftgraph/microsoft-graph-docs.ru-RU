---
title: Создание iosPkcsCertificateProfile
description: Создание нового объекта iosPkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cb5f93296d7117cd003d807afbdf19211d607a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396261"
---
# <a name="create-iospkcscertificateprofile"></a><span data-ttu-id="3a8af-103">Создание iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3a8af-103">Create iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="3a8af-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a8af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a8af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a8af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a8af-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a8af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a8af-107">Создание нового объекта [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3a8af-107">Create a new [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a8af-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="3a8af-108">Prerequisites</span></span>
<span data-ttu-id="3a8af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a8af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a8af-111">Permission type</span></span>|<span data-ttu-id="3a8af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a8af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a8af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a8af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a8af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a8af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3a8af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a8af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a8af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a8af-116">Not supported.</span></span>|
|<span data-ttu-id="3a8af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a8af-117">Application</span></span>|<span data-ttu-id="3a8af-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a8af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a8af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a8af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3a8af-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a8af-120">Request headers</span></span>
|<span data-ttu-id="3a8af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a8af-121">Header</span></span>|<span data-ttu-id="3a8af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a8af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a8af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a8af-123">Authorization</span></span>|<span data-ttu-id="3a8af-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3a8af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a8af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a8af-125">Accept</span></span>|<span data-ttu-id="3a8af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a8af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a8af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a8af-127">Request body</span></span>
<span data-ttu-id="3a8af-128">В тексте запроса укажите представление JSON для объекта iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3a8af-128">In the request body, supply a JSON representation for the iosPkcsCertificateProfile object.</span></span>

<span data-ttu-id="3a8af-129">В следующей таблице показаны свойства, которые необходимы для создания iosPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="3a8af-129">The following table shows the properties that are required when you create the iosPkcsCertificateProfile.</span></span>

|<span data-ttu-id="3a8af-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a8af-130">Property</span></span>|<span data-ttu-id="3a8af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a8af-131">Type</span></span>|<span data-ttu-id="3a8af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a8af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a8af-133">id</span><span class="sxs-lookup"><span data-stu-id="3a8af-133">id</span></span>|<span data-ttu-id="3a8af-134">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-134">String</span></span>|<span data-ttu-id="3a8af-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3a8af-135">Key of the entity.</span></span> <span data-ttu-id="3a8af-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a8af-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3a8af-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a8af-138">DateTimeOffset</span></span>|<span data-ttu-id="3a8af-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3a8af-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3a8af-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a8af-141">roleScopeTagIds</span></span>|<span data-ttu-id="3a8af-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a8af-142">String collection</span></span>|<span data-ttu-id="3a8af-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3a8af-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3a8af-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3a8af-145">supportsScopeTags</span></span>|<span data-ttu-id="3a8af-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3a8af-146">Boolean</span></span>|<span data-ttu-id="3a8af-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3a8af-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3a8af-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3a8af-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3a8af-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3a8af-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3a8af-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a8af-150">This property is read-only.</span></span> <span data-ttu-id="3a8af-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a8af-152">createdDateTime</span></span>|<span data-ttu-id="3a8af-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a8af-153">DateTimeOffset</span></span>|<span data-ttu-id="3a8af-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3a8af-154">DateTime the object was created.</span></span> <span data-ttu-id="3a8af-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-156">description</span><span class="sxs-lookup"><span data-stu-id="3a8af-156">description</span></span>|<span data-ttu-id="3a8af-157">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-157">String</span></span>|<span data-ttu-id="3a8af-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a8af-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3a8af-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3a8af-160">displayName</span></span>|<span data-ttu-id="3a8af-161">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-161">String</span></span>|<span data-ttu-id="3a8af-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a8af-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3a8af-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-164">version</span><span class="sxs-lookup"><span data-stu-id="3a8af-164">version</span></span>|<span data-ttu-id="3a8af-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3a8af-165">Int32</span></span>|<span data-ttu-id="3a8af-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3a8af-166">Version of the device configuration.</span></span> <span data-ttu-id="3a8af-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3a8af-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3a8af-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3a8af-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3a8af-169">Int32</span></span>|<span data-ttu-id="3a8af-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="3a8af-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3a8af-171">Допустимые значения от 1 до 99 унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3a8af-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3a8af-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3a8af-172">subjectNameFormat</span></span>|[<span data-ttu-id="3a8af-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3a8af-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="3a8af-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3a8af-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="3a8af-175">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="3a8af-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="3a8af-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="3a8af-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3a8af-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3a8af-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3a8af-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3a8af-179">Тип имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="3a8af-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="3a8af-180">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="3a8af-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3a8af-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3a8af-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3a8af-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3a8af-183">Int32</span><span class="sxs-lookup"><span data-stu-id="3a8af-183">Int32</span></span>|<span data-ttu-id="3a8af-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3a8af-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="3a8af-185">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3a8af-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3a8af-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3a8af-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3a8af-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3a8af-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3a8af-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="3a8af-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="3a8af-189">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3a8af-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="3a8af-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3a8af-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3a8af-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="3a8af-191">certificationAuthority</span></span>|<span data-ttu-id="3a8af-192">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-192">String</span></span>|<span data-ttu-id="3a8af-193">PKCS центром сертификации.</span><span class="sxs-lookup"><span data-stu-id="3a8af-193">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="3a8af-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="3a8af-194">certificationAuthorityName</span></span>|<span data-ttu-id="3a8af-195">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-195">String</span></span>|<span data-ttu-id="3a8af-196">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="3a8af-196">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="3a8af-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="3a8af-197">certificateTemplateName</span></span>|<span data-ttu-id="3a8af-198">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-198">String</span></span>|<span data-ttu-id="3a8af-199">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="3a8af-199">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="3a8af-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="3a8af-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="3a8af-201">String</span><span class="sxs-lookup"><span data-stu-id="3a8af-201">String</span></span>|<span data-ttu-id="3a8af-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="3a8af-202">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="3a8af-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a8af-203">Response</span></span>
<span data-ttu-id="3a8af-204">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a8af-204">If successful, this method returns a `201 Created` response code and a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a8af-205">Пример</span><span class="sxs-lookup"><span data-stu-id="3a8af-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a8af-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a8af-206">Request</span></span>
<span data-ttu-id="3a8af-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a8af-207">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3a8af-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a8af-208">Response</span></span>
<span data-ttu-id="3a8af-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a8af-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




