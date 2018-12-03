---
title: Обновление windowsPhone81ImportedPFXCertificateProfile
description: Обновление свойства объекта windowsPhone81ImportedPFXCertificateProfile.
ms.openlocfilehash: d30370482c2bd68e0394917e8d859b23588dc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078848"
---
# <a name="update-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="3d366-103">Обновление windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3d366-103">Update windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="3d366-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d366-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d366-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d366-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d366-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3d366-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d366-107">Обновление свойства объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3d366-107">Update the properties of a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d366-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d366-108">Prerequisites</span></span>
<span data-ttu-id="3d366-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d366-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d366-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d366-111">Permission type</span></span>|<span data-ttu-id="3d366-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d366-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d366-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d366-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d366-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d366-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d366-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d366-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d366-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d366-116">Not supported.</span></span>|
|<span data-ttu-id="3d366-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d366-117">Application</span></span>|<span data-ttu-id="3d366-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d366-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d366-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d366-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3d366-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d366-120">Request headers</span></span>
|<span data-ttu-id="3d366-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d366-121">Header</span></span>|<span data-ttu-id="3d366-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d366-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d366-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d366-123">Authorization</span></span>|<span data-ttu-id="3d366-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3d366-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d366-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d366-125">Accept</span></span>|<span data-ttu-id="3d366-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d366-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d366-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d366-127">Request body</span></span>
<span data-ttu-id="3d366-128">В тексте запроса укажите представление JSON для объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3d366-128">In the request body, supply a JSON representation for the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="3d366-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-129">The following table shows the properties that are required when you create the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="3d366-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d366-130">Property</span></span>|<span data-ttu-id="3d366-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d366-131">Type</span></span>|<span data-ttu-id="3d366-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d366-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d366-133">id</span><span class="sxs-lookup"><span data-stu-id="3d366-133">id</span></span>|<span data-ttu-id="3d366-134">String</span><span class="sxs-lookup"><span data-stu-id="3d366-134">String</span></span>|<span data-ttu-id="3d366-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3d366-135">Key of the entity.</span></span> <span data-ttu-id="3d366-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d366-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3d366-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d366-138">DateTimeOffset</span></span>|<span data-ttu-id="3d366-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3d366-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3d366-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3d366-141">roleScopeTagIds</span></span>|<span data-ttu-id="3d366-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d366-142">String collection</span></span>|<span data-ttu-id="3d366-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="3d366-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3d366-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3d366-145">supportsScopeTags</span></span>|<span data-ttu-id="3d366-146">Логический</span><span class="sxs-lookup"><span data-stu-id="3d366-146">Boolean</span></span>|<span data-ttu-id="3d366-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="3d366-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3d366-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="3d366-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3d366-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3d366-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3d366-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d366-150">This property is read-only.</span></span> <span data-ttu-id="3d366-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d366-152">createdDateTime</span></span>|<span data-ttu-id="3d366-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d366-153">DateTimeOffset</span></span>|<span data-ttu-id="3d366-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3d366-154">DateTime the object was created.</span></span> <span data-ttu-id="3d366-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-156">описание</span><span class="sxs-lookup"><span data-stu-id="3d366-156">description</span></span>|<span data-ttu-id="3d366-157">String</span><span class="sxs-lookup"><span data-stu-id="3d366-157">String</span></span>|<span data-ttu-id="3d366-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d366-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3d366-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3d366-160">displayName</span></span>|<span data-ttu-id="3d366-161">String</span><span class="sxs-lookup"><span data-stu-id="3d366-161">String</span></span>|<span data-ttu-id="3d366-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d366-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3d366-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-164">version</span><span class="sxs-lookup"><span data-stu-id="3d366-164">version</span></span>|<span data-ttu-id="3d366-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3d366-165">Int32</span></span>|<span data-ttu-id="3d366-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3d366-166">Version of the device configuration.</span></span> <span data-ttu-id="3d366-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3d366-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="3d366-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="3d366-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3d366-169">Int32</span></span>|<span data-ttu-id="3d366-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="3d366-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="3d366-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3d366-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3d366-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="3d366-172">keyStorageProvider</span></span>|[<span data-ttu-id="3d366-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3d366-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="3d366-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3d366-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="3d366-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="3d366-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3d366-176">subjectNameFormat</span></span>|[<span data-ttu-id="3d366-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3d366-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="3d366-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3d366-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="3d366-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="3d366-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3d366-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="3d366-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3d366-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3d366-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3d366-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3d366-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3d366-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="3d366-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="3d366-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3d366-185">Int32</span></span>|<span data-ttu-id="3d366-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3d366-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="3d366-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3d366-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="3d366-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="3d366-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="3d366-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3d366-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="3d366-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="3d366-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="3d366-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3d366-191">intendedPurpose</span></span>|[<span data-ttu-id="3d366-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="3d366-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="3d366-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="3d366-193">Not yet documented.</span></span> <span data-ttu-id="3d366-194">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="3d366-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="3d366-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d366-195">Response</span></span>
<span data-ttu-id="3d366-196">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3d366-196">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d366-197">Пример</span><span class="sxs-lookup"><span data-stu-id="3d366-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d366-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d366-198">Request</span></span>
<span data-ttu-id="3d366-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d366-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 573

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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="3d366-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d366-200">Response</span></span>
<span data-ttu-id="3d366-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3d366-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
  "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "intendedPurpose": "smimeEncryption"
}
```





