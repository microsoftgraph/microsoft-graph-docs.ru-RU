---
title: Создание iosEduDeviceConfiguration
description: Создание нового объекта iosEduDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: f43fc2f753f4d1c5d83aef0b50f10a2cfabe0b84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333931"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="f74f6-103">Создание iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f74f6-103">Create iosEduDeviceConfiguration</span></span>

> <span data-ttu-id="f74f6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f74f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f74f6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f74f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f74f6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f74f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f74f6-107">Создание нового объекта [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f74f6-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f74f6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f74f6-108">Prerequisites</span></span>
<span data-ttu-id="f74f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f74f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f74f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f74f6-111">Permission type</span></span>|<span data-ttu-id="f74f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f74f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f74f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f74f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f74f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f74f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f74f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f74f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f74f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f74f6-116">Not supported.</span></span>|
|<span data-ttu-id="f74f6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f74f6-117">Application</span></span>|<span data-ttu-id="f74f6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f74f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f74f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f74f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f74f6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f74f6-120">Request headers</span></span>
|<span data-ttu-id="f74f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f74f6-121">Header</span></span>|<span data-ttu-id="f74f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f74f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f74f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f74f6-123">Authorization</span></span>|<span data-ttu-id="f74f6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f74f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f74f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f74f6-125">Accept</span></span>|<span data-ttu-id="f74f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f74f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f74f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f74f6-127">Request body</span></span>
<span data-ttu-id="f74f6-128">В тексте запроса укажите представление JSON для объекта iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f74f6-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="f74f6-129">В следующей таблице показаны свойства, которые необходимы для создания iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f74f6-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="f74f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f74f6-130">Property</span></span>|<span data-ttu-id="f74f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f74f6-131">Type</span></span>|<span data-ttu-id="f74f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f74f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f74f6-133">id</span><span class="sxs-lookup"><span data-stu-id="f74f6-133">id</span></span>|<span data-ttu-id="f74f6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f74f6-134">String</span></span>|<span data-ttu-id="f74f6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f74f6-135">Key of the entity.</span></span> <span data-ttu-id="f74f6-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f74f6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f74f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f74f6-138">DateTimeOffset</span></span>|<span data-ttu-id="f74f6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f74f6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f74f6-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f74f6-141">roleScopeTagIds</span></span>|<span data-ttu-id="f74f6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f74f6-142">String collection</span></span>|<span data-ttu-id="f74f6-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f74f6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f74f6-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f74f6-145">supportsScopeTags</span></span>|<span data-ttu-id="f74f6-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="f74f6-146">Boolean</span></span>|<span data-ttu-id="f74f6-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f74f6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f74f6-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f74f6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f74f6-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f74f6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f74f6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f74f6-150">This property is read-only.</span></span> <span data-ttu-id="f74f6-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f74f6-152">createdDateTime</span></span>|<span data-ttu-id="f74f6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f74f6-153">DateTimeOffset</span></span>|<span data-ttu-id="f74f6-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f74f6-154">DateTime the object was created.</span></span> <span data-ttu-id="f74f6-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-156">описание</span><span class="sxs-lookup"><span data-stu-id="f74f6-156">description</span></span>|<span data-ttu-id="f74f6-157">Строка</span><span class="sxs-lookup"><span data-stu-id="f74f6-157">String</span></span>|<span data-ttu-id="f74f6-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f74f6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f74f6-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f74f6-160">displayName</span></span>|<span data-ttu-id="f74f6-161">Строка</span><span class="sxs-lookup"><span data-stu-id="f74f6-161">String</span></span>|<span data-ttu-id="f74f6-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f74f6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f74f6-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-164">version</span><span class="sxs-lookup"><span data-stu-id="f74f6-164">version</span></span>|<span data-ttu-id="f74f6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f74f6-165">Int32</span></span>|<span data-ttu-id="f74f6-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f74f6-166">Version of the device configuration.</span></span> <span data-ttu-id="f74f6-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f74f6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f74f6-168">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="f74f6-168">teacherCertificateSettings</span></span>|<span data-ttu-id="f74f6-169">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="f74f6-169">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="f74f6-170">Сертификаты доверенных корневых и PFX для преподавателей</span><span class="sxs-lookup"><span data-stu-id="f74f6-170">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="f74f6-171">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="f74f6-171">studentCertificateSettings</span></span>|<span data-ttu-id="f74f6-172">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="f74f6-172">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="f74f6-173">Сертификаты доверенных корневых и PFX для учащихся</span><span class="sxs-lookup"><span data-stu-id="f74f6-173">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="f74f6-174">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="f74f6-174">deviceCertificateSettings</span></span>|<span data-ttu-id="f74f6-175">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="f74f6-175">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="f74f6-176">Доверенные корневые папки и PFX сертификатов для устройств</span><span class="sxs-lookup"><span data-stu-id="f74f6-176">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="f74f6-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="f74f6-177">Response</span></span>
<span data-ttu-id="f74f6-178">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f74f6-178">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f74f6-179">Пример</span><span class="sxs-lookup"><span data-stu-id="f74f6-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="f74f6-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="f74f6-180">Request</span></span>
<span data-ttu-id="f74f6-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f74f6-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="f74f6-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="f74f6-182">Response</span></span>
<span data-ttu-id="f74f6-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f74f6-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





