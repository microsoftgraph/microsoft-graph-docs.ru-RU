---
title: Обновление androidPkcsCertificateProfile
description: Обновление свойств объекта androidPkcsCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27d14392a7ef4e92346b3c31854d5570df91882e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928941"
---
# <a name="update-androidpkcscertificateprofile"></a><span data-ttu-id="f4b1f-103">Обновление androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="f4b1f-103">Update androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="f4b1f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4b1f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4b1f-106">Обновление свойств объекта [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f4b1f-106">Update the properties of a [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4b1f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4b1f-107">Prerequisites</span></span>
<span data-ttu-id="f4b1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b1f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b1f-110">Permission type</span></span>|<span data-ttu-id="f4b1f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4b1f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4b1f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b1f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f4b1f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4b1f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-115">Not supported.</span></span>|
|<span data-ttu-id="f4b1f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4b1f-116">Application</span></span>|<span data-ttu-id="f4b1f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4b1f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4b1f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f4b1f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4b1f-119">Request headers</span></span>
|<span data-ttu-id="f4b1f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4b1f-120">Header</span></span>|<span data-ttu-id="f4b1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4b1f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4b1f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4b1f-122">Authorization</span></span>|<span data-ttu-id="f4b1f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4b1f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4b1f-124">Accept</span></span>|<span data-ttu-id="f4b1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4b1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4b1f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4b1f-126">Request body</span></span>
<span data-ttu-id="f4b1f-127">В тексте запроса добавьте представление объекта [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-127">In the request body, supply a JSON representation for the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="f4b1f-128">В следующей таблице приведены свойства, необходимые при создании [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-128">The following table shows the properties that are required when you create the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="f4b1f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4b1f-129">Property</span></span>|<span data-ttu-id="f4b1f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4b1f-130">Type</span></span>|<span data-ttu-id="f4b1f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4b1f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4b1f-132">id</span><span class="sxs-lookup"><span data-stu-id="f4b1f-132">id</span></span>|<span data-ttu-id="f4b1f-133">String</span><span class="sxs-lookup"><span data-stu-id="f4b1f-133">String</span></span>|<span data-ttu-id="f4b1f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-134">Key of the entity.</span></span> <span data-ttu-id="f4b1f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b1f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f4b1f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b1f-137">DateTimeOffset</span></span>|<span data-ttu-id="f4b1f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f4b1f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4b1f-140">roleScopeTagIds</span></span>|<span data-ttu-id="f4b1f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4b1f-141">String collection</span></span>|<span data-ttu-id="f4b1f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f4b1f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f4b1f-144">supportsScopeTags</span></span>|<span data-ttu-id="f4b1f-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f4b1f-145">Boolean</span></span>|<span data-ttu-id="f4b1f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f4b1f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f4b1f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f4b1f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-149">This property is read-only.</span></span> <span data-ttu-id="f4b1f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b1f-151">createdDateTime</span></span>|<span data-ttu-id="f4b1f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4b1f-152">DateTimeOffset</span></span>|<span data-ttu-id="f4b1f-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-153">DateTime the object was created.</span></span> <span data-ttu-id="f4b1f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-155">description</span><span class="sxs-lookup"><span data-stu-id="f4b1f-155">description</span></span>|<span data-ttu-id="f4b1f-156">String</span><span class="sxs-lookup"><span data-stu-id="f4b1f-156">String</span></span>|<span data-ttu-id="f4b1f-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f4b1f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f4b1f-159">displayName</span></span>|<span data-ttu-id="f4b1f-160">Строка</span><span class="sxs-lookup"><span data-stu-id="f4b1f-160">String</span></span>|<span data-ttu-id="f4b1f-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f4b1f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-163">version</span><span class="sxs-lookup"><span data-stu-id="f4b1f-163">version</span></span>|<span data-ttu-id="f4b1f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b1f-164">Int32</span></span>|<span data-ttu-id="f4b1f-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-165">Version of the device configuration.</span></span> <span data-ttu-id="f4b1f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f4b1f-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="f4b1f-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="f4b1f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b1f-168">Int32</span></span>|<span data-ttu-id="f4b1f-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="f4b1f-170">Допустимые значения — от 1 до 99, наследуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4b1f-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4b1f-171">subjectNameFormat</span></span>|[<span data-ttu-id="f4b1f-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="f4b1f-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="f4b1f-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="f4b1f-174">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f4b1f-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="f4b1f-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4b1f-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="f4b1f-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="f4b1f-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="f4b1f-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="f4b1f-179">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f4b1f-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="f4b1f-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="f4b1f-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="f4b1f-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f4b1f-182">Int32</span></span>|<span data-ttu-id="f4b1f-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="f4b1f-184">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4b1f-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4b1f-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="f4b1f-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="f4b1f-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="f4b1f-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="f4b1f-188">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="f4b1f-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="f4b1f-190">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="f4b1f-190">extendedKeyUsages</span></span>|<span data-ttu-id="f4b1f-191">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="f4b1f-192">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="f4b1f-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="f4b1f-193">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f4b1f-194">Наследуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="f4b1f-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="f4b1f-195">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="f4b1f-195">certificationAuthority</span></span>|<span data-ttu-id="f4b1f-196">Строка</span><span class="sxs-lookup"><span data-stu-id="f4b1f-196">String</span></span>|<span data-ttu-id="f4b1f-197">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="f4b1f-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="f4b1f-198">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="f4b1f-198">certificationAuthorityName</span></span>|<span data-ttu-id="f4b1f-199">Строка</span><span class="sxs-lookup"><span data-stu-id="f4b1f-199">String</span></span>|<span data-ttu-id="f4b1f-200">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="f4b1f-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="f4b1f-201">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="f4b1f-201">certificateTemplateName</span></span>|<span data-ttu-id="f4b1f-202">Строка</span><span class="sxs-lookup"><span data-stu-id="f4b1f-202">String</span></span>|<span data-ttu-id="f4b1f-203">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="f4b1f-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="f4b1f-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="f4b1f-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="f4b1f-205">Строка</span><span class="sxs-lookup"><span data-stu-id="f4b1f-205">String</span></span>|<span data-ttu-id="f4b1f-206">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="f4b1f-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b1f-207">Response</span></span>
<span data-ttu-id="f4b1f-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-208">If successful, this method returns a `200 OK` response code and an updated [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4b1f-209">Пример</span><span class="sxs-lookup"><span data-stu-id="f4b1f-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4b1f-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4b1f-210">Request</span></span>
<span data-ttu-id="f4b1f-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f4b1f-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b1f-212">Response</span></span>
<span data-ttu-id="f4b1f-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4b1f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




