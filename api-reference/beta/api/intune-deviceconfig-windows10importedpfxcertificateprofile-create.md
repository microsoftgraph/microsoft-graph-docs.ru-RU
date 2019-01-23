---
title: Создание windows10ImportedPFXCertificateProfile
description: Создание нового объекта windows10ImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 666a849b1713c7009af7473438ed546e7639165d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408133"
---
# <a name="create-windows10importedpfxcertificateprofile"></a><span data-ttu-id="5e065-103">Создание windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="5e065-103">Create windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="5e065-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e065-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5e065-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e065-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e065-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e065-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e065-107">Создание нового объекта [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5e065-107">Create a new [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e065-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5e065-108">Prerequisites</span></span>
<span data-ttu-id="5e065-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5e065-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e065-111">Permission type</span></span>|<span data-ttu-id="5e065-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e065-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e065-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e065-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e065-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e065-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e065-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e065-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e065-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e065-116">Not supported.</span></span>|
|<span data-ttu-id="5e065-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e065-117">Application</span></span>|<span data-ttu-id="5e065-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e065-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e065-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e065-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5e065-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e065-120">Request headers</span></span>
|<span data-ttu-id="5e065-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e065-121">Header</span></span>|<span data-ttu-id="5e065-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e065-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e065-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e065-123">Authorization</span></span>|<span data-ttu-id="5e065-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e065-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e065-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e065-125">Accept</span></span>|<span data-ttu-id="5e065-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e065-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e065-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e065-127">Request body</span></span>
<span data-ttu-id="5e065-128">В тексте запроса укажите представление JSON для объекта windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5e065-128">In the request body, supply a JSON representation for the windows10ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="5e065-129">В следующей таблице показаны свойства, которые необходимы для создания windows10ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="5e065-129">The following table shows the properties that are required when you create the windows10ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="5e065-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e065-130">Property</span></span>|<span data-ttu-id="5e065-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e065-131">Type</span></span>|<span data-ttu-id="5e065-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e065-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e065-133">id</span><span class="sxs-lookup"><span data-stu-id="5e065-133">id</span></span>|<span data-ttu-id="5e065-134">String</span><span class="sxs-lookup"><span data-stu-id="5e065-134">String</span></span>|<span data-ttu-id="5e065-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e065-135">Key of the entity.</span></span> <span data-ttu-id="5e065-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e065-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5e065-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e065-138">DateTimeOffset</span></span>|<span data-ttu-id="5e065-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5e065-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5e065-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e065-141">roleScopeTagIds</span></span>|<span data-ttu-id="5e065-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e065-142">String collection</span></span>|<span data-ttu-id="5e065-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5e065-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5e065-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5e065-145">supportsScopeTags</span></span>|<span data-ttu-id="5e065-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5e065-146">Boolean</span></span>|<span data-ttu-id="5e065-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5e065-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5e065-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5e065-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5e065-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5e065-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5e065-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e065-150">This property is read-only.</span></span> <span data-ttu-id="5e065-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e065-152">createdDateTime</span></span>|<span data-ttu-id="5e065-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e065-153">DateTimeOffset</span></span>|<span data-ttu-id="5e065-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5e065-154">DateTime the object was created.</span></span> <span data-ttu-id="5e065-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-156">description</span><span class="sxs-lookup"><span data-stu-id="5e065-156">description</span></span>|<span data-ttu-id="5e065-157">String</span><span class="sxs-lookup"><span data-stu-id="5e065-157">String</span></span>|<span data-ttu-id="5e065-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e065-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5e065-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5e065-160">displayName</span></span>|<span data-ttu-id="5e065-161">String</span><span class="sxs-lookup"><span data-stu-id="5e065-161">String</span></span>|<span data-ttu-id="5e065-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e065-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5e065-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-164">version</span><span class="sxs-lookup"><span data-stu-id="5e065-164">version</span></span>|<span data-ttu-id="5e065-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5e065-165">Int32</span></span>|<span data-ttu-id="5e065-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5e065-166">Version of the device configuration.</span></span> <span data-ttu-id="5e065-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e065-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5e065-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="5e065-169">Int32</span><span class="sxs-lookup"><span data-stu-id="5e065-169">Int32</span></span>|<span data-ttu-id="5e065-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="5e065-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5e065-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5e065-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5e065-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="5e065-172">keyStorageProvider</span></span>|[<span data-ttu-id="5e065-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="5e065-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="5e065-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5e065-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="5e065-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="5e065-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5e065-176">subjectNameFormat</span></span>|[<span data-ttu-id="5e065-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="5e065-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="5e065-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5e065-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="5e065-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="5e065-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5e065-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="5e065-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="5e065-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="5e065-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5e065-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="5e065-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="5e065-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5e065-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5e065-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5e065-185">Int32</span></span>|<span data-ttu-id="5e065-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5e065-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="5e065-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5e065-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5e065-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5e065-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5e065-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="5e065-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="5e065-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5e065-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="5e065-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="5e065-191">intendedPurpose</span></span>|[<span data-ttu-id="5e065-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="5e065-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="5e065-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5e065-193">Not yet documented.</span></span> <span data-ttu-id="5e065-194">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="5e065-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="5e065-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e065-195">Response</span></span>
<span data-ttu-id="5e065-196">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5e065-196">If successful, this method returns a `201 Created` response code and a [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e065-197">Пример</span><span class="sxs-lookup"><span data-stu-id="5e065-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e065-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e065-198">Request</span></span>
<span data-ttu-id="5e065-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e065-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="5e065-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e065-200">Response</span></span>
<span data-ttu-id="5e065-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e065-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




