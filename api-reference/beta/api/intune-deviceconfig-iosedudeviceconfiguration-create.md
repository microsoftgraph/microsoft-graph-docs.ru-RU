---
title: Создание Иоседудевицеконфигуратион
description: Создание нового объекта Иоседудевицеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9e3a85c2ceb1a37b36a26e3a4ee93c05c855b8b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923590"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="02ad1-103">Создание Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="02ad1-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="02ad1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ad1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02ad1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02ad1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02ad1-106">Создание нового объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="02ad1-106">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02ad1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="02ad1-107">Prerequisites</span></span>
<span data-ttu-id="02ad1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ad1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02ad1-110">Permission type</span></span>|<span data-ttu-id="02ad1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02ad1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02ad1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02ad1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02ad1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ad1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02ad1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02ad1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02ad1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ad1-115">Not supported.</span></span>|
|<span data-ttu-id="02ad1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02ad1-116">Application</span></span>|<span data-ttu-id="02ad1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ad1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02ad1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02ad1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02ad1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02ad1-119">Request headers</span></span>
|<span data-ttu-id="02ad1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02ad1-120">Header</span></span>|<span data-ttu-id="02ad1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="02ad1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02ad1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02ad1-122">Authorization</span></span>|<span data-ttu-id="02ad1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02ad1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02ad1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="02ad1-124">Accept</span></span>|<span data-ttu-id="02ad1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02ad1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02ad1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02ad1-126">Request body</span></span>
<span data-ttu-id="02ad1-127">В тексте запроса добавьте представление объекта Иоседудевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02ad1-127">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="02ad1-128">В следующей таблице приведены свойства, необходимые при создании Иоседудевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="02ad1-128">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="02ad1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="02ad1-129">Property</span></span>|<span data-ttu-id="02ad1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="02ad1-130">Type</span></span>|<span data-ttu-id="02ad1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="02ad1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02ad1-132">id</span><span class="sxs-lookup"><span data-stu-id="02ad1-132">id</span></span>|<span data-ttu-id="02ad1-133">String</span><span class="sxs-lookup"><span data-stu-id="02ad1-133">String</span></span>|<span data-ttu-id="02ad1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="02ad1-134">Key of the entity.</span></span> <span data-ttu-id="02ad1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02ad1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="02ad1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02ad1-137">DateTimeOffset</span></span>|<span data-ttu-id="02ad1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="02ad1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="02ad1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02ad1-140">roleScopeTagIds</span></span>|<span data-ttu-id="02ad1-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02ad1-141">String collection</span></span>|<span data-ttu-id="02ad1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="02ad1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="02ad1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="02ad1-144">supportsScopeTags</span></span>|<span data-ttu-id="02ad1-145">Логический</span><span class="sxs-lookup"><span data-stu-id="02ad1-145">Boolean</span></span>|<span data-ttu-id="02ad1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="02ad1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="02ad1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="02ad1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="02ad1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="02ad1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="02ad1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02ad1-149">This property is read-only.</span></span> <span data-ttu-id="02ad1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02ad1-151">createdDateTime</span></span>|<span data-ttu-id="02ad1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02ad1-152">DateTimeOffset</span></span>|<span data-ttu-id="02ad1-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="02ad1-153">DateTime the object was created.</span></span> <span data-ttu-id="02ad1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-155">description</span><span class="sxs-lookup"><span data-stu-id="02ad1-155">description</span></span>|<span data-ttu-id="02ad1-156">String</span><span class="sxs-lookup"><span data-stu-id="02ad1-156">String</span></span>|<span data-ttu-id="02ad1-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02ad1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="02ad1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="02ad1-159">displayName</span></span>|<span data-ttu-id="02ad1-160">Строка</span><span class="sxs-lookup"><span data-stu-id="02ad1-160">String</span></span>|<span data-ttu-id="02ad1-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02ad1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="02ad1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-163">version</span><span class="sxs-lookup"><span data-stu-id="02ad1-163">version</span></span>|<span data-ttu-id="02ad1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="02ad1-164">Int32</span></span>|<span data-ttu-id="02ad1-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="02ad1-165">Version of the device configuration.</span></span> <span data-ttu-id="02ad1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="02ad1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02ad1-167">Теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="02ad1-167">teacherCertificateSettings</span></span>|<span data-ttu-id="02ad1-168">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="02ad1-168">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="02ad1-169">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="02ad1-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="02ad1-170">Студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="02ad1-170">studentCertificateSettings</span></span>|<span data-ttu-id="02ad1-171">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="02ad1-171">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="02ad1-172">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="02ad1-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="02ad1-173">Девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="02ad1-173">deviceCertificateSettings</span></span>|<span data-ttu-id="02ad1-174">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="02ad1-174">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="02ad1-175">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="02ad1-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="02ad1-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="02ad1-176">Response</span></span>
<span data-ttu-id="02ad1-177">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02ad1-177">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02ad1-178">Пример</span><span class="sxs-lookup"><span data-stu-id="02ad1-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="02ad1-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="02ad1-179">Request</span></span>
<span data-ttu-id="02ad1-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02ad1-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1910

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```

### <a name="response"></a><span data-ttu-id="02ad1-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="02ad1-181">Response</span></span>
<span data-ttu-id="02ad1-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02ad1-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2082

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "renewalThresholdPercentage": 10,
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```




