---
title: Обновление androidPkcsCertificateProfile
description: Обновление свойства объекта androidPkcsCertificateProfile.
ms.openlocfilehash: 44b3279bc56e6e60e3b44665b2bd939c58752ec2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078617"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="be658-103">Обновление androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="be658-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="be658-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="be658-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be658-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be658-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be658-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="be658-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be658-107">Обновление свойства объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="be658-107">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="be658-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be658-108">Prerequisites</span></span>
<span data-ttu-id="be658-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be658-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be658-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be658-111">Permission type</span></span>|<span data-ttu-id="be658-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be658-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be658-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be658-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be658-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be658-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be658-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be658-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be658-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be658-116">Not supported.</span></span>|
|<span data-ttu-id="be658-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be658-117">Application</span></span>|<span data-ttu-id="be658-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be658-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be658-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be658-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="be658-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be658-120">Request headers</span></span>
|<span data-ttu-id="be658-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be658-121">Header</span></span>|<span data-ttu-id="be658-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be658-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be658-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="be658-123">Authorization</span></span>|<span data-ttu-id="be658-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="be658-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be658-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be658-125">Accept</span></span>|<span data-ttu-id="be658-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be658-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be658-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be658-127">Request body</span></span>
<span data-ttu-id="be658-128">В тексте запроса укажите представление JSON для объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="be658-128">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="be658-129">В следующей таблице показаны свойства, которые необходимы для создания [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="be658-129">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="be658-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="be658-130">Property</span></span>|<span data-ttu-id="be658-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be658-131">Type</span></span>|<span data-ttu-id="be658-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be658-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be658-133">id</span><span class="sxs-lookup"><span data-stu-id="be658-133">id</span></span>|<span data-ttu-id="be658-134">String</span><span class="sxs-lookup"><span data-stu-id="be658-134">String</span></span>|<span data-ttu-id="be658-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be658-135">Key of the entity.</span></span> <span data-ttu-id="be658-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be658-137">lastModifiedDateTime</span></span>|<span data-ttu-id="be658-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be658-138">DateTimeOffset</span></span>|<span data-ttu-id="be658-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be658-139">DateTime the object was last modified.</span></span> <span data-ttu-id="be658-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be658-141">roleScopeTagIds</span></span>|<span data-ttu-id="be658-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="be658-142">String collection</span></span>|<span data-ttu-id="be658-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="be658-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be658-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="be658-145">supportsScopeTags</span></span>|<span data-ttu-id="be658-146">Логический</span><span class="sxs-lookup"><span data-stu-id="be658-146">Boolean</span></span>|<span data-ttu-id="be658-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="be658-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be658-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="be658-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be658-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="be658-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be658-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be658-150">This property is read-only.</span></span> <span data-ttu-id="be658-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be658-152">createdDateTime</span></span>|<span data-ttu-id="be658-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be658-153">DateTimeOffset</span></span>|<span data-ttu-id="be658-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="be658-154">DateTime the object was created.</span></span> <span data-ttu-id="be658-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-156">описание</span><span class="sxs-lookup"><span data-stu-id="be658-156">description</span></span>|<span data-ttu-id="be658-157">String</span><span class="sxs-lookup"><span data-stu-id="be658-157">String</span></span>|<span data-ttu-id="be658-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be658-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be658-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-160">displayName</span><span class="sxs-lookup"><span data-stu-id="be658-160">displayName</span></span>|<span data-ttu-id="be658-161">String</span><span class="sxs-lookup"><span data-stu-id="be658-161">String</span></span>|<span data-ttu-id="be658-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be658-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be658-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-164">version</span><span class="sxs-lookup"><span data-stu-id="be658-164">version</span></span>|<span data-ttu-id="be658-165">Int32</span><span class="sxs-lookup"><span data-stu-id="be658-165">Int32</span></span>|<span data-ttu-id="be658-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be658-166">Version of the device configuration.</span></span> <span data-ttu-id="be658-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be658-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be658-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="be658-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="be658-169">Int32</span><span class="sxs-lookup"><span data-stu-id="be658-169">Int32</span></span>|<span data-ttu-id="be658-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="be658-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="be658-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be658-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="be658-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="be658-172">subjectNameFormat</span></span>|[<span data-ttu-id="be658-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="be658-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="be658-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="be658-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="be658-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be658-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="be658-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="be658-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="be658-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="be658-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="be658-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="be658-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="be658-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="be658-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="be658-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be658-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="be658-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="be658-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="be658-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="be658-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="be658-183">Int32</span><span class="sxs-lookup"><span data-stu-id="be658-183">Int32</span></span>|<span data-ttu-id="be658-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="be658-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="be658-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be658-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="be658-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="be658-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="be658-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="be658-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="be658-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="be658-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="be658-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="be658-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="be658-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="be658-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="be658-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="be658-191">extendedKeyUsages</span></span>|<span data-ttu-id="be658-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="be658-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="be658-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="be658-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="be658-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="be658-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="be658-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="be658-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="be658-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="be658-196">certificationAuthority</span></span>|<span data-ttu-id="be658-197">String</span><span class="sxs-lookup"><span data-stu-id="be658-197">String</span></span>|<span data-ttu-id="be658-198">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="be658-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="be658-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="be658-199">certificationAuthorityName</span></span>|<span data-ttu-id="be658-200">String</span><span class="sxs-lookup"><span data-stu-id="be658-200">String</span></span>|<span data-ttu-id="be658-201">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="be658-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="be658-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="be658-202">certificateTemplateName</span></span>|<span data-ttu-id="be658-203">String</span><span class="sxs-lookup"><span data-stu-id="be658-203">String</span></span>|<span data-ttu-id="be658-204">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="be658-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="be658-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="be658-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="be658-206">String</span><span class="sxs-lookup"><span data-stu-id="be658-206">String</span></span>|<span data-ttu-id="be658-207">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="be658-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="be658-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="be658-208">Response</span></span>
<span data-ttu-id="be658-209">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="be658-209">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be658-210">Пример</span><span class="sxs-lookup"><span data-stu-id="be658-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="be658-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="be658-211">Request</span></span>
<span data-ttu-id="be658-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be658-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 954

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
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="be658-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="be658-213">Response</span></span>
<span data-ttu-id="be658-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="be658-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1130

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
  "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
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
  "subjectAlternativeNameType": "emailAddress",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```





