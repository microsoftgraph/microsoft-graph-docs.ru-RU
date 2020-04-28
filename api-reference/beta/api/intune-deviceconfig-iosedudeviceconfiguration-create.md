---
title: Создание Иоседудевицеконфигуратион
description: Создание нового объекта Иоседудевицеконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d2edfb2fbf16cc4822d386cadca26df6d99a429
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439251"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="270c1-103">Создание Иоседудевицеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="270c1-103">Create iosEduDeviceConfiguration</span></span>

<span data-ttu-id="270c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="270c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="270c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="270c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="270c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="270c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="270c1-107">Создание нового объекта [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="270c1-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="270c1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="270c1-108">Prerequisites</span></span>
<span data-ttu-id="270c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="270c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270c1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="270c1-111">Permission type</span></span>|<span data-ttu-id="270c1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="270c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="270c1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="270c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="270c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="270c1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="270c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="270c1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="270c1-116">Not supported.</span></span>|
|<span data-ttu-id="270c1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="270c1-117">Application</span></span>|<span data-ttu-id="270c1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="270c1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="270c1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="270c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="270c1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="270c1-120">Request headers</span></span>
|<span data-ttu-id="270c1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="270c1-121">Header</span></span>|<span data-ttu-id="270c1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="270c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="270c1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="270c1-123">Authorization</span></span>|<span data-ttu-id="270c1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="270c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="270c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="270c1-125">Accept</span></span>|<span data-ttu-id="270c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="270c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="270c1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="270c1-127">Request body</span></span>
<span data-ttu-id="270c1-128">В тексте запроса добавьте представление объекта Иоседудевицеконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="270c1-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="270c1-129">В следующей таблице приведены свойства, необходимые при создании Иоседудевицеконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="270c1-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="270c1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="270c1-130">Property</span></span>|<span data-ttu-id="270c1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="270c1-131">Type</span></span>|<span data-ttu-id="270c1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="270c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270c1-133">id</span><span class="sxs-lookup"><span data-stu-id="270c1-133">id</span></span>|<span data-ttu-id="270c1-134">String</span><span class="sxs-lookup"><span data-stu-id="270c1-134">String</span></span>|<span data-ttu-id="270c1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="270c1-135">Key of the entity.</span></span> <span data-ttu-id="270c1-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="270c1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="270c1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270c1-138">DateTimeOffset</span></span>|<span data-ttu-id="270c1-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="270c1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="270c1-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="270c1-141">roleScopeTagIds</span></span>|<span data-ttu-id="270c1-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="270c1-142">String collection</span></span>|<span data-ttu-id="270c1-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="270c1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="270c1-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="270c1-145">supportsScopeTags</span></span>|<span data-ttu-id="270c1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="270c1-146">Boolean</span></span>|<span data-ttu-id="270c1-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="270c1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="270c1-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="270c1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="270c1-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="270c1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="270c1-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="270c1-150">This property is read-only.</span></span> <span data-ttu-id="270c1-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="270c1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="270c1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="270c1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="270c1-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="270c1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="270c1-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="270c1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="270c1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="270c1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="270c1-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="270c1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="270c1-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="270c1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="270c1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="270c1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="270c1-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="270c1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="270c1-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="270c1-164">createdDateTime</span></span>|<span data-ttu-id="270c1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270c1-165">DateTimeOffset</span></span>|<span data-ttu-id="270c1-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="270c1-166">DateTime the object was created.</span></span> <span data-ttu-id="270c1-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-168">description</span><span class="sxs-lookup"><span data-stu-id="270c1-168">description</span></span>|<span data-ttu-id="270c1-169">String</span><span class="sxs-lookup"><span data-stu-id="270c1-169">String</span></span>|<span data-ttu-id="270c1-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="270c1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="270c1-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="270c1-172">displayName</span></span>|<span data-ttu-id="270c1-173">Строка</span><span class="sxs-lookup"><span data-stu-id="270c1-173">String</span></span>|<span data-ttu-id="270c1-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="270c1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="270c1-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-176">version</span><span class="sxs-lookup"><span data-stu-id="270c1-176">version</span></span>|<span data-ttu-id="270c1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="270c1-177">Int32</span></span>|<span data-ttu-id="270c1-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="270c1-178">Version of the device configuration.</span></span> <span data-ttu-id="270c1-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="270c1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="270c1-180">теачерцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="270c1-180">teacherCertificateSettings</span></span>|<span data-ttu-id="270c1-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="270c1-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="270c1-182">Доверенные корневые сертификаты и сертификаты PFX для преподавателя</span><span class="sxs-lookup"><span data-stu-id="270c1-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="270c1-183">студентцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="270c1-183">studentCertificateSettings</span></span>|<span data-ttu-id="270c1-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="270c1-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="270c1-185">Доверенные корневые сертификаты и сертификаты PFX для учащегося</span><span class="sxs-lookup"><span data-stu-id="270c1-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="270c1-186">девицецертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="270c1-186">deviceCertificateSettings</span></span>|<span data-ttu-id="270c1-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="270c1-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="270c1-188">Доверенные корневые сертификаты и сертификаты PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="270c1-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="270c1-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="270c1-189">Response</span></span>
<span data-ttu-id="270c1-190">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иоседудевицеконфигуратион](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="270c1-190">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270c1-191">Пример</span><span class="sxs-lookup"><span data-stu-id="270c1-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="270c1-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="270c1-192">Request</span></span>
<span data-ttu-id="270c1-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="270c1-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2683

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="270c1-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="270c1-194">Response</span></span>
<span data-ttu-id="270c1-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="270c1-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2855

{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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



