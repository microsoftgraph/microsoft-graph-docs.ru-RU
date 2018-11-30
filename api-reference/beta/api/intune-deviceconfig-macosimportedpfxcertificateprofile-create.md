---
title: Создание macOSImportedPFXCertificateProfile
description: Создание нового объекта macOSImportedPFXCertificateProfile.
ms.openlocfilehash: facd2a9189e66ac795302c176c578457e207074f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080902"
---
# <a name="create-macosimportedpfxcertificateprofile"></a><span data-ttu-id="731e0-103">Создание macOSImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="731e0-103">Create macOSImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="731e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="731e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="731e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="731e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="731e0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="731e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="731e0-107">Создание нового объекта [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="731e0-107">Create a new [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="731e0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="731e0-108">Prerequisites</span></span>
<span data-ttu-id="731e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="731e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="731e0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="731e0-111">Permission type</span></span>|<span data-ttu-id="731e0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="731e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="731e0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="731e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="731e0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="731e0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="731e0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="731e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="731e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="731e0-116">Not supported.</span></span>|
|<span data-ttu-id="731e0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="731e0-117">Application</span></span>|<span data-ttu-id="731e0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="731e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="731e0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="731e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="731e0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="731e0-120">Request headers</span></span>
|<span data-ttu-id="731e0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="731e0-121">Header</span></span>|<span data-ttu-id="731e0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="731e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="731e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="731e0-123">Authorization</span></span>|<span data-ttu-id="731e0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="731e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="731e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="731e0-125">Accept</span></span>|<span data-ttu-id="731e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="731e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="731e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="731e0-127">Request body</span></span>
<span data-ttu-id="731e0-128">В тексте запроса укажите представление JSON для объекта macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="731e0-128">In the request body, supply a JSON representation for the macOSImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="731e0-129">В следующей таблице показаны свойства, которые необходимы для создания macOSImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="731e0-129">The following table shows the properties that are required when you create the macOSImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="731e0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="731e0-130">Property</span></span>|<span data-ttu-id="731e0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="731e0-131">Type</span></span>|<span data-ttu-id="731e0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="731e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="731e0-133">id</span><span class="sxs-lookup"><span data-stu-id="731e0-133">id</span></span>|<span data-ttu-id="731e0-134">String</span><span class="sxs-lookup"><span data-stu-id="731e0-134">String</span></span>|<span data-ttu-id="731e0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="731e0-135">Key of the entity.</span></span> <span data-ttu-id="731e0-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="731e0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="731e0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731e0-138">DateTimeOffset</span></span>|<span data-ttu-id="731e0-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="731e0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="731e0-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="731e0-141">roleScopeTagIds</span></span>|<span data-ttu-id="731e0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="731e0-142">String collection</span></span>|<span data-ttu-id="731e0-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="731e0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="731e0-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="731e0-145">supportsScopeTags</span></span>|<span data-ttu-id="731e0-146">Логический</span><span class="sxs-lookup"><span data-stu-id="731e0-146">Boolean</span></span>|<span data-ttu-id="731e0-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="731e0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="731e0-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="731e0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="731e0-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="731e0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="731e0-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="731e0-150">This property is read-only.</span></span> <span data-ttu-id="731e0-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="731e0-152">createdDateTime</span></span>|<span data-ttu-id="731e0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="731e0-153">DateTimeOffset</span></span>|<span data-ttu-id="731e0-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="731e0-154">DateTime the object was created.</span></span> <span data-ttu-id="731e0-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-156">описание</span><span class="sxs-lookup"><span data-stu-id="731e0-156">description</span></span>|<span data-ttu-id="731e0-157">String</span><span class="sxs-lookup"><span data-stu-id="731e0-157">String</span></span>|<span data-ttu-id="731e0-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731e0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="731e0-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="731e0-160">displayName</span></span>|<span data-ttu-id="731e0-161">String</span><span class="sxs-lookup"><span data-stu-id="731e0-161">String</span></span>|<span data-ttu-id="731e0-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731e0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="731e0-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-164">version</span><span class="sxs-lookup"><span data-stu-id="731e0-164">version</span></span>|<span data-ttu-id="731e0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="731e0-165">Int32</span></span>|<span data-ttu-id="731e0-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="731e0-166">Version of the device configuration.</span></span> <span data-ttu-id="731e0-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="731e0-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="731e0-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="731e0-169">Int32</span><span class="sxs-lookup"><span data-stu-id="731e0-169">Int32</span></span>|<span data-ttu-id="731e0-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="731e0-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="731e0-171">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="731e0-171">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="731e0-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="731e0-172">subjectNameFormat</span></span>|[<span data-ttu-id="731e0-173">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="731e0-173">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="731e0-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="731e0-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="731e0-175">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-175">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="731e0-176">Возможные значения: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span><span class="sxs-lookup"><span data-stu-id="731e0-176">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="731e0-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="731e0-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="731e0-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="731e0-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="731e0-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="731e0-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="731e0-180">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-180">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="731e0-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="731e0-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="731e0-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="731e0-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="731e0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="731e0-183">Int32</span></span>|<span data-ttu-id="731e0-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="731e0-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="731e0-185">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="731e0-185">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="731e0-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="731e0-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="731e0-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="731e0-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="731e0-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="731e0-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="731e0-189">Наследуется от [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="731e0-189">Inherited from [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md).</span></span> <span data-ttu-id="731e0-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="731e0-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="731e0-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="731e0-191">intendedPurpose</span></span>|[<span data-ttu-id="731e0-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="731e0-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="731e0-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="731e0-193">Not yet documented.</span></span> <span data-ttu-id="731e0-194">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="731e0-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="731e0-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="731e0-195">Response</span></span>
<span data-ttu-id="731e0-196">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="731e0-196">If successful, this method returns a `201 Created` response code and a [macOSImportedPFXCertificateProfile](../resources/intune-deviceconfig-macosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="731e0-197">Пример</span><span class="sxs-lookup"><span data-stu-id="731e0-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="731e0-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="731e0-198">Request</span></span>
<span data-ttu-id="731e0-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="731e0-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.macOSImportedPFXCertificateProfile",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="731e0-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="731e0-200">Response</span></span>
<span data-ttu-id="731e0-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="731e0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





