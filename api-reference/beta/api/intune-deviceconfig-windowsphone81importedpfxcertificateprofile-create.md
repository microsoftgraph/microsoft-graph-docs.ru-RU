---
title: Создание windowsPhone81ImportedPFXCertificateProfile
description: Создание нового объекта windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75e083e531b5647146b09f49d0bcafe8a5802817
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966049"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="ccd47-103">Создание windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ccd47-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="ccd47-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccd47-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ccd47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd47-106">Создание нового объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd47-106">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccd47-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ccd47-107">Prerequisites</span></span>
<span data-ttu-id="ccd47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd47-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd47-110">Permission type</span></span>|<span data-ttu-id="ccd47-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd47-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd47-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd47-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd47-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd47-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd47-115">Not supported.</span></span>|
|<span data-ttu-id="ccd47-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd47-116">Application</span></span>|<span data-ttu-id="ccd47-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd47-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ccd47-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccd47-119">Request headers</span></span>
|<span data-ttu-id="ccd47-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ccd47-120">Header</span></span>|<span data-ttu-id="ccd47-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ccd47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccd47-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ccd47-122">Authorization</span></span>|<span data-ttu-id="ccd47-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccd47-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ccd47-124">Accept</span></span>|<span data-ttu-id="ccd47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ccd47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd47-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccd47-126">Request body</span></span>
<span data-ttu-id="ccd47-127">В тексте запроса добавьте представление объекта windowsPhone81ImportedPFXCertificateProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ccd47-127">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="ccd47-128">В следующей таблице приведены свойства, необходимые при создании windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="ccd47-128">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="ccd47-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ccd47-129">Property</span></span>|<span data-ttu-id="ccd47-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd47-130">Type</span></span>|<span data-ttu-id="ccd47-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd47-132">id</span><span class="sxs-lookup"><span data-stu-id="ccd47-132">id</span></span>|<span data-ttu-id="ccd47-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ccd47-133">String</span></span>|<span data-ttu-id="ccd47-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ccd47-134">Key of the entity.</span></span> <span data-ttu-id="ccd47-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd47-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ccd47-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd47-137">DateTimeOffset</span></span>|<span data-ttu-id="ccd47-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ccd47-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ccd47-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ccd47-140">roleScopeTagIds</span></span>|<span data-ttu-id="ccd47-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ccd47-141">String collection</span></span>|<span data-ttu-id="ccd47-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ccd47-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ccd47-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ccd47-144">supportsScopeTags</span></span>|<span data-ttu-id="ccd47-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccd47-145">Boolean</span></span>|<span data-ttu-id="ccd47-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ccd47-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ccd47-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ccd47-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ccd47-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ccd47-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ccd47-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ccd47-149">This property is read-only.</span></span> <span data-ttu-id="ccd47-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccd47-151">createdDateTime</span></span>|<span data-ttu-id="ccd47-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccd47-152">DateTimeOffset</span></span>|<span data-ttu-id="ccd47-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ccd47-153">DateTime the object was created.</span></span> <span data-ttu-id="ccd47-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-155">description</span><span class="sxs-lookup"><span data-stu-id="ccd47-155">description</span></span>|<span data-ttu-id="ccd47-156">String</span><span class="sxs-lookup"><span data-stu-id="ccd47-156">String</span></span>|<span data-ttu-id="ccd47-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccd47-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ccd47-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ccd47-159">displayName</span></span>|<span data-ttu-id="ccd47-160">String</span><span class="sxs-lookup"><span data-stu-id="ccd47-160">String</span></span>|<span data-ttu-id="ccd47-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccd47-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ccd47-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-163">version</span><span class="sxs-lookup"><span data-stu-id="ccd47-163">version</span></span>|<span data-ttu-id="ccd47-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd47-164">Int32</span></span>|<span data-ttu-id="ccd47-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ccd47-165">Version of the device configuration.</span></span> <span data-ttu-id="ccd47-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ccd47-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="ccd47-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="ccd47-168">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd47-168">Int32</span></span>|<span data-ttu-id="ccd47-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="ccd47-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="ccd47-170">Допустимые значения — от 1 до 99, наСледуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ccd47-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ccd47-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="ccd47-171">keyStorageProvider</span></span>|[<span data-ttu-id="ccd47-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="ccd47-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="ccd47-173">Поставщик хранилища ключей (KSP), наСледуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ccd47-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="ccd47-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="ccd47-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ccd47-175">subjectNameFormat</span></span>|[<span data-ttu-id="ccd47-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="ccd47-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="ccd47-177">Формат имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ccd47-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="ccd47-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="ccd47-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ccd47-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="ccd47-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ccd47-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ccd47-181">Тип альтернативного имени субъекта сертификата наСледуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ccd47-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="ccd47-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ccd47-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="ccd47-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="ccd47-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ccd47-184">Int32</span></span>|<span data-ttu-id="ccd47-185">Значение срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ccd47-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="ccd47-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ccd47-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="ccd47-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="ccd47-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="ccd47-188">Масштаб срока действия сертификата, наСледуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ccd47-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="ccd47-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="ccd47-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="ccd47-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ccd47-190">intendedPurpose</span></span>|[<span data-ttu-id="ccd47-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="ccd47-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="ccd47-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ccd47-192">Not yet documented.</span></span> <span data-ttu-id="ccd47-193">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="ccd47-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="ccd47-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd47-194">Response</span></span>
<span data-ttu-id="ccd47-195">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ccd47-195">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccd47-196">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd47-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccd47-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd47-197">Request</span></span>
<span data-ttu-id="ccd47-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ccd47-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ccd47-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd47-199">Response</span></span>
<span data-ttu-id="ccd47-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccd47-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




