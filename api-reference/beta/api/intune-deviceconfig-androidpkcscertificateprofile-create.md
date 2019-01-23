---
title: Создание androidPkcsCertificateProfile
description: Создание нового объекта androidPkcsCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9efcf4361d168cd44bbbe16da43941d3ed1215f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395176"
---
# <a name="create-androidpkcscertificateprofile"></a><span data-ttu-id="13dd7-103">Создание androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="13dd7-103">Create androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="13dd7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13dd7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="13dd7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13dd7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13dd7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13dd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13dd7-107">Создание нового объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="13dd7-107">Create a new [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13dd7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="13dd7-108">Prerequisites</span></span>
<span data-ttu-id="13dd7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="13dd7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13dd7-111">Permission type</span></span>|<span data-ttu-id="13dd7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13dd7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13dd7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13dd7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13dd7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13dd7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="13dd7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13dd7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13dd7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13dd7-116">Not supported.</span></span>|
|<span data-ttu-id="13dd7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13dd7-117">Application</span></span>|<span data-ttu-id="13dd7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13dd7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13dd7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13dd7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="13dd7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13dd7-120">Request headers</span></span>
|<span data-ttu-id="13dd7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13dd7-121">Header</span></span>|<span data-ttu-id="13dd7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13dd7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13dd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13dd7-123">Authorization</span></span>|<span data-ttu-id="13dd7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="13dd7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13dd7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="13dd7-125">Accept</span></span>|<span data-ttu-id="13dd7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="13dd7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13dd7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13dd7-127">Request body</span></span>
<span data-ttu-id="13dd7-128">В тексте запроса укажите представление JSON для объекта androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="13dd7-128">In the request body, supply a JSON representation for the androidPkcsCertificateProfile object.</span></span>

<span data-ttu-id="13dd7-129">В следующей таблице показаны свойства, которые необходимы для создания androidPkcsCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="13dd7-129">The following table shows the properties that are required when you create the androidPkcsCertificateProfile.</span></span>

|<span data-ttu-id="13dd7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="13dd7-130">Property</span></span>|<span data-ttu-id="13dd7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="13dd7-131">Type</span></span>|<span data-ttu-id="13dd7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="13dd7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13dd7-133">id</span><span class="sxs-lookup"><span data-stu-id="13dd7-133">id</span></span>|<span data-ttu-id="13dd7-134">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-134">String</span></span>|<span data-ttu-id="13dd7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="13dd7-135">Key of the entity.</span></span> <span data-ttu-id="13dd7-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13dd7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="13dd7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13dd7-138">DateTimeOffset</span></span>|<span data-ttu-id="13dd7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="13dd7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="13dd7-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13dd7-141">roleScopeTagIds</span></span>|<span data-ttu-id="13dd7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="13dd7-142">String collection</span></span>|<span data-ttu-id="13dd7-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="13dd7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="13dd7-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="13dd7-145">supportsScopeTags</span></span>|<span data-ttu-id="13dd7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="13dd7-146">Boolean</span></span>|<span data-ttu-id="13dd7-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="13dd7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="13dd7-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="13dd7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="13dd7-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="13dd7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="13dd7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13dd7-150">This property is read-only.</span></span> <span data-ttu-id="13dd7-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13dd7-152">createdDateTime</span></span>|<span data-ttu-id="13dd7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13dd7-153">DateTimeOffset</span></span>|<span data-ttu-id="13dd7-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="13dd7-154">DateTime the object was created.</span></span> <span data-ttu-id="13dd7-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-156">description</span><span class="sxs-lookup"><span data-stu-id="13dd7-156">description</span></span>|<span data-ttu-id="13dd7-157">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-157">String</span></span>|<span data-ttu-id="13dd7-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13dd7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="13dd7-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="13dd7-160">displayName</span></span>|<span data-ttu-id="13dd7-161">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-161">String</span></span>|<span data-ttu-id="13dd7-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13dd7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="13dd7-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-164">version</span><span class="sxs-lookup"><span data-stu-id="13dd7-164">version</span></span>|<span data-ttu-id="13dd7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="13dd7-165">Int32</span></span>|<span data-ttu-id="13dd7-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="13dd7-166">Version of the device configuration.</span></span> <span data-ttu-id="13dd7-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="13dd7-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="13dd7-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="13dd7-169">Int32</span><span class="sxs-lookup"><span data-stu-id="13dd7-169">Int32</span></span>|<span data-ttu-id="13dd7-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="13dd7-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="13dd7-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13dd7-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="13dd7-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="13dd7-172">subjectNameFormat</span></span>|[<span data-ttu-id="13dd7-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="13dd7-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="13dd7-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="13dd7-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="13dd7-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="13dd7-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="13dd7-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="13dd7-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="13dd7-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="13dd7-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="13dd7-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="13dd7-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="13dd7-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="13dd7-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="13dd7-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="13dd7-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="13dd7-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="13dd7-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="13dd7-183">Int32</span><span class="sxs-lookup"><span data-stu-id="13dd7-183">Int32</span></span>|<span data-ttu-id="13dd7-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="13dd7-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="13dd7-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13dd7-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="13dd7-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="13dd7-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="13dd7-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="13dd7-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="13dd7-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="13dd7-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="13dd7-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="13dd7-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="13dd7-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="13dd7-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="13dd7-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="13dd7-191">extendedKeyUsages</span></span>|<span data-ttu-id="13dd7-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="13dd7-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="13dd7-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="13dd7-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="13dd7-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="13dd7-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="13dd7-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="13dd7-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="13dd7-196">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="13dd7-196">certificationAuthority</span></span>|<span data-ttu-id="13dd7-197">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-197">String</span></span>|<span data-ttu-id="13dd7-198">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="13dd7-198">PKCS Certification Authority</span></span>|
|<span data-ttu-id="13dd7-199">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="13dd7-199">certificationAuthorityName</span></span>|<span data-ttu-id="13dd7-200">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-200">String</span></span>|<span data-ttu-id="13dd7-201">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="13dd7-201">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="13dd7-202">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="13dd7-202">certificateTemplateName</span></span>|<span data-ttu-id="13dd7-203">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-203">String</span></span>|<span data-ttu-id="13dd7-204">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="13dd7-204">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="13dd7-205">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="13dd7-205">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="13dd7-206">String</span><span class="sxs-lookup"><span data-stu-id="13dd7-206">String</span></span>|<span data-ttu-id="13dd7-207">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="13dd7-207">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="13dd7-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="13dd7-208">Response</span></span>
<span data-ttu-id="13dd7-209">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="13dd7-209">If successful, this method returns a `201 Created` response code and a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13dd7-210">Пример</span><span class="sxs-lookup"><span data-stu-id="13dd7-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="13dd7-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="13dd7-211">Request</span></span>
<span data-ttu-id="13dd7-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13dd7-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 958

{
  "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="13dd7-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="13dd7-213">Response</span></span>
<span data-ttu-id="13dd7-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="13dd7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




