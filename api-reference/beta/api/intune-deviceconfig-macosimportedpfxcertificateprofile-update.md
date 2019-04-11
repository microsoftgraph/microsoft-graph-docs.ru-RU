---
title: Обновление Макосимпортедпфксцертификатепрофиле
description: Обновление свойств объекта Макосимпортедпфксцертификатепрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bdf83aa5fca824ed0180c630a69f80502cae559
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804825"
---
# <a name="update-macosimportedpfxcertificateprofile"></a><span data-ttu-id="c41ce-103">Обновление Макосимпортедпфксцертификатепрофиле</span><span class="sxs-lookup"><span data-stu-id="c41ce-103">Update macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="c41ce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c41ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c41ce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c41ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c41ce-106">Обновление свойств объекта [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c41ce-106">Update the properties of a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c41ce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c41ce-107">Prerequisites</span></span>
<span data-ttu-id="c41ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c41ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c41ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c41ce-110">Permission type</span></span>|<span data-ttu-id="c41ce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c41ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c41ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c41ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c41ce-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c41ce-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c41ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c41ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c41ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c41ce-115">Not supported.</span></span>|
|<span data-ttu-id="c41ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c41ce-116">Application</span></span>|<span data-ttu-id="c41ce-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c41ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c41ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c41ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c41ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c41ce-119">Request headers</span></span>
|<span data-ttu-id="c41ce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c41ce-120">Header</span></span>|<span data-ttu-id="c41ce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c41ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c41ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c41ce-122">Authorization</span></span>|<span data-ttu-id="c41ce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c41ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c41ce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c41ce-124">Accept</span></span>|<span data-ttu-id="c41ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c41ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c41ce-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c41ce-126">Request body</span></span>
<span data-ttu-id="c41ce-127">В тексте запроса добавьте представление объекта [Макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c41ce-127">In the request body, supply a JSON representation for the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="c41ce-128">В следующей таблице приведены свойства, необходимые при создании [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-128">The following table shows the properties that are required when you create the [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="c41ce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c41ce-129">Property</span></span>|<span data-ttu-id="c41ce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c41ce-130">Type</span></span>|<span data-ttu-id="c41ce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c41ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41ce-132">id</span><span class="sxs-lookup"><span data-stu-id="c41ce-132">id</span></span>|<span data-ttu-id="c41ce-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c41ce-133">String</span></span>|<span data-ttu-id="c41ce-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c41ce-134">Key of the entity.</span></span> <span data-ttu-id="c41ce-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c41ce-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c41ce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c41ce-137">DateTimeOffset</span></span>|<span data-ttu-id="c41ce-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c41ce-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c41ce-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c41ce-140">roleScopeTagIds</span></span>|<span data-ttu-id="c41ce-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c41ce-141">String collection</span></span>|<span data-ttu-id="c41ce-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c41ce-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c41ce-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c41ce-144">supportsScopeTags</span></span>|<span data-ttu-id="c41ce-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c41ce-145">Boolean</span></span>|<span data-ttu-id="c41ce-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c41ce-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c41ce-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c41ce-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c41ce-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c41ce-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c41ce-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c41ce-149">This property is read-only.</span></span> <span data-ttu-id="c41ce-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c41ce-151">createdDateTime</span></span>|<span data-ttu-id="c41ce-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c41ce-152">DateTimeOffset</span></span>|<span data-ttu-id="c41ce-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c41ce-153">DateTime the object was created.</span></span> <span data-ttu-id="c41ce-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-155">description</span><span class="sxs-lookup"><span data-stu-id="c41ce-155">description</span></span>|<span data-ttu-id="c41ce-156">String</span><span class="sxs-lookup"><span data-stu-id="c41ce-156">String</span></span>|<span data-ttu-id="c41ce-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c41ce-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c41ce-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c41ce-159">displayName</span></span>|<span data-ttu-id="c41ce-160">String</span><span class="sxs-lookup"><span data-stu-id="c41ce-160">String</span></span>|<span data-ttu-id="c41ce-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c41ce-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c41ce-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-163">version</span><span class="sxs-lookup"><span data-stu-id="c41ce-163">version</span></span>|<span data-ttu-id="c41ce-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c41ce-164">Int32</span></span>|<span data-ttu-id="c41ce-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c41ce-165">Version of the device configuration.</span></span> <span data-ttu-id="c41ce-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c41ce-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="c41ce-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="c41ce-168">Int32</span><span class="sxs-lookup"><span data-stu-id="c41ce-168">Int32</span></span>|<span data-ttu-id="c41ce-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="c41ce-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="c41ce-170">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c41ce-170">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c41ce-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="c41ce-171">subjectNameFormat</span></span>|[<span data-ttu-id="c41ce-172">Апплесубжектнамеформат</span><span class="sxs-lookup"><span data-stu-id="c41ce-172">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="c41ce-173">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c41ce-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="c41ce-174">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-174">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="c41ce-175">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="c41ce-175">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="c41ce-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c41ce-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="c41ce-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="c41ce-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="c41ce-178">Тип альтернативного имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="c41ce-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="c41ce-179">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-179">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="c41ce-180">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="c41ce-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="c41ce-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="c41ce-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="c41ce-182">Int32</span><span class="sxs-lookup"><span data-stu-id="c41ce-182">Int32</span></span>|<span data-ttu-id="c41ce-183">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c41ce-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="c41ce-184">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="c41ce-184">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="c41ce-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c41ce-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="c41ce-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="c41ce-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="c41ce-187">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="c41ce-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="c41ce-188">НаСледуется от [макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="c41ce-188">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="c41ce-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="c41ce-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="c41ce-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c41ce-190">intendedPurpose</span></span>|[<span data-ttu-id="c41ce-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="c41ce-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="c41ce-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c41ce-192">Not yet documented.</span></span> <span data-ttu-id="c41ce-193">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="c41ce-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="c41ce-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="c41ce-194">Response</span></span>
<span data-ttu-id="c41ce-195">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосимпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c41ce-195">If successful, this method returns a `200 OK` response code and an updated [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c41ce-196">Пример</span><span class="sxs-lookup"><span data-stu-id="c41ce-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="c41ce-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="c41ce-197">Request</span></span>
<span data-ttu-id="c41ce-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c41ce-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="c41ce-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="c41ce-199">Response</span></span>
<span data-ttu-id="c41ce-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c41ce-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





