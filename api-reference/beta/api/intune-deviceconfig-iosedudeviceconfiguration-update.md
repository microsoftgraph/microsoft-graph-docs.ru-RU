---
title: Обновление Иоседудевицеконфигуратион
description: Обновление свойств объекта Иоседудевицеконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 596358572145978551a2943ed1480444b6dab06e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467349"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="dd451-103">Обновление Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dd451-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="dd451-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd451-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd451-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd451-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd451-106">Обновление свойств объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dd451-106">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd451-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd451-107">Prerequisites</span></span>
<span data-ttu-id="dd451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd451-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd451-110">Permission type</span></span>|<span data-ttu-id="dd451-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd451-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd451-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd451-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd451-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd451-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd451-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd451-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd451-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd451-115">Not supported.</span></span>|
|<span data-ttu-id="dd451-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd451-116">Application</span></span>|<span data-ttu-id="dd451-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd451-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd451-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd451-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dd451-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd451-119">Request headers</span></span>
|<span data-ttu-id="dd451-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd451-120">Header</span></span>|<span data-ttu-id="dd451-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dd451-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd451-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd451-122">Authorization</span></span>|<span data-ttu-id="dd451-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd451-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd451-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dd451-124">Accept</span></span>|<span data-ttu-id="dd451-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd451-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd451-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd451-126">Request body</span></span>
<span data-ttu-id="dd451-127">В тексте запроса добавьте представление объекта [Иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd451-127">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="dd451-128">В следующей таблице приведены свойства, необходимые при создании [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-128">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="dd451-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd451-129">Property</span></span>|<span data-ttu-id="dd451-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd451-130">Type</span></span>|<span data-ttu-id="dd451-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd451-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd451-132">id</span><span class="sxs-lookup"><span data-stu-id="dd451-132">id</span></span>|<span data-ttu-id="dd451-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dd451-133">String</span></span>|<span data-ttu-id="dd451-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-134">Key of the entity.</span></span> <span data-ttu-id="dd451-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd451-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dd451-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd451-137">DateTimeOffset</span></span>|<span data-ttu-id="dd451-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dd451-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd451-140">roleScopeTagIds</span></span>|<span data-ttu-id="dd451-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="dd451-141">String collection</span></span>|<span data-ttu-id="dd451-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="dd451-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd451-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="dd451-144">supportsScopeTags</span></span>|<span data-ttu-id="dd451-145">Логический</span><span class="sxs-lookup"><span data-stu-id="dd451-145">Boolean</span></span>|<span data-ttu-id="dd451-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="dd451-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd451-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="dd451-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd451-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="dd451-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd451-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd451-149">This property is read-only.</span></span> <span data-ttu-id="dd451-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd451-151">createdDateTime</span></span>|<span data-ttu-id="dd451-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd451-152">DateTimeOffset</span></span>|<span data-ttu-id="dd451-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dd451-153">DateTime the object was created.</span></span> <span data-ttu-id="dd451-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-155">description</span><span class="sxs-lookup"><span data-stu-id="dd451-155">description</span></span>|<span data-ttu-id="dd451-156">String</span><span class="sxs-lookup"><span data-stu-id="dd451-156">String</span></span>|<span data-ttu-id="dd451-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd451-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd451-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dd451-159">displayName</span></span>|<span data-ttu-id="dd451-160">String</span><span class="sxs-lookup"><span data-stu-id="dd451-160">String</span></span>|<span data-ttu-id="dd451-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd451-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd451-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-163">version</span><span class="sxs-lookup"><span data-stu-id="dd451-163">version</span></span>|<span data-ttu-id="dd451-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dd451-164">Int32</span></span>|<span data-ttu-id="dd451-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dd451-165">Version of the device configuration.</span></span> <span data-ttu-id="dd451-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dd451-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd451-167">Теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="dd451-167">teacherCertificateSettings</span></span>|<span data-ttu-id="dd451-168">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="dd451-168">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="dd451-169">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="dd451-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="dd451-170">Студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="dd451-170">studentCertificateSettings</span></span>|<span data-ttu-id="dd451-171">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="dd451-171">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="dd451-172">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="dd451-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="dd451-173">Девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="dd451-173">deviceCertificateSettings</span></span>|<span data-ttu-id="dd451-174">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="dd451-174">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="dd451-175">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="dd451-175">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="dd451-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd451-176">Response</span></span>
<span data-ttu-id="dd451-177">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd451-177">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd451-178">Пример</span><span class="sxs-lookup"><span data-stu-id="dd451-178">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd451-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd451-179">Request</span></span>
<span data-ttu-id="dd451-180">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd451-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="dd451-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd451-181">Response</span></span>
<span data-ttu-id="dd451-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd451-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





