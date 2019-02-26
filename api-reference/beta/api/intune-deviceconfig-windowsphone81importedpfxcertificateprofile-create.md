---
title: Создание windowsPhone81ImportedPFXCertificateProfile
description: Создание нового объекта windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1126114b04d6c10acd0f01f1d07efbe695e08ad7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144935"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="adb41-103">Создание windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="adb41-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="adb41-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adb41-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adb41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adb41-106">Создание нового объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="adb41-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adb41-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="adb41-107">Prerequisites</span></span>
<span data-ttu-id="adb41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="adb41-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adb41-110">Permission type</span></span>|<span data-ttu-id="adb41-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adb41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adb41-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adb41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="adb41-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb41-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adb41-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adb41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adb41-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb41-115">Not supported.</span></span>|
|<span data-ttu-id="adb41-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adb41-116">Application</span></span>|<span data-ttu-id="adb41-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adb41-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adb41-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adb41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="adb41-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adb41-119">Request headers</span></span>
|<span data-ttu-id="adb41-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adb41-120">Header</span></span>|<span data-ttu-id="adb41-121">Значение</span><span class="sxs-lookup"><span data-stu-id="adb41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adb41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="adb41-122">Authorization</span></span>|<span data-ttu-id="adb41-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="adb41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adb41-124">Accept</span><span class="sxs-lookup"><span data-stu-id="adb41-124">Accept</span></span>|<span data-ttu-id="adb41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="adb41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adb41-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adb41-126">Request body</span></span>
<span data-ttu-id="adb41-127">В тексте запроса добавьте представление объекта windowsPhone81ImportedPFXCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adb41-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="adb41-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="adb41-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="adb41-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="adb41-129">Property</span></span>|<span data-ttu-id="adb41-130">Тип</span><span class="sxs-lookup"><span data-stu-id="adb41-130">Type</span></span>|<span data-ttu-id="adb41-131">Описание</span><span class="sxs-lookup"><span data-stu-id="adb41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adb41-132">id</span><span class="sxs-lookup"><span data-stu-id="adb41-132">id</span></span>|<span data-ttu-id="adb41-133">String</span><span class="sxs-lookup"><span data-stu-id="adb41-133">String</span></span>|<span data-ttu-id="adb41-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="adb41-134">Key of the entity.</span></span> <span data-ttu-id="adb41-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adb41-136">lastModifiedDateTime</span></span>|<span data-ttu-id="adb41-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb41-137">DateTimeOffset</span></span>|<span data-ttu-id="adb41-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="adb41-138">DateTime the object was last modified.</span></span> <span data-ttu-id="adb41-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="adb41-140">roleScopeTagIds</span></span>|<span data-ttu-id="adb41-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="adb41-141">String collection</span></span>|<span data-ttu-id="adb41-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="adb41-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="adb41-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="adb41-144">supportsScopeTags</span></span>|<span data-ttu-id="adb41-145">Логический</span><span class="sxs-lookup"><span data-stu-id="adb41-145">Boolean</span></span>|<span data-ttu-id="adb41-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="adb41-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="adb41-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="adb41-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="adb41-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="adb41-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="adb41-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adb41-149">This property is read-only.</span></span> <span data-ttu-id="adb41-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adb41-151">createdDateTime</span></span>|<span data-ttu-id="adb41-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adb41-152">DateTimeOffset</span></span>|<span data-ttu-id="adb41-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="adb41-153">DateTime the object was created.</span></span> <span data-ttu-id="adb41-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-155">description</span><span class="sxs-lookup"><span data-stu-id="adb41-155">description</span></span>|<span data-ttu-id="adb41-156">String</span><span class="sxs-lookup"><span data-stu-id="adb41-156">String</span></span>|<span data-ttu-id="adb41-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="adb41-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="adb41-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-159">displayName</span><span class="sxs-lookup"><span data-stu-id="adb41-159">displayName</span></span>|<span data-ttu-id="adb41-160">String</span><span class="sxs-lookup"><span data-stu-id="adb41-160">String</span></span>|<span data-ttu-id="adb41-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="adb41-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="adb41-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-163">version</span><span class="sxs-lookup"><span data-stu-id="adb41-163">version</span></span>|<span data-ttu-id="adb41-164">Int32</span><span class="sxs-lookup"><span data-stu-id="adb41-164">Int32</span></span>|<span data-ttu-id="adb41-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="adb41-165">Version of the device configuration.</span></span> <span data-ttu-id="adb41-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adb41-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="adb41-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="adb41-168">Int32</span><span class="sxs-lookup"><span data-stu-id="adb41-168">Int32</span></span>|<span data-ttu-id="adb41-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="adb41-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="adb41-170">Допустимые значения — от 1 до 99, наСледуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="adb41-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="adb41-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="adb41-171">keyStorageProvider</span></span>|[<span data-ttu-id="adb41-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="adb41-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="adb41-173">Поставщик хранилища ключей (KSP), наСледуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="adb41-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="adb41-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="adb41-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="adb41-175">subjectNameFormat</span></span>|[<span data-ttu-id="adb41-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="adb41-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="adb41-177">Формат имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="adb41-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="adb41-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="adb41-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="adb41-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="adb41-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="adb41-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="adb41-181">Тип альтернативного имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="adb41-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="adb41-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="adb41-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="adb41-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="adb41-184">Int32</span><span class="sxs-lookup"><span data-stu-id="adb41-184">Int32</span></span>|<span data-ttu-id="adb41-185">Значение срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="adb41-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="adb41-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="adb41-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="adb41-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="adb41-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="adb41-188">Масштаб срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="adb41-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="adb41-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="adb41-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="adb41-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="adb41-190">intendedPurpose</span></span>|[<span data-ttu-id="adb41-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="adb41-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="adb41-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="adb41-192">Not yet documented.</span></span> <span data-ttu-id="adb41-193">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="adb41-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="adb41-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="adb41-194">Response</span></span>
<span data-ttu-id="adb41-195">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adb41-195">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb41-196">Пример</span><span class="sxs-lookup"><span data-stu-id="adb41-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="adb41-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="adb41-197">Request</span></span>
<span data-ttu-id="adb41-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adb41-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="adb41-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="adb41-199">Response</span></span>
<span data-ttu-id="adb41-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="adb41-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




