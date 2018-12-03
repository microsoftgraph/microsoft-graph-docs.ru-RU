---
title: Создание androidWorkProfilePkcsCertificateProfile
description: Создание нового объекта androidWorkProfilePkcsCertificateProfile.
ms.openlocfilehash: 23f2a34bcd4d947856d63aa2e93426d65d100fbc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078650"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="85630-103">Создание androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="85630-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="85630-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85630-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85630-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85630-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85630-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="85630-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85630-107">Создание нового объекта [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="85630-107">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="85630-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85630-108">Prerequisites</span></span>
<span data-ttu-id="85630-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85630-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85630-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85630-111">Permission type</span></span>|<span data-ttu-id="85630-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85630-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85630-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85630-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85630-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85630-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85630-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85630-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85630-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85630-116">Not supported.</span></span>|
|<span data-ttu-id="85630-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85630-117">Application</span></span>|<span data-ttu-id="85630-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85630-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85630-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85630-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85630-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85630-120">Request headers</span></span>
|<span data-ttu-id="85630-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85630-121">Header</span></span>|<span data-ttu-id="85630-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85630-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85630-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85630-123">Authorization</span></span>|<span data-ttu-id="85630-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="85630-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85630-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85630-125">Accept</span></span>|<span data-ttu-id="85630-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85630-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85630-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85630-127">Request body</span></span>
<span data-ttu-id="85630-128">В тексте запроса укажите представление JSON для объекта androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="85630-128">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="85630-129">В следующей таблице показаны свойства, которые необходимы для создания androidWorkProfilePkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="85630-129">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="85630-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="85630-130">Property</span></span>|<span data-ttu-id="85630-131">Тип</span><span class="sxs-lookup"><span data-stu-id="85630-131">Type</span></span>|<span data-ttu-id="85630-132">Описание</span><span class="sxs-lookup"><span data-stu-id="85630-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85630-133">id</span><span class="sxs-lookup"><span data-stu-id="85630-133">id</span></span>|<span data-ttu-id="85630-134">String</span><span class="sxs-lookup"><span data-stu-id="85630-134">String</span></span>|<span data-ttu-id="85630-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85630-135">Key of the entity.</span></span> <span data-ttu-id="85630-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85630-137">lastModifiedDateTime</span></span>|<span data-ttu-id="85630-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85630-138">DateTimeOffset</span></span>|<span data-ttu-id="85630-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="85630-139">DateTime the object was last modified.</span></span> <span data-ttu-id="85630-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85630-141">roleScopeTagIds</span></span>|<span data-ttu-id="85630-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="85630-142">String collection</span></span>|<span data-ttu-id="85630-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="85630-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85630-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="85630-145">supportsScopeTags</span></span>|<span data-ttu-id="85630-146">Логический</span><span class="sxs-lookup"><span data-stu-id="85630-146">Boolean</span></span>|<span data-ttu-id="85630-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="85630-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85630-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="85630-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85630-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="85630-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85630-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85630-150">This property is read-only.</span></span> <span data-ttu-id="85630-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85630-152">createdDateTime</span></span>|<span data-ttu-id="85630-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85630-153">DateTimeOffset</span></span>|<span data-ttu-id="85630-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="85630-154">DateTime the object was created.</span></span> <span data-ttu-id="85630-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-156">описание</span><span class="sxs-lookup"><span data-stu-id="85630-156">description</span></span>|<span data-ttu-id="85630-157">String</span><span class="sxs-lookup"><span data-stu-id="85630-157">String</span></span>|<span data-ttu-id="85630-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85630-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85630-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-160">displayName</span><span class="sxs-lookup"><span data-stu-id="85630-160">displayName</span></span>|<span data-ttu-id="85630-161">String</span><span class="sxs-lookup"><span data-stu-id="85630-161">String</span></span>|<span data-ttu-id="85630-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85630-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85630-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-164">version</span><span class="sxs-lookup"><span data-stu-id="85630-164">version</span></span>|<span data-ttu-id="85630-165">Int32</span><span class="sxs-lookup"><span data-stu-id="85630-165">Int32</span></span>|<span data-ttu-id="85630-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="85630-166">Version of the device configuration.</span></span> <span data-ttu-id="85630-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85630-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85630-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="85630-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="85630-169">Int32</span><span class="sxs-lookup"><span data-stu-id="85630-169">Int32</span></span>|<span data-ttu-id="85630-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="85630-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="85630-171">Допустимые значения от 1 до 99 унаследованные от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="85630-171">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="85630-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="85630-172">subjectNameFormat</span></span>|[<span data-ttu-id="85630-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="85630-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="85630-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="85630-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="85630-175">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="85630-175">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="85630-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="85630-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="85630-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="85630-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="85630-178">Int32</span><span class="sxs-lookup"><span data-stu-id="85630-178">Int32</span></span>|<span data-ttu-id="85630-179">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="85630-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="85630-180">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="85630-180">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="85630-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="85630-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="85630-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="85630-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="85630-183">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="85630-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="85630-184">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="85630-184">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="85630-185">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="85630-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="85630-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="85630-186">extendedKeyUsages</span></span>|<span data-ttu-id="85630-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="85630-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="85630-188">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="85630-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="85630-189">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="85630-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="85630-190">Наследуется от [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="85630-190">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="85630-191">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="85630-191">certificationAuthority</span></span>|<span data-ttu-id="85630-192">String</span><span class="sxs-lookup"><span data-stu-id="85630-192">String</span></span>|<span data-ttu-id="85630-193">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="85630-193">PKCS Certification Authority</span></span>|
|<span data-ttu-id="85630-194">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="85630-194">certificationAuthorityName</span></span>|<span data-ttu-id="85630-195">String</span><span class="sxs-lookup"><span data-stu-id="85630-195">String</span></span>|<span data-ttu-id="85630-196">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="85630-196">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="85630-197">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="85630-197">certificateTemplateName</span></span>|<span data-ttu-id="85630-198">String</span><span class="sxs-lookup"><span data-stu-id="85630-198">String</span></span>|<span data-ttu-id="85630-199">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="85630-199">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="85630-200">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="85630-200">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="85630-201">String</span><span class="sxs-lookup"><span data-stu-id="85630-201">String</span></span>|<span data-ttu-id="85630-202">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="85630-202">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="85630-203">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="85630-203">subjectAlternativeNameType</span></span>|[<span data-ttu-id="85630-204">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="85630-204">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="85630-205">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="85630-205">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="85630-206">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="85630-206">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="85630-207">Ответ</span><span class="sxs-lookup"><span data-stu-id="85630-207">Response</span></span>
<span data-ttu-id="85630-208">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85630-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85630-209">Пример</span><span class="sxs-lookup"><span data-stu-id="85630-209">Example</span></span>
### <a name="request"></a><span data-ttu-id="85630-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="85630-210">Request</span></span>
<span data-ttu-id="85630-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85630-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1033

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="85630-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="85630-212">Response</span></span>
<span data-ttu-id="85630-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="85630-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1141

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
  "id": "a7d4a505-a505-a7d4-05a5-d4a705a5d4a7",
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
  "subjectNameFormat": "commonNameIncludingEmail",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "subjectAlternativeNameType": "emailAddress"
}
```





