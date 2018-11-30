---
title: Обновление iosEduDeviceConfiguration
description: Обновление свойства объекта iosEduDeviceConfiguration.
ms.openlocfilehash: e911337bcbe220cff76d58dc01c462324bb2226f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079936"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="71851-103">Обновление iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="71851-103">Update iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="71851-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71851-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71851-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71851-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71851-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71851-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71851-107">Обновление свойства объекта [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="71851-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71851-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71851-108">Prerequisites</span></span>
<span data-ttu-id="71851-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71851-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71851-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71851-111">Permission type</span></span>|<span data-ttu-id="71851-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71851-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71851-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71851-113">Delegated (work or school account)</span></span>|<span data-ttu-id="71851-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71851-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71851-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71851-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71851-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71851-116">Not supported.</span></span>|
|<span data-ttu-id="71851-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71851-117">Application</span></span>|<span data-ttu-id="71851-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71851-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71851-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71851-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71851-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71851-120">Request headers</span></span>
|<span data-ttu-id="71851-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71851-121">Header</span></span>|<span data-ttu-id="71851-122">Значение</span><span class="sxs-lookup"><span data-stu-id="71851-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71851-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71851-123">Authorization</span></span>|<span data-ttu-id="71851-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="71851-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71851-125">Accept</span><span class="sxs-lookup"><span data-stu-id="71851-125">Accept</span></span>|<span data-ttu-id="71851-126">application/json</span><span class="sxs-lookup"><span data-stu-id="71851-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71851-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71851-127">Request body</span></span>
<span data-ttu-id="71851-128">В тексте запроса укажите представление JSON для объекта [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="71851-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="71851-129">В следующей таблице показаны свойства, которые необходимы для создания [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="71851-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="71851-130">Property</span></span>|<span data-ttu-id="71851-131">Тип</span><span class="sxs-lookup"><span data-stu-id="71851-131">Type</span></span>|<span data-ttu-id="71851-132">Описание</span><span class="sxs-lookup"><span data-stu-id="71851-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71851-133">id</span><span class="sxs-lookup"><span data-stu-id="71851-133">id</span></span>|<span data-ttu-id="71851-134">String</span><span class="sxs-lookup"><span data-stu-id="71851-134">String</span></span>|<span data-ttu-id="71851-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71851-135">Key of the entity.</span></span> <span data-ttu-id="71851-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71851-137">lastModifiedDateTime</span></span>|<span data-ttu-id="71851-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71851-138">DateTimeOffset</span></span>|<span data-ttu-id="71851-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="71851-139">DateTime the object was last modified.</span></span> <span data-ttu-id="71851-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71851-141">roleScopeTagIds</span></span>|<span data-ttu-id="71851-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71851-142">String collection</span></span>|<span data-ttu-id="71851-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="71851-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71851-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71851-145">supportsScopeTags</span></span>|<span data-ttu-id="71851-146">Логический</span><span class="sxs-lookup"><span data-stu-id="71851-146">Boolean</span></span>|<span data-ttu-id="71851-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="71851-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71851-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="71851-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71851-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="71851-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71851-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71851-150">This property is read-only.</span></span> <span data-ttu-id="71851-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71851-152">createdDateTime</span></span>|<span data-ttu-id="71851-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71851-153">DateTimeOffset</span></span>|<span data-ttu-id="71851-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="71851-154">DateTime the object was created.</span></span> <span data-ttu-id="71851-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-156">описание</span><span class="sxs-lookup"><span data-stu-id="71851-156">description</span></span>|<span data-ttu-id="71851-157">String</span><span class="sxs-lookup"><span data-stu-id="71851-157">String</span></span>|<span data-ttu-id="71851-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71851-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71851-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-160">displayName</span><span class="sxs-lookup"><span data-stu-id="71851-160">displayName</span></span>|<span data-ttu-id="71851-161">String</span><span class="sxs-lookup"><span data-stu-id="71851-161">String</span></span>|<span data-ttu-id="71851-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71851-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71851-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-164">version</span><span class="sxs-lookup"><span data-stu-id="71851-164">version</span></span>|<span data-ttu-id="71851-165">Int32</span><span class="sxs-lookup"><span data-stu-id="71851-165">Int32</span></span>|<span data-ttu-id="71851-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71851-166">Version of the device configuration.</span></span> <span data-ttu-id="71851-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71851-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71851-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="71851-168">teacherCertificateSettings</span></span>|<span data-ttu-id="71851-169">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="71851-169">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="71851-170">Сертификаты доверенных корневых и PFX для преподавателей</span><span class="sxs-lookup"><span data-stu-id="71851-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="71851-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="71851-171">studentCertificateSettings</span></span>|<span data-ttu-id="71851-172">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="71851-172">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="71851-173">Сертификаты доверенных корневых и PFX для учащихся</span><span class="sxs-lookup"><span data-stu-id="71851-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="71851-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="71851-174">deviceCertificateSettings</span></span>|<span data-ttu-id="71851-175">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="71851-175">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="71851-176">Доверенные корневые папки и PFX сертификатов для устройств</span><span class="sxs-lookup"><span data-stu-id="71851-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="71851-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="71851-177">Response</span></span>
<span data-ttu-id="71851-178">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71851-178">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71851-179">Пример</span><span class="sxs-lookup"><span data-stu-id="71851-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="71851-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="71851-180">Request</span></span>
<span data-ttu-id="71851-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71851-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1910

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="71851-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="71851-182">Response</span></span>
<span data-ttu-id="71851-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="71851-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





