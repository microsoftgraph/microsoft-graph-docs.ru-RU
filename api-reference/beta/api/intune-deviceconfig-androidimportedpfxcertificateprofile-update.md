---
title: Обновление androidImportedPFXCertificateProfile
description: Обновление свойства объекта androidImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7b7a70297a093c714fe6c28998bb8e708f34276a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863800"
---
# <a name="update-androidimportedpfxcertificateprofile"></a><span data-ttu-id="07869-103">Обновление androidImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="07869-103">Update androidImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="07869-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07869-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07869-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07869-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07869-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07869-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07869-107">Обновление свойства объекта [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="07869-107">Update the properties of a [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="07869-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07869-108">Prerequisites</span></span>
<span data-ttu-id="07869-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07869-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07869-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07869-111">Permission type</span></span>|<span data-ttu-id="07869-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07869-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07869-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07869-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07869-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07869-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07869-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07869-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07869-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07869-116">Not supported.</span></span>|
|<span data-ttu-id="07869-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07869-117">Application</span></span>|<span data-ttu-id="07869-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07869-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07869-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07869-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="07869-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07869-120">Request headers</span></span>
|<span data-ttu-id="07869-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07869-121">Header</span></span>|<span data-ttu-id="07869-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07869-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07869-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07869-123">Authorization</span></span>|<span data-ttu-id="07869-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="07869-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07869-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07869-125">Accept</span></span>|<span data-ttu-id="07869-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07869-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07869-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="07869-127">Request body</span></span>
<span data-ttu-id="07869-128">В тексте запроса укажите представление JSON для объекта [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="07869-128">In the request body, supply a JSON representation for the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object.</span></span>

<span data-ttu-id="07869-129">В следующей таблице показаны свойства, которые необходимы для создания [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="07869-129">The following table shows the properties that are required when you create the [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md).</span></span>

|<span data-ttu-id="07869-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07869-130">Property</span></span>|<span data-ttu-id="07869-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07869-131">Type</span></span>|<span data-ttu-id="07869-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07869-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07869-133">id</span><span class="sxs-lookup"><span data-stu-id="07869-133">id</span></span>|<span data-ttu-id="07869-134">Строка</span><span class="sxs-lookup"><span data-stu-id="07869-134">String</span></span>|<span data-ttu-id="07869-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07869-135">Key of the entity.</span></span> <span data-ttu-id="07869-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07869-137">lastModifiedDateTime</span></span>|<span data-ttu-id="07869-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07869-138">DateTimeOffset</span></span>|<span data-ttu-id="07869-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="07869-139">DateTime the object was last modified.</span></span> <span data-ttu-id="07869-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07869-141">roleScopeTagIds</span></span>|<span data-ttu-id="07869-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="07869-142">String collection</span></span>|<span data-ttu-id="07869-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="07869-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="07869-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="07869-145">supportsScopeTags</span></span>|<span data-ttu-id="07869-146">Логический</span><span class="sxs-lookup"><span data-stu-id="07869-146">Boolean</span></span>|<span data-ttu-id="07869-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="07869-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="07869-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="07869-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="07869-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="07869-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="07869-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="07869-150">This property is read-only.</span></span> <span data-ttu-id="07869-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07869-152">createdDateTime</span></span>|<span data-ttu-id="07869-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07869-153">DateTimeOffset</span></span>|<span data-ttu-id="07869-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="07869-154">DateTime the object was created.</span></span> <span data-ttu-id="07869-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-156">описание</span><span class="sxs-lookup"><span data-stu-id="07869-156">description</span></span>|<span data-ttu-id="07869-157">Строка</span><span class="sxs-lookup"><span data-stu-id="07869-157">String</span></span>|<span data-ttu-id="07869-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07869-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="07869-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-160">displayName</span><span class="sxs-lookup"><span data-stu-id="07869-160">displayName</span></span>|<span data-ttu-id="07869-161">Строка</span><span class="sxs-lookup"><span data-stu-id="07869-161">String</span></span>|<span data-ttu-id="07869-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07869-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="07869-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-164">version</span><span class="sxs-lookup"><span data-stu-id="07869-164">version</span></span>|<span data-ttu-id="07869-165">Int32</span><span class="sxs-lookup"><span data-stu-id="07869-165">Int32</span></span>|<span data-ttu-id="07869-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07869-166">Version of the device configuration.</span></span> <span data-ttu-id="07869-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07869-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07869-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="07869-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="07869-169">Int32</span><span class="sxs-lookup"><span data-stu-id="07869-169">Int32</span></span>|<span data-ttu-id="07869-170">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="07869-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="07869-171">Допустимые значения от 1 до 99 унаследованные от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07869-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="07869-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="07869-172">subjectNameFormat</span></span>|[<span data-ttu-id="07869-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="07869-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="07869-174">Формат имени субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="07869-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="07869-175">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07869-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="07869-176">Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span><span class="sxs-lookup"><span data-stu-id="07869-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="07869-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="07869-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="07869-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="07869-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="07869-179">Тип альтернативное имя субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="07869-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="07869-180">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07869-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="07869-181">Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="07869-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="07869-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="07869-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="07869-183">Int32</span><span class="sxs-lookup"><span data-stu-id="07869-183">Int32</span></span>|<span data-ttu-id="07869-184">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="07869-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="07869-185">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07869-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="07869-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="07869-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="07869-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="07869-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="07869-188">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="07869-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="07869-189">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="07869-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="07869-190">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="07869-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="07869-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="07869-191">extendedKeyUsages</span></span>|<span data-ttu-id="07869-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="07869-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="07869-193">Параметры расширенного использования ключа (EKU).</span><span class="sxs-lookup"><span data-stu-id="07869-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="07869-194">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="07869-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="07869-195">Наследуется от [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="07869-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="07869-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="07869-196">intendedPurpose</span></span>|[<span data-ttu-id="07869-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="07869-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="07869-198">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="07869-198">Not yet documented.</span></span> <span data-ttu-id="07869-199">Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span><span class="sxs-lookup"><span data-stu-id="07869-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="07869-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="07869-200">Response</span></span>
<span data-ttu-id="07869-201">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07869-201">If successful, this method returns a `200 OK` response code and an updated [androidImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07869-202">Пример</span><span class="sxs-lookup"><span data-stu-id="07869-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="07869-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="07869-203">Request</span></span>
<span data-ttu-id="07869-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07869-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 708

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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="07869-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="07869-205">Response</span></span>
<span data-ttu-id="07869-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07869-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 891

{
  "@odata.type": "#microsoft.graph.androidImportedPFXCertificateProfile",
  "id": "1cd3b0a6-b0a6-1cd3-a6b0-d31ca6b0d31c",
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
  "intendedPurpose": "smimeEncryption"
}
```





