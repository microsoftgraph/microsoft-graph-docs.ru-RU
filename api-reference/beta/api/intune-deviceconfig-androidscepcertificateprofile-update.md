---
title: Обновление androidScepCertificateProfile
description: Обновление свойств объекта androidScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 182710b083ac79604cb238226084f7bee02dd5c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151508"
---
# <a name="update-androidscepcertificateprofile"></a><span data-ttu-id="7b76d-103">Обновление androidScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="7b76d-103">Update androidScepCertificateProfile</span></span>

> <span data-ttu-id="7b76d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b76d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b76d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b76d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b76d-106">Обновление свойств объекта [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="7b76d-106">Update the properties of a [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b76d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7b76d-107">Prerequisites</span></span>
<span data-ttu-id="7b76d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b76d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b76d-110">Permission type</span></span>|<span data-ttu-id="7b76d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b76d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b76d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b76d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7b76d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b76d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b76d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b76d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b76d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b76d-115">Not supported.</span></span>|
|<span data-ttu-id="7b76d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b76d-116">Application</span></span>|<span data-ttu-id="7b76d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b76d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b76d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b76d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7b76d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b76d-119">Request headers</span></span>
|<span data-ttu-id="7b76d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7b76d-120">Header</span></span>|<span data-ttu-id="7b76d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7b76d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b76d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b76d-122">Authorization</span></span>|<span data-ttu-id="7b76d-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7b76d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b76d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7b76d-124">Accept</span></span>|<span data-ttu-id="7b76d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7b76d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b76d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7b76d-126">Request body</span></span>
<span data-ttu-id="7b76d-127">В тексте запроса добавьте представление объекта [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b76d-127">In the request body, supply a JSON representation for the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="7b76d-128">В следующей таблице приведены свойства, необходимые при создании [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-128">The following table shows the properties that are required when you create the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md).</span></span>

|<span data-ttu-id="7b76d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b76d-129">Property</span></span>|<span data-ttu-id="7b76d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7b76d-130">Type</span></span>|<span data-ttu-id="7b76d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7b76d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b76d-132">id</span><span class="sxs-lookup"><span data-stu-id="7b76d-132">id</span></span>|<span data-ttu-id="7b76d-133">String</span><span class="sxs-lookup"><span data-stu-id="7b76d-133">String</span></span>|<span data-ttu-id="7b76d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7b76d-134">Key of the entity.</span></span> <span data-ttu-id="7b76d-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b76d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7b76d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b76d-137">DateTimeOffset</span></span>|<span data-ttu-id="7b76d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7b76d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7b76d-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7b76d-140">roleScopeTagIds</span></span>|<span data-ttu-id="7b76d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b76d-141">String collection</span></span>|<span data-ttu-id="7b76d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7b76d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7b76d-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7b76d-144">supportsScopeTags</span></span>|<span data-ttu-id="7b76d-145">Логический</span><span class="sxs-lookup"><span data-stu-id="7b76d-145">Boolean</span></span>|<span data-ttu-id="7b76d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7b76d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7b76d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7b76d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7b76d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7b76d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7b76d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7b76d-149">This property is read-only.</span></span> <span data-ttu-id="7b76d-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7b76d-151">createdDateTime</span></span>|<span data-ttu-id="7b76d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b76d-152">DateTimeOffset</span></span>|<span data-ttu-id="7b76d-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7b76d-153">DateTime the object was created.</span></span> <span data-ttu-id="7b76d-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-155">description</span><span class="sxs-lookup"><span data-stu-id="7b76d-155">description</span></span>|<span data-ttu-id="7b76d-156">String</span><span class="sxs-lookup"><span data-stu-id="7b76d-156">String</span></span>|<span data-ttu-id="7b76d-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b76d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7b76d-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="7b76d-159">displayName</span></span>|<span data-ttu-id="7b76d-160">String</span><span class="sxs-lookup"><span data-stu-id="7b76d-160">String</span></span>|<span data-ttu-id="7b76d-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b76d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7b76d-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-163">version</span><span class="sxs-lookup"><span data-stu-id="7b76d-163">version</span></span>|<span data-ttu-id="7b76d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7b76d-164">Int32</span></span>|<span data-ttu-id="7b76d-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7b76d-165">Version of the device configuration.</span></span> <span data-ttu-id="7b76d-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7b76d-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="7b76d-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="7b76d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7b76d-168">Int32</span></span>|<span data-ttu-id="7b76d-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="7b76d-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="7b76d-170">Допустимые значения — от 1 до 99, наСледуемые от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7b76d-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7b76d-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7b76d-171">subjectNameFormat</span></span>|[<span data-ttu-id="7b76d-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="7b76d-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="7b76d-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7b76d-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="7b76d-174">НаСледуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="7b76d-175">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="7b76d-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7b76d-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="7b76d-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="7b76d-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="7b76d-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="7b76d-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="7b76d-179">НаСледуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="7b76d-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="7b76d-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="7b76d-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="7b76d-182">Int32</span><span class="sxs-lookup"><span data-stu-id="7b76d-182">Int32</span></span>|<span data-ttu-id="7b76d-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7b76d-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="7b76d-184">НаСледуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7b76d-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7b76d-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7b76d-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="7b76d-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="7b76d-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="7b76d-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="7b76d-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="7b76d-188">НаСледуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7b76d-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="7b76d-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="7b76d-190">Екстендедкэйусажес</span><span class="sxs-lookup"><span data-stu-id="7b76d-190">extendedKeyUsages</span></span>|<span data-ttu-id="7b76d-191">Коллекция [екстендедкэйусаже](../resources/intune-deviceconfig-extendedkeyusage.md)</span><span class="sxs-lookup"><span data-stu-id="7b76d-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="7b76d-192">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="7b76d-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="7b76d-193">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7b76d-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7b76d-194">НаСледуется от [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7b76d-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="7b76d-195">Сцепсерверурлс</span><span class="sxs-lookup"><span data-stu-id="7b76d-195">scepServerUrls</span></span>|<span data-ttu-id="7b76d-196">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7b76d-196">String collection</span></span>|<span data-ttu-id="7b76d-197">URL-адреса сервера SCEP</span><span class="sxs-lookup"><span data-stu-id="7b76d-197">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="7b76d-198">Свойства subjectnameformatstring</span><span class="sxs-lookup"><span data-stu-id="7b76d-198">subjectNameFormatString</span></span>|<span data-ttu-id="7b76d-199">String</span><span class="sxs-lookup"><span data-stu-id="7b76d-199">String</span></span>|<span data-ttu-id="7b76d-200">Настраиваемый формат для использования с SubjectNameFormat = Custom.</span><span class="sxs-lookup"><span data-stu-id="7b76d-200">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="7b76d-201">Пример: CN = {EmailAddress}}, E = {EmailAddress}}, OU = Enterprise Users, O = Contoso Corporation, L = Redmond, ST = Вашингтон, C = US</span><span class="sxs-lookup"><span data-stu-id="7b76d-201">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="7b76d-202">Кэйусаже</span><span class="sxs-lookup"><span data-stu-id="7b76d-202">keyUsage</span></span>|[<span data-ttu-id="7b76d-203">Кэйусажес</span><span class="sxs-lookup"><span data-stu-id="7b76d-203">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="7b76d-204">Использование ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7b76d-204">SCEP Key Usage.</span></span> <span data-ttu-id="7b76d-205">Возможные значения: `keyEncipherment`, `digitalSignature`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-205">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="7b76d-206">keySize</span><span class="sxs-lookup"><span data-stu-id="7b76d-206">keySize</span></span>|[<span data-ttu-id="7b76d-207">keySize</span><span class="sxs-lookup"><span data-stu-id="7b76d-207">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="7b76d-208">Размер ключа SCEP.</span><span class="sxs-lookup"><span data-stu-id="7b76d-208">SCEP Key Size.</span></span> <span data-ttu-id="7b76d-209">Возможные значения: `size1024`, `size2048`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-209">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="7b76d-210">Хашалгорисм</span><span class="sxs-lookup"><span data-stu-id="7b76d-210">hashAlgorithm</span></span>|[<span data-ttu-id="7b76d-211">Хашалгорисмс</span><span class="sxs-lookup"><span data-stu-id="7b76d-211">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="7b76d-212">Алгоритм хеширования SCEP.</span><span class="sxs-lookup"><span data-stu-id="7b76d-212">SCEP Hash Algorithm.</span></span> <span data-ttu-id="7b76d-213">Возможные значения: `sha1`, `sha2`.</span><span class="sxs-lookup"><span data-stu-id="7b76d-213">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="7b76d-214">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="7b76d-214">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="7b76d-215">String</span><span class="sxs-lookup"><span data-stu-id="7b76d-215">String</span></span>|<span data-ttu-id="7b76d-216">Настраиваемая строка, определяющая атрибут AAD.</span><span class="sxs-lookup"><span data-stu-id="7b76d-216">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="7b76d-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b76d-217">Response</span></span>
<span data-ttu-id="7b76d-218">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7b76d-218">If successful, this method returns a `200 OK` response code and an updated [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b76d-219">Пример</span><span class="sxs-lookup"><span data-stu-id="7b76d-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b76d-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b76d-220">Request</span></span>
<span data-ttu-id="7b76d-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b76d-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 974

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="7b76d-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b76d-222">Response</span></span>
<span data-ttu-id="7b76d-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7b76d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1146

{
  "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
  "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




