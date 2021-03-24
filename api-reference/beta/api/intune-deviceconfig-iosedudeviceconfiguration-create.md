---
title: Создание iosEduDeviceConfiguration
description: Создайте новый объект iosEduDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6e9e889b740db34a74529999e83e612b866b073
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129918"
---
# <a name="create-iosedudeviceconfiguration"></a><span data-ttu-id="d7ede-103">Создание iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d7ede-103">Create iosEduDeviceConfiguration</span></span>

<span data-ttu-id="d7ede-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ede-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7ede-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ede-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7ede-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7ede-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7ede-107">Создайте новый [объект iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d7ede-107">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7ede-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d7ede-108">Prerequisites</span></span>
<span data-ttu-id="d7ede-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7ede-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7ede-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7ede-111">Permission type</span></span>|<span data-ttu-id="d7ede-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7ede-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7ede-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7ede-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7ede-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7ede-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7ede-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7ede-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7ede-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ede-116">Not supported.</span></span>|
|<span data-ttu-id="d7ede-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7ede-117">Application</span></span>|<span data-ttu-id="d7ede-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7ede-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7ede-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7ede-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d7ede-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7ede-120">Request headers</span></span>
|<span data-ttu-id="d7ede-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7ede-121">Header</span></span>|<span data-ttu-id="d7ede-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d7ede-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7ede-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7ede-123">Authorization</span></span>|<span data-ttu-id="d7ede-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7ede-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7ede-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7ede-125">Accept</span></span>|<span data-ttu-id="d7ede-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7ede-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7ede-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7ede-127">Request body</span></span>
<span data-ttu-id="d7ede-128">В теле запроса поставляем представление JSON для объекта iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7ede-128">In the request body, supply a JSON representation for the iosEduDeviceConfiguration object.</span></span>

<span data-ttu-id="d7ede-129">В следующей таблице показаны свойства, необходимые при создании iosEduDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d7ede-129">The following table shows the properties that are required when you create the iosEduDeviceConfiguration.</span></span>

|<span data-ttu-id="d7ede-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ede-130">Property</span></span>|<span data-ttu-id="d7ede-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ede-131">Type</span></span>|<span data-ttu-id="d7ede-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ede-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ede-133">id</span><span class="sxs-lookup"><span data-stu-id="d7ede-133">id</span></span>|<span data-ttu-id="d7ede-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ede-134">String</span></span>|<span data-ttu-id="d7ede-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ede-135">Key of the entity.</span></span> <span data-ttu-id="d7ede-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ede-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d7ede-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ede-138">DateTimeOffset</span></span>|<span data-ttu-id="d7ede-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ede-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d7ede-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d7ede-141">roleScopeTagIds</span></span>|<span data-ttu-id="d7ede-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d7ede-142">String collection</span></span>|<span data-ttu-id="d7ede-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="d7ede-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d7ede-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d7ede-145">supportsScopeTags</span></span>|<span data-ttu-id="d7ede-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7ede-146">Boolean</span></span>|<span data-ttu-id="d7ede-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d7ede-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d7ede-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="d7ede-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d7ede-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d7ede-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d7ede-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7ede-150">This property is read-only.</span></span> <span data-ttu-id="d7ede-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7ede-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d7ede-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d7ede-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d7ede-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7ede-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d7ede-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7ede-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d7ede-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d7ede-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d7ede-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7ede-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d7ede-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7ede-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d7ede-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7ede-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d7ede-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d7ede-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d7ede-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ede-164">createdDateTime</span></span>|<span data-ttu-id="d7ede-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ede-165">DateTimeOffset</span></span>|<span data-ttu-id="d7ede-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d7ede-166">DateTime the object was created.</span></span> <span data-ttu-id="d7ede-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-168">description</span><span class="sxs-lookup"><span data-stu-id="d7ede-168">description</span></span>|<span data-ttu-id="d7ede-169">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ede-169">String</span></span>|<span data-ttu-id="d7ede-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ede-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d7ede-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d7ede-172">displayName</span></span>|<span data-ttu-id="d7ede-173">Строка</span><span class="sxs-lookup"><span data-stu-id="d7ede-173">String</span></span>|<span data-ttu-id="d7ede-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ede-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d7ede-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-176">version</span><span class="sxs-lookup"><span data-stu-id="d7ede-176">version</span></span>|<span data-ttu-id="d7ede-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d7ede-177">Int32</span></span>|<span data-ttu-id="d7ede-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d7ede-178">Version of the device configuration.</span></span> <span data-ttu-id="d7ede-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d7ede-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d7ede-180">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="d7ede-180">teacherCertificateSettings</span></span>|<span data-ttu-id="d7ede-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d7ede-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d7ede-182">Сертификаты Trusted Root и PFX для teacher</span><span class="sxs-lookup"><span data-stu-id="d7ede-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="d7ede-183">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="d7ede-183">studentCertificateSettings</span></span>|<span data-ttu-id="d7ede-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d7ede-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d7ede-185">Сертификаты Trusted Root и PFX для студента</span><span class="sxs-lookup"><span data-stu-id="d7ede-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="d7ede-186">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="d7ede-186">deviceCertificateSettings</span></span>|<span data-ttu-id="d7ede-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="d7ede-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="d7ede-188">Сертификаты Trusted Root и PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="d7ede-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="d7ede-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7ede-189">Response</span></span>
<span data-ttu-id="d7ede-190">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d7ede-190">If successful, this method returns a `201 Created` response code and a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7ede-191">Пример</span><span class="sxs-lookup"><span data-stu-id="d7ede-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7ede-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7ede-192">Request</span></span>
<span data-ttu-id="d7ede-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7ede-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d7ede-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7ede-194">Response</span></span>
<span data-ttu-id="d7ede-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7ede-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




