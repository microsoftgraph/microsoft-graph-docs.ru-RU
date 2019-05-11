---
title: Обновление windows10ImportedPFXCertificateProfile
description: Обновление свойств объекта windows10ImportedPFXCertificateProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 271076658b8feb56ef9e0f168f1dfe18fe5533de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918649"
---
# <a name="update-windows10importedpfxcertificateprofile"></a><span data-ttu-id="03b4d-103">Обновление windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="03b4d-103">Update windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="03b4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03b4d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03b4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03b4d-106">Обновление свойств объекта [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03b4d-106">Update the properties of a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03b4d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03b4d-107">Prerequisites</span></span>
<span data-ttu-id="03b4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03b4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b4d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03b4d-110">Permission type</span></span>|<span data-ttu-id="03b4d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03b4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03b4d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03b4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03b4d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b4d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03b4d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03b4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03b4d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b4d-115">Not supported.</span></span>|
|<span data-ttu-id="03b4d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03b4d-116">Application</span></span>|<span data-ttu-id="03b4d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03b4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03b4d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03b4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03b4d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03b4d-119">Request headers</span></span>
|<span data-ttu-id="03b4d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03b4d-120">Header</span></span>|<span data-ttu-id="03b4d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="03b4d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03b4d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03b4d-122">Authorization</span></span>|<span data-ttu-id="03b4d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03b4d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03b4d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="03b4d-124">Accept</span></span>|<span data-ttu-id="03b4d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03b4d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b4d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03b4d-126">Request body</span></span>
<span data-ttu-id="03b4d-127">В тексте запроса добавьте представление объекта [Windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03b4d-127">In the request body, supply a JSON representation for the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="03b4d-128">В следующей таблице приведены свойства, необходимые при создании [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-128">The following table shows the properties that are required when you create the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="03b4d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="03b4d-129">Property</span></span>|<span data-ttu-id="03b4d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="03b4d-130">Type</span></span>|<span data-ttu-id="03b4d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="03b4d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03b4d-132">id</span><span class="sxs-lookup"><span data-stu-id="03b4d-132">id</span></span>|<span data-ttu-id="03b4d-133">String</span><span class="sxs-lookup"><span data-stu-id="03b4d-133">String</span></span>|<span data-ttu-id="03b4d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03b4d-134">Key of the entity.</span></span> <span data-ttu-id="03b4d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03b4d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="03b4d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03b4d-137">DateTimeOffset</span></span>|<span data-ttu-id="03b4d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="03b4d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="03b4d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03b4d-140">roleScopeTagIds</span></span>|<span data-ttu-id="03b4d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="03b4d-141">String collection</span></span>|<span data-ttu-id="03b4d-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="03b4d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03b4d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="03b4d-144">supportsScopeTags</span></span>|<span data-ttu-id="03b4d-145">Логический</span><span class="sxs-lookup"><span data-stu-id="03b4d-145">Boolean</span></span>|<span data-ttu-id="03b4d-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="03b4d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03b4d-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="03b4d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03b4d-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="03b4d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03b4d-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03b4d-149">This property is read-only.</span></span> <span data-ttu-id="03b4d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03b4d-151">createdDateTime</span></span>|<span data-ttu-id="03b4d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03b4d-152">DateTimeOffset</span></span>|<span data-ttu-id="03b4d-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="03b4d-153">DateTime the object was created.</span></span> <span data-ttu-id="03b4d-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-155">description</span><span class="sxs-lookup"><span data-stu-id="03b4d-155">description</span></span>|<span data-ttu-id="03b4d-156">String</span><span class="sxs-lookup"><span data-stu-id="03b4d-156">String</span></span>|<span data-ttu-id="03b4d-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03b4d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03b4d-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="03b4d-159">displayName</span></span>|<span data-ttu-id="03b4d-160">Строка</span><span class="sxs-lookup"><span data-stu-id="03b4d-160">String</span></span>|<span data-ttu-id="03b4d-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03b4d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03b4d-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-163">version</span><span class="sxs-lookup"><span data-stu-id="03b4d-163">version</span></span>|<span data-ttu-id="03b4d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="03b4d-164">Int32</span></span>|<span data-ttu-id="03b4d-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03b4d-165">Version of the device configuration.</span></span> <span data-ttu-id="03b4d-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03b4d-167">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="03b4d-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="03b4d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="03b4d-168">Int32</span></span>|<span data-ttu-id="03b4d-169">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="03b4d-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="03b4d-170">Допустимые значения — от 1 до 99, наследуемые от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03b4d-170">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03b4d-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="03b4d-171">keyStorageProvider</span></span>|[<span data-ttu-id="03b4d-172">Кэйсторажепровидероптион</span><span class="sxs-lookup"><span data-stu-id="03b4d-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="03b4d-173">Поставщик хранилища ключей (KSP), наследуемый от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-173">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="03b4d-174">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="03b4d-174">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="03b4d-175">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03b4d-175">subjectNameFormat</span></span>|[<span data-ttu-id="03b4d-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="03b4d-176">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="03b4d-177">Формат имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-177">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="03b4d-178">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="03b4d-178">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="03b4d-179">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03b4d-179">subjectAlternativeNameType</span></span>|[<span data-ttu-id="03b4d-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="03b4d-180">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="03b4d-181">Тип альтернативного имени субъекта сертификата наследуется от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-181">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="03b4d-182">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="03b4d-182">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="03b4d-183">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="03b4d-183">certificateValidityPeriodValue</span></span>|<span data-ttu-id="03b4d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="03b4d-184">Int32</span></span>|<span data-ttu-id="03b4d-185">Значение срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03b4d-185">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="03b4d-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03b4d-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="03b4d-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="03b4d-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="03b4d-188">Масштаб срока действия сертификата, наследуемого от [windowscertificateprofilebase)](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03b4d-188">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="03b4d-189">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="03b4d-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="03b4d-190">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="03b4d-190">intendedPurpose</span></span>|[<span data-ttu-id="03b4d-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="03b4d-191">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="03b4d-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="03b4d-192">Not yet documented.</span></span> <span data-ttu-id="03b4d-193">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="03b4d-193">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="03b4d-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b4d-194">Response</span></span>
<span data-ttu-id="03b4d-195">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03b4d-195">If successful, this method returns a `200 OK` response code and an updated [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b4d-196">Пример</span><span class="sxs-lookup"><span data-stu-id="03b4d-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="03b4d-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="03b4d-197">Request</span></span>
<span data-ttu-id="03b4d-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03b4d-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 586

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="03b4d-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="03b4d-199">Response</span></span>
<span data-ttu-id="03b4d-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03b4d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 758

{
  "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
  "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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




