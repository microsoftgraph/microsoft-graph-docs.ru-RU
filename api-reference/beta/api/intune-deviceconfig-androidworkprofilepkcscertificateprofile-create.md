---
title: Создание Андроидворкпрофилепкксцертификатепрофиле
description: Создание нового объекта Андроидворкпрофилепкксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21e2af61ef6d378b29baf257ac39ba6cf66700f6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928374"
---
# <a name="create-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="03e96-103">Создание Андроидворкпрофилепкксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="03e96-103">Create androidWorkProfilePkcsCertificateProfile</span></span>

> <span data-ttu-id="03e96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03e96-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03e96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e96-106">Создание нового объекта [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03e96-106">Create a new [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03e96-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03e96-107">Prerequisites</span></span>
<span data-ttu-id="03e96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e96-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03e96-110">Permission type</span></span>|<span data-ttu-id="03e96-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03e96-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03e96-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03e96-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03e96-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e96-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03e96-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03e96-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03e96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e96-115">Not supported.</span></span>|
|<span data-ttu-id="03e96-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03e96-116">Application</span></span>|<span data-ttu-id="03e96-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e96-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03e96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03e96-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="03e96-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03e96-119">Request headers</span></span>
|<span data-ttu-id="03e96-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03e96-120">Header</span></span>|<span data-ttu-id="03e96-121">Значение</span><span class="sxs-lookup"><span data-stu-id="03e96-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03e96-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03e96-122">Authorization</span></span>|<span data-ttu-id="03e96-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03e96-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03e96-124">Accept</span><span class="sxs-lookup"><span data-stu-id="03e96-124">Accept</span></span>|<span data-ttu-id="03e96-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03e96-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e96-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03e96-126">Request body</span></span>
<span data-ttu-id="03e96-127">В тексте запроса добавьте представление объекта Андроидворкпрофилепкксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03e96-127">In the request body, supply a JSON representation for the androidWorkProfilePkcsCertificateProfile object.</span></span>

<span data-ttu-id="03e96-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилепкксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="03e96-128">The following table shows the properties that are required when you create the androidWorkProfilePkcsCertificateProfile.</span></span>

|<span data-ttu-id="03e96-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="03e96-129">Property</span></span>|<span data-ttu-id="03e96-130">Тип</span><span class="sxs-lookup"><span data-stu-id="03e96-130">Type</span></span>|<span data-ttu-id="03e96-131">Описание</span><span class="sxs-lookup"><span data-stu-id="03e96-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e96-132">id</span><span class="sxs-lookup"><span data-stu-id="03e96-132">id</span></span>|<span data-ttu-id="03e96-133">String</span><span class="sxs-lookup"><span data-stu-id="03e96-133">String</span></span>|<span data-ttu-id="03e96-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03e96-134">Key of the entity.</span></span> <span data-ttu-id="03e96-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03e96-136">lastModifiedDateTime</span></span>|<span data-ttu-id="03e96-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e96-137">DateTimeOffset</span></span>|<span data-ttu-id="03e96-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="03e96-138">DateTime the object was last modified.</span></span> <span data-ttu-id="03e96-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03e96-140">roleScopeTagIds</span></span>|<span data-ttu-id="03e96-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="03e96-141">String collection</span></span>|<span data-ttu-id="03e96-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="03e96-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03e96-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="03e96-144">supportsScopeTags</span></span>|<span data-ttu-id="03e96-145">Логический</span><span class="sxs-lookup"><span data-stu-id="03e96-145">Boolean</span></span>|<span data-ttu-id="03e96-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="03e96-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03e96-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="03e96-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03e96-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="03e96-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03e96-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03e96-149">This property is read-only.</span></span> <span data-ttu-id="03e96-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03e96-151">createdDateTime</span></span>|<span data-ttu-id="03e96-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e96-152">DateTimeOffset</span></span>|<span data-ttu-id="03e96-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="03e96-153">DateTime the object was created.</span></span> <span data-ttu-id="03e96-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-155">description</span><span class="sxs-lookup"><span data-stu-id="03e96-155">description</span></span>|<span data-ttu-id="03e96-156">String</span><span class="sxs-lookup"><span data-stu-id="03e96-156">String</span></span>|<span data-ttu-id="03e96-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03e96-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03e96-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-159">displayName</span><span class="sxs-lookup"><span data-stu-id="03e96-159">displayName</span></span>|<span data-ttu-id="03e96-160">Строка</span><span class="sxs-lookup"><span data-stu-id="03e96-160">String</span></span>|<span data-ttu-id="03e96-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03e96-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03e96-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-163">version</span><span class="sxs-lookup"><span data-stu-id="03e96-163">version</span></span>|<span data-ttu-id="03e96-164">Int32</span><span class="sxs-lookup"><span data-stu-id="03e96-164">Int32</span></span>|<span data-ttu-id="03e96-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03e96-165">Version of the device configuration.</span></span> <span data-ttu-id="03e96-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e96-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="03e96-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="03e96-168">Int32</span><span class="sxs-lookup"><span data-stu-id="03e96-168">Int32</span></span>|<span data-ttu-id="03e96-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="03e96-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="03e96-170">Допустимые значения — от 1 до 99, наследуемые от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03e96-170">Valid values 1 to 99 Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03e96-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03e96-171">subjectNameFormat</span></span>|[<span data-ttu-id="03e96-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03e96-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="03e96-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="03e96-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="03e96-174">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-174">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="03e96-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="03e96-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="03e96-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="03e96-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="03e96-177">Int32</span><span class="sxs-lookup"><span data-stu-id="03e96-177">Int32</span></span>|<span data-ttu-id="03e96-178">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="03e96-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="03e96-179">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03e96-179">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03e96-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03e96-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="03e96-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03e96-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="03e96-182">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="03e96-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="03e96-183">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-183">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="03e96-184">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="03e96-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="03e96-185">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="03e96-185">extendedKeyUsages</span></span>|<span data-ttu-id="03e96-186">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="03e96-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="03e96-187">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="03e96-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="03e96-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="03e96-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="03e96-189">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03e96-189">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03e96-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03e96-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="03e96-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03e96-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="03e96-192">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="03e96-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="03e96-193">Наследуется от [андроидворкпрофилецертификатепрофилебасе](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e96-193">Inherited from [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md).</span></span> <span data-ttu-id="03e96-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="03e96-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="03e96-195">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="03e96-195">certificationAuthority</span></span>|<span data-ttu-id="03e96-196">Строка</span><span class="sxs-lookup"><span data-stu-id="03e96-196">String</span></span>|<span data-ttu-id="03e96-197">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="03e96-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="03e96-198">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="03e96-198">certificationAuthorityName</span></span>|<span data-ttu-id="03e96-199">Строка</span><span class="sxs-lookup"><span data-stu-id="03e96-199">String</span></span>|<span data-ttu-id="03e96-200">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="03e96-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="03e96-201">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="03e96-201">certificateTemplateName</span></span>|<span data-ttu-id="03e96-202">Строка</span><span class="sxs-lookup"><span data-stu-id="03e96-202">String</span></span>|<span data-ttu-id="03e96-203">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="03e96-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="03e96-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="03e96-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="03e96-205">Строка</span><span class="sxs-lookup"><span data-stu-id="03e96-205">String</span></span>|<span data-ttu-id="03e96-206">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="03e96-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="03e96-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="03e96-207">Response</span></span>
<span data-ttu-id="03e96-208">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилепкксцертификатепрофиле](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03e96-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e96-209">Пример</span><span class="sxs-lookup"><span data-stu-id="03e96-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="03e96-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="03e96-210">Request</span></span>
<span data-ttu-id="03e96-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03e96-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 969

{
  "@odata.type": "#microsoft.graph.androidWorkProfilePkcsCertificateProfile",
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
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="03e96-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="03e96-212">Response</span></span>
<span data-ttu-id="03e96-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03e96-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "subjectAlternativeNameType": "emailAddress",
  "certificationAuthority": "Certification Authority value",
  "certificationAuthorityName": "Certification Authority Name value",
  "certificateTemplateName": "Certificate Template Name value",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




