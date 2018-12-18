---
title: Создание windowsPhone81ImportedPFXCertificateProfile
description: Создание нового объекта windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
ms.openlocfilehash: 925bfb3ded68140a41cce60c1907c3fe91725569
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350549"
---
# <a name="create-windowsphone81importedpfxcertificateprofile"></a><span data-ttu-id="6b599-103">Создание windowsPhone81ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6b599-103">Create windowsPhone81ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="6b599-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b599-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b599-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b599-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b599-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b599-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b599-107">Создание нового объекта [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6b599-107">Create a new [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b599-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b599-108">Prerequisites</span></span>
<span data-ttu-id="6b599-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b599-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b599-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b599-111">Permission type</span></span>|<span data-ttu-id="6b599-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b599-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b599-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b599-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b599-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b599-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b599-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b599-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b599-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b599-116">Not supported.</span></span>|
|<span data-ttu-id="6b599-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b599-117">Application</span></span>|<span data-ttu-id="6b599-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b599-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b599-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b599-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b599-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b599-120">Request headers</span></span>
|<span data-ttu-id="6b599-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b599-121">Header</span></span>|<span data-ttu-id="6b599-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6b599-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b599-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b599-123">Authorization</span></span>|<span data-ttu-id="6b599-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6b599-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b599-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b599-125">Accept</span></span>|<span data-ttu-id="6b599-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b599-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b599-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b599-127">Request body</span></span>
<span data-ttu-id="6b599-128">В тексте запроса укажите представление JSON для объекта windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6b599-128">In the request body, supply a JSON representation for the windowsPhone81ImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="6b599-129">В следующей таблице показаны свойства, которые необходимы для создания windowsPhone81ImportedPFXCertificateProfile.</span><span class="sxs-lookup"><span data-stu-id="6b599-129">The following table shows the properties that are required when you create the windowsPhone81ImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="6b599-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b599-130">Property</span></span>|<span data-ttu-id="6b599-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6b599-131">Type</span></span>|<span data-ttu-id="6b599-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6b599-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b599-133">id</span><span class="sxs-lookup"><span data-stu-id="6b599-133">id</span></span>|<span data-ttu-id="6b599-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6b599-134">String</span></span>|<span data-ttu-id="6b599-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6b599-135">Key of the entity.</span></span> <span data-ttu-id="6b599-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b599-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6b599-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b599-138">DateTimeOffset</span></span>|<span data-ttu-id="6b599-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6b599-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6b599-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b599-141">roleScopeTagIds</span></span>|<span data-ttu-id="6b599-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6b599-142">String collection</span></span>|<span data-ttu-id="6b599-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6b599-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b599-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b599-145">supportsScopeTags</span></span>|<span data-ttu-id="6b599-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="6b599-146">Boolean</span></span>|<span data-ttu-id="6b599-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="6b599-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b599-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="6b599-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b599-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6b599-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b599-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b599-150">This property is read-only.</span></span> <span data-ttu-id="6b599-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b599-152">createdDateTime</span></span>|<span data-ttu-id="6b599-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b599-153">DateTimeOffset</span></span>|<span data-ttu-id="6b599-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6b599-154">DateTime the object was created.</span></span> <span data-ttu-id="6b599-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-156">описание</span><span class="sxs-lookup"><span data-stu-id="6b599-156">description</span></span>|<span data-ttu-id="6b599-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6b599-157">String</span></span>|<span data-ttu-id="6b599-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b599-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b599-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6b599-160">displayName</span></span>|<span data-ttu-id="6b599-161">Строка</span><span class="sxs-lookup"><span data-stu-id="6b599-161">String</span></span>|<span data-ttu-id="6b599-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b599-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b599-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-164">version</span><span class="sxs-lookup"><span data-stu-id="6b599-164">version</span></span>|<span data-ttu-id="6b599-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6b599-165">Int32</span></span>|<span data-ttu-id="6b599-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6b599-166">Version of the device configuration.</span></span> <span data-ttu-id="6b599-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b599-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="6b599-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="6b599-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6b599-169">Int32</span></span>|<span data-ttu-id="6b599-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="6b599-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="6b599-171">Допустимые значения от 1 до 99 унаследованные от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6b599-171">Valid values 1 to 99 Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6b599-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="6b599-172">keyStorageProvider</span></span>|[<span data-ttu-id="6b599-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="6b599-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="6b599-174">Inherited поставщика хранилища ключ (KSP) из [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-174">Key Storage Provider (KSP) Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6b599-175">Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span><span class="sxs-lookup"><span data-stu-id="6b599-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="6b599-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6b599-176">subjectNameFormat</span></span>|[<span data-ttu-id="6b599-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="6b599-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="6b599-178">Сертификат субъекта имя формата наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-178">Certificate Subject Name Format Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6b599-179">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="6b599-179">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="6b599-180">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6b599-180">subjectAlternativeNameType</span></span>|[<span data-ttu-id="6b599-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="6b599-181">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="6b599-182">Сертификат Subject Alternative имя типа наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-182">Certificate Subject Alternative Name Type Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6b599-183">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="6b599-183">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="6b599-184">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="6b599-184">certificateValidityPeriodValue</span></span>|<span data-ttu-id="6b599-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6b599-185">Int32</span></span>|<span data-ttu-id="6b599-186">Значение для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6b599-186">Value for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)</span></span>|
|<span data-ttu-id="6b599-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6b599-187">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="6b599-188">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="6b599-188">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="6b599-189">Масштаб для сертификата действия периода наследуется от [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6b599-189">Scale for the Certificate Validity Period Inherited from [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md).</span></span> <span data-ttu-id="6b599-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="6b599-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="6b599-191">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6b599-191">intendedPurpose</span></span>|[<span data-ttu-id="6b599-192">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="6b599-192">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="6b599-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="6b599-193">Not yet documented.</span></span> <span data-ttu-id="6b599-194">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="6b599-194">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="6b599-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b599-195">Response</span></span>
<span data-ttu-id="6b599-196">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6b599-196">If successful, this method returns a `201 Created` response code and a [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b599-197">Пример</span><span class="sxs-lookup"><span data-stu-id="6b599-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b599-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b599-198">Request</span></span>
<span data-ttu-id="6b599-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b599-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 655

{
  "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
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

### <a name="response"></a><span data-ttu-id="6b599-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b599-200">Response</span></span>
<span data-ttu-id="6b599-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6b599-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





