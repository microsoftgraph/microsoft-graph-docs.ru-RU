---
title: Создание iosScepCertificateProfile
description: Создание нового объекта iosScepCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4048e008fdfab4aeae8485680e9d2c8c19c468be
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423449"
---
# <a name="create-iosscepcertificateprofile"></a><span data-ttu-id="54880-103">Создание iosScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="54880-103">Create iosScepCertificateProfile</span></span>

> <span data-ttu-id="54880-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54880-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54880-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54880-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54880-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54880-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54880-107">Создание нового объекта [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="54880-107">Create a new [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54880-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="54880-108">Prerequisites</span></span>
<span data-ttu-id="54880-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54880-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54880-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54880-111">Permission type</span></span>|<span data-ttu-id="54880-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54880-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54880-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54880-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54880-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54880-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54880-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54880-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54880-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54880-116">Not supported.</span></span>|
|<span data-ttu-id="54880-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54880-117">Application</span></span>|<span data-ttu-id="54880-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54880-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54880-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54880-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54880-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54880-120">Request headers</span></span>
|<span data-ttu-id="54880-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54880-121">Header</span></span>|<span data-ttu-id="54880-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54880-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54880-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54880-123">Authorization</span></span>|<span data-ttu-id="54880-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54880-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54880-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54880-125">Accept</span></span>|<span data-ttu-id="54880-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54880-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54880-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54880-127">Request body</span></span>
<span data-ttu-id="54880-128">В тексте запроса укажите представление JSON для объекта iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="54880-128">In the request body, supply a JSON representation for the iosScepCertificateProfile object.</span></span>

<span data-ttu-id="54880-129">В следующей таблице показаны свойства, которые необходимы для создания iosScepCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="54880-129">The following table shows the properties that are required when you create the iosScepCertificateProfile.</span></span>

|<span data-ttu-id="54880-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54880-130">Property</span></span>|<span data-ttu-id="54880-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54880-131">Type</span></span>|<span data-ttu-id="54880-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54880-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54880-133">id</span><span class="sxs-lookup"><span data-stu-id="54880-133">id</span></span>|<span data-ttu-id="54880-134">String</span><span class="sxs-lookup"><span data-stu-id="54880-134">String</span></span>|<span data-ttu-id="54880-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54880-135">Key of the entity.</span></span> <span data-ttu-id="54880-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54880-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54880-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54880-138">DateTimeOffset</span></span>|<span data-ttu-id="54880-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54880-139">DateTime the object was last modified.</span></span> <span data-ttu-id="54880-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54880-141">roleScopeTagIds</span></span>|<span data-ttu-id="54880-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54880-142">String collection</span></span>|<span data-ttu-id="54880-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="54880-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54880-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54880-145">supportsScopeTags</span></span>|<span data-ttu-id="54880-146">Логический</span><span class="sxs-lookup"><span data-stu-id="54880-146">Boolean</span></span>|<span data-ttu-id="54880-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="54880-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54880-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="54880-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54880-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="54880-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54880-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54880-150">This property is read-only.</span></span> <span data-ttu-id="54880-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54880-152">createdDateTime</span></span>|<span data-ttu-id="54880-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54880-153">DateTimeOffset</span></span>|<span data-ttu-id="54880-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54880-154">DateTime the object was created.</span></span> <span data-ttu-id="54880-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-156">description</span><span class="sxs-lookup"><span data-stu-id="54880-156">description</span></span>|<span data-ttu-id="54880-157">String</span><span class="sxs-lookup"><span data-stu-id="54880-157">String</span></span>|<span data-ttu-id="54880-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54880-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54880-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-160">displayName</span><span class="sxs-lookup"><span data-stu-id="54880-160">displayName</span></span>|<span data-ttu-id="54880-161">String</span><span class="sxs-lookup"><span data-stu-id="54880-161">String</span></span>|<span data-ttu-id="54880-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54880-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54880-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-164">version</span><span class="sxs-lookup"><span data-stu-id="54880-164">version</span></span>|<span data-ttu-id="54880-165">Int32</span><span class="sxs-lookup"><span data-stu-id="54880-165">Int32</span></span>|<span data-ttu-id="54880-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54880-166">Version of the device configuration.</span></span> <span data-ttu-id="54880-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54880-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54880-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="54880-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="54880-169">Int32</span><span class="sxs-lookup"><span data-stu-id="54880-169">Int32</span></span>|<span data-ttu-id="54880-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="54880-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="54880-171">Допустимые значения от 1 до 99 унаследованные от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="54880-171">Valid values 1 to 99 Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="54880-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="54880-172">subjectNameFormat</span></span>|[<span data-ttu-id="54880-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="54880-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="54880-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="54880-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="54880-175">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54880-175">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="54880-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="54880-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="54880-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="54880-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="54880-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="54880-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="54880-179">Тип имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="54880-179">Certificate Subject Alternative Name type.</span></span> <span data-ttu-id="54880-180">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54880-180">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="54880-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="54880-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="54880-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="54880-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="54880-183">Int32</span><span class="sxs-lookup"><span data-stu-id="54880-183">Int32</span></span>|<span data-ttu-id="54880-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="54880-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="54880-185">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="54880-185">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="54880-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54880-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="54880-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="54880-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="54880-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="54880-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="54880-189">Наследуется от [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="54880-189">Inherited from [iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md).</span></span> <span data-ttu-id="54880-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="54880-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="54880-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="54880-191">scepServerUrls</span></span>|<span data-ttu-id="54880-192">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54880-192">String collection</span></span>|<span data-ttu-id="54880-193">URL-адреса сервера SCEP.</span><span class="sxs-lookup"><span data-stu-id="54880-193">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="54880-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="54880-194">subjectNameFormatString</span></span>|<span data-ttu-id="54880-195">String</span><span class="sxs-lookup"><span data-stu-id="54880-195">String</span></span>|<span data-ttu-id="54880-196">Пользовательский формат для использования с SubjectNameFormat = пользовательский.</span><span class="sxs-lookup"><span data-stu-id="54880-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="54880-197">Например: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = корпоративных пользователей, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="54880-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="54880-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="54880-198">keyUsage</span></span>|[<span data-ttu-id="54880-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="54880-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="54880-200">SCEP использования ключа.</span><span class="sxs-lookup"><span data-stu-id="54880-200">SCEP Key Usage.</span></span> <span data-ttu-id="54880-201">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="54880-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="54880-202">keySize</span><span class="sxs-lookup"><span data-stu-id="54880-202">keySize</span></span>|[<span data-ttu-id="54880-203">keySize</span><span class="sxs-lookup"><span data-stu-id="54880-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="54880-204">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="54880-204">SCEP Key Size.</span></span> <span data-ttu-id="54880-205">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="54880-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="54880-206">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="54880-206">extendedKeyUsages</span></span>|<span data-ttu-id="54880-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="54880-207">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="54880-208">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="54880-208">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="54880-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="54880-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="54880-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="54880-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="54880-211">String</span><span class="sxs-lookup"><span data-stu-id="54880-211">String</span></span>|<span data-ttu-id="54880-212">Пользовательская строка, которая определяет атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="54880-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="54880-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="54880-213">certificateStore</span></span>|[<span data-ttu-id="54880-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="54880-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="54880-215">Целевой хранилища сертификатов.</span><span class="sxs-lookup"><span data-stu-id="54880-215">Target store certificate.</span></span> <span data-ttu-id="54880-216">Возможные значения: `user`, `machine`.</span><span class="sxs-lookup"><span data-stu-id="54880-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="54880-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="54880-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="54880-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="54880-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="54880-219">Параметры Alterantive имя настраиваемой темы.</span><span class="sxs-lookup"><span data-stu-id="54880-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="54880-220">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="54880-220">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="54880-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="54880-221">Response</span></span>
<span data-ttu-id="54880-222">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54880-222">If successful, this method returns a `201 Created` response code and a [iosScepCertificateProfile](../resources/intune-deviceconfig-iosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54880-223">Пример</span><span class="sxs-lookup"><span data-stu-id="54880-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="54880-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="54880-224">Request</span></span>
<span data-ttu-id="54880-225">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54880-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54880-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="54880-226">Response</span></span>
<span data-ttu-id="54880-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54880-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




