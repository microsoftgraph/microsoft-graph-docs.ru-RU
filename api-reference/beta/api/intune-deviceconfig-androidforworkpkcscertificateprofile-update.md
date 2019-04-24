---
title: Обновление androidForWorkPkcsCertificateProfile
description: Обновление свойств объекта androidForWorkPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b0c108915c9af848aed5040cc39f14cd654e0e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32478387"
---
# <a name="update-androidforworkpkcscertificateprofile"></a><span data-ttu-id="81067-103">Обновление androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="81067-103">Update androidForWorkPkcsCertificateProfile</span></span>

> <span data-ttu-id="81067-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81067-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81067-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81067-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81067-106">Обновление свойств объекта [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="81067-106">Update the properties of a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81067-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="81067-107">Prerequisites</span></span>
<span data-ttu-id="81067-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81067-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81067-110">Permission type</span></span>|<span data-ttu-id="81067-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="81067-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81067-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81067-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81067-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81067-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="81067-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81067-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81067-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81067-115">Not supported.</span></span>|
|<span data-ttu-id="81067-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81067-116">Application</span></span>|<span data-ttu-id="81067-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81067-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81067-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81067-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="81067-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81067-119">Request headers</span></span>
|<span data-ttu-id="81067-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81067-120">Header</span></span>|<span data-ttu-id="81067-121">Значение</span><span class="sxs-lookup"><span data-stu-id="81067-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81067-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81067-122">Authorization</span></span>|<span data-ttu-id="81067-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81067-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81067-124">Accept</span><span class="sxs-lookup"><span data-stu-id="81067-124">Accept</span></span>|<span data-ttu-id="81067-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81067-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81067-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81067-126">Request body</span></span>
<span data-ttu-id="81067-127">В тексте запроса добавьте представление объекта [AndroidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81067-127">In the request body, supply a JSON representation for the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object.</span></span>

<span data-ttu-id="81067-128">В следующей таблице приведены свойства, необходимые при создании [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="81067-128">The following table shows the properties that are required when you create the [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

|<span data-ttu-id="81067-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="81067-129">Property</span></span>|<span data-ttu-id="81067-130">Тип</span><span class="sxs-lookup"><span data-stu-id="81067-130">Type</span></span>|<span data-ttu-id="81067-131">Описание</span><span class="sxs-lookup"><span data-stu-id="81067-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81067-132">id</span><span class="sxs-lookup"><span data-stu-id="81067-132">id</span></span>|<span data-ttu-id="81067-133">Строка</span><span class="sxs-lookup"><span data-stu-id="81067-133">String</span></span>|<span data-ttu-id="81067-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="81067-134">Key of the entity.</span></span> <span data-ttu-id="81067-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81067-136">lastModifiedDateTime</span></span>|<span data-ttu-id="81067-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81067-137">DateTimeOffset</span></span>|<span data-ttu-id="81067-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="81067-138">DateTime the object was last modified.</span></span> <span data-ttu-id="81067-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81067-140">roleScopeTagIds</span></span>|<span data-ttu-id="81067-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="81067-141">String collection</span></span>|<span data-ttu-id="81067-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="81067-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="81067-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="81067-144">supportsScopeTags</span></span>|<span data-ttu-id="81067-145">Логический</span><span class="sxs-lookup"><span data-stu-id="81067-145">Boolean</span></span>|<span data-ttu-id="81067-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="81067-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="81067-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="81067-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="81067-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="81067-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="81067-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81067-149">This property is read-only.</span></span> <span data-ttu-id="81067-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81067-151">createdDateTime</span></span>|<span data-ttu-id="81067-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81067-152">DateTimeOffset</span></span>|<span data-ttu-id="81067-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="81067-153">DateTime the object was created.</span></span> <span data-ttu-id="81067-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-155">description</span><span class="sxs-lookup"><span data-stu-id="81067-155">description</span></span>|<span data-ttu-id="81067-156">String</span><span class="sxs-lookup"><span data-stu-id="81067-156">String</span></span>|<span data-ttu-id="81067-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81067-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="81067-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-159">displayName</span><span class="sxs-lookup"><span data-stu-id="81067-159">displayName</span></span>|<span data-ttu-id="81067-160">String</span><span class="sxs-lookup"><span data-stu-id="81067-160">String</span></span>|<span data-ttu-id="81067-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81067-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="81067-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-163">version</span><span class="sxs-lookup"><span data-stu-id="81067-163">version</span></span>|<span data-ttu-id="81067-164">Int32</span><span class="sxs-lookup"><span data-stu-id="81067-164">Int32</span></span>|<span data-ttu-id="81067-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="81067-165">Version of the device configuration.</span></span> <span data-ttu-id="81067-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="81067-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="81067-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="81067-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="81067-168">Int32</span><span class="sxs-lookup"><span data-stu-id="81067-168">Int32</span></span>|<span data-ttu-id="81067-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="81067-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="81067-170">Допустимые значения — от 1 до 99, наСледуемые от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="81067-170">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="81067-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81067-171">subjectNameFormat</span></span>|[<span data-ttu-id="81067-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="81067-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="81067-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="81067-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="81067-174">НаСледуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81067-174">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="81067-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="81067-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="81067-176">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="81067-176">certificateValidityPeriodValue</span></span>|<span data-ttu-id="81067-177">Int32</span><span class="sxs-lookup"><span data-stu-id="81067-177">Int32</span></span>|<span data-ttu-id="81067-178">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="81067-178">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="81067-179">НаСледуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="81067-179">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="81067-180">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="81067-180">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="81067-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="81067-181">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="81067-182">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="81067-182">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="81067-183">НаСледуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81067-183">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="81067-184">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="81067-184">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="81067-185">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="81067-185">extendedKeyUsages</span></span>|<span data-ttu-id="81067-186">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="81067-186">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="81067-187">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="81067-187">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="81067-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="81067-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="81067-189">НаСледуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="81067-189">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="81067-190">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="81067-190">subjectAlternativeNameType</span></span>|[<span data-ttu-id="81067-191">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="81067-191">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="81067-192">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="81067-192">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="81067-193">НаСледуется от [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="81067-193">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="81067-194">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="81067-194">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="81067-195">Цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="81067-195">certificationAuthority</span></span>|<span data-ttu-id="81067-196">String</span><span class="sxs-lookup"><span data-stu-id="81067-196">String</span></span>|<span data-ttu-id="81067-197">Центр сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="81067-197">PKCS Certification Authority</span></span>|
|<span data-ttu-id="81067-198">Цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="81067-198">certificationAuthorityName</span></span>|<span data-ttu-id="81067-199">String</span><span class="sxs-lookup"><span data-stu-id="81067-199">String</span></span>|<span data-ttu-id="81067-200">Имя центра сертификации PKCS</span><span class="sxs-lookup"><span data-stu-id="81067-200">PKCS Certification Authority Name</span></span>|
|<span data-ttu-id="81067-201">Цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="81067-201">certificateTemplateName</span></span>|<span data-ttu-id="81067-202">String</span><span class="sxs-lookup"><span data-stu-id="81067-202">String</span></span>|<span data-ttu-id="81067-203">Имя шаблона сертификата PKCS</span><span class="sxs-lookup"><span data-stu-id="81067-203">PKCS Certificate Template Name</span></span>|
|<span data-ttu-id="81067-204">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="81067-204">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="81067-205">String</span><span class="sxs-lookup"><span data-stu-id="81067-205">String</span></span>|<span data-ttu-id="81067-206">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="81067-206">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="81067-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="81067-207">Response</span></span>
<span data-ttu-id="81067-208">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81067-208">If successful, this method returns a `200 OK` response code and an updated [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81067-209">Пример</span><span class="sxs-lookup"><span data-stu-id="81067-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="81067-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="81067-210">Request</span></span>
<span data-ttu-id="81067-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81067-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 965

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="81067-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="81067-212">Response</span></span>
<span data-ttu-id="81067-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81067-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1137

{
  "@odata.type": "#microsoft.graph.androidForWorkPkcsCertificateProfile",
  "id": "0a2d7691-7691-0a2d-9176-2d0a91762d0a",
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





