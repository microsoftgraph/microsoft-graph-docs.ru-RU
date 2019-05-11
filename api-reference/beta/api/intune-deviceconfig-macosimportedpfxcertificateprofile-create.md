---
title: Создание Макосимпортедпфксцертификатепрофиле
description: Создание нового объекта Макосимпортедпфксцертификатепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1084100716aaabb4eb44f424e429cfaf334f2992
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922447"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="a70d0-103">Создание Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="a70d0-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="a70d0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a70d0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a70d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70d0-106">Создание нового объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a70d0-106">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a70d0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a70d0-107">Prerequisites</span></span>
<span data-ttu-id="a70d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a70d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a70d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a70d0-110">Permission type</span></span>|<span data-ttu-id="a70d0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a70d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a70d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a70d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a70d0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a70d0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a70d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a70d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a70d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70d0-115">Not supported.</span></span>|
|<span data-ttu-id="a70d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a70d0-116">Application</span></span>|<span data-ttu-id="a70d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a70d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a70d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a70d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a70d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a70d0-119">Request headers</span></span>
|<span data-ttu-id="a70d0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a70d0-120">Header</span></span>|<span data-ttu-id="a70d0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a70d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a70d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a70d0-122">Authorization</span></span>|<span data-ttu-id="a70d0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a70d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a70d0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a70d0-124">Accept</span></span>|<span data-ttu-id="a70d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a70d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a70d0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a70d0-126">Request body</span></span>
<span data-ttu-id="a70d0-127">В тексте запроса добавьте представление объекта Макосимпортедпфксцертификатепрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a70d0-127">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="a70d0-128">В следующей таблице приведены свойства, необходимые при создании Макосимпортедпфксцертификатепрофиле.</span><span class="sxs-lookup"><span data-stu-id="a70d0-128">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="a70d0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a70d0-129">Property</span></span>|<span data-ttu-id="a70d0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a70d0-130">Type</span></span>|<span data-ttu-id="a70d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a70d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70d0-132">id</span><span class="sxs-lookup"><span data-stu-id="a70d0-132">id</span></span>|<span data-ttu-id="a70d0-133">String</span><span class="sxs-lookup"><span data-stu-id="a70d0-133">String</span></span>|<span data-ttu-id="a70d0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a70d0-134">Key of the entity.</span></span> <span data-ttu-id="a70d0-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a70d0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a70d0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70d0-137">DateTimeOffset</span></span>|<span data-ttu-id="a70d0-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a70d0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a70d0-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a70d0-140">roleScopeTagIds</span></span>|<span data-ttu-id="a70d0-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a70d0-141">String collection</span></span>|<span data-ttu-id="a70d0-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a70d0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a70d0-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a70d0-144">supportsScopeTags</span></span>|<span data-ttu-id="a70d0-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a70d0-145">Boolean</span></span>|<span data-ttu-id="a70d0-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a70d0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a70d0-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a70d0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a70d0-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a70d0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a70d0-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a70d0-149">This property is read-only.</span></span> <span data-ttu-id="a70d0-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a70d0-151">createdDateTime</span></span>|<span data-ttu-id="a70d0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70d0-152">DateTimeOffset</span></span>|<span data-ttu-id="a70d0-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a70d0-153">DateTime the object was created.</span></span> <span data-ttu-id="a70d0-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-155">description</span><span class="sxs-lookup"><span data-stu-id="a70d0-155">description</span></span>|<span data-ttu-id="a70d0-156">String</span><span class="sxs-lookup"><span data-stu-id="a70d0-156">String</span></span>|<span data-ttu-id="a70d0-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70d0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a70d0-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a70d0-159">displayName</span></span>|<span data-ttu-id="a70d0-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a70d0-160">String</span></span>|<span data-ttu-id="a70d0-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70d0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a70d0-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-163">version</span><span class="sxs-lookup"><span data-stu-id="a70d0-163">version</span></span>|<span data-ttu-id="a70d0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a70d0-164">Int32</span></span>|<span data-ttu-id="a70d0-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a70d0-165">Version of the device configuration.</span></span> <span data-ttu-id="a70d0-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a70d0-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="a70d0-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="a70d0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a70d0-168">Int32</span></span>|<span data-ttu-id="a70d0-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="a70d0-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="a70d0-170">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a70d0-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a70d0-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="a70d0-171">subjectNameFormat</span></span>|[<span data-ttu-id="a70d0-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="a70d0-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="a70d0-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="a70d0-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="a70d0-174">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a70d0-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="a70d0-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="a70d0-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a70d0-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="a70d0-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a70d0-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a70d0-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="a70d0-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="a70d0-179">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a70d0-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a70d0-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a70d0-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="a70d0-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="a70d0-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a70d0-182">Int32</span></span>|<span data-ttu-id="a70d0-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="a70d0-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="a70d0-184">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a70d0-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="a70d0-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a70d0-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="a70d0-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="a70d0-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="a70d0-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="a70d0-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="a70d0-188">Наследуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a70d0-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="a70d0-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="a70d0-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="a70d0-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a70d0-190">intendedPurpose</span></span>|[<span data-ttu-id="a70d0-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="a70d0-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="a70d0-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a70d0-192">Not yet documented.</span></span> <span data-ttu-id="a70d0-193">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="a70d0-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="a70d0-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a70d0-194">Response</span></span>
<span data-ttu-id="a70d0-195">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a70d0-195">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a70d0-196">Пример</span><span class="sxs-lookup"><span data-stu-id="a70d0-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="a70d0-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="a70d0-197">Request</span></span>
<span data-ttu-id="a70d0-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a70d0-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="a70d0-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="a70d0-199">Response</span></span>
<span data-ttu-id="a70d0-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a70d0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 696

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "id": "4175bd8c-bd8c-4175-8cbd-75418cbd7541",
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
  "intendedPurpose": "smimeEncryption"
}
```




