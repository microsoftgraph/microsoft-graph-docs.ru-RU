---
title: Обновление iosEduDeviceConfiguration
description: Обновление свойств объекта iosEduDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 950f5fe05af228a123686b9d530d8723333c8322
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129883"
---
# <a name="update-iosedudeviceconfiguration"></a><span data-ttu-id="a2196-103">Обновление iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2196-103">Update iosEduDeviceConfiguration</span></span>

<span data-ttu-id="a2196-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2196-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2196-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2196-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2196-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2196-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2196-107">Обновление свойств объекта [iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2196-107">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2196-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a2196-108">Prerequisites</span></span>
<span data-ttu-id="a2196-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2196-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2196-111">Permission type</span></span>|<span data-ttu-id="a2196-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2196-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2196-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2196-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2196-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2196-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2196-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2196-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2196-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2196-116">Not supported.</span></span>|
|<span data-ttu-id="a2196-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2196-117">Application</span></span>|<span data-ttu-id="a2196-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2196-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2196-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2196-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2196-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a2196-120">Request headers</span></span>
|<span data-ttu-id="a2196-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2196-121">Header</span></span>|<span data-ttu-id="a2196-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a2196-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2196-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2196-123">Authorization</span></span>|<span data-ttu-id="a2196-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2196-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2196-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2196-125">Accept</span></span>|<span data-ttu-id="a2196-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2196-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2196-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2196-127">Request body</span></span>
<span data-ttu-id="a2196-128">В теле запроса поставляем представление JSON для [объекта iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2196-128">In the request body, supply a JSON representation for the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a2196-129">В следующей таблице показаны свойства, необходимые при создании [iosEduDeviceConfiguration.](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2196-129">The following table shows the properties that are required when you create the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>

|<span data-ttu-id="a2196-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2196-130">Property</span></span>|<span data-ttu-id="a2196-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2196-131">Type</span></span>|<span data-ttu-id="a2196-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2196-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2196-133">id</span><span class="sxs-lookup"><span data-stu-id="a2196-133">id</span></span>|<span data-ttu-id="a2196-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a2196-134">String</span></span>|<span data-ttu-id="a2196-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a2196-135">Key of the entity.</span></span> <span data-ttu-id="a2196-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2196-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a2196-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2196-138">DateTimeOffset</span></span>|<span data-ttu-id="a2196-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a2196-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a2196-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a2196-141">roleScopeTagIds</span></span>|<span data-ttu-id="a2196-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a2196-142">String collection</span></span>|<span data-ttu-id="a2196-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a2196-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a2196-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a2196-145">supportsScopeTags</span></span>|<span data-ttu-id="a2196-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2196-146">Boolean</span></span>|<span data-ttu-id="a2196-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a2196-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a2196-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="a2196-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a2196-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a2196-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a2196-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2196-150">This property is read-only.</span></span> <span data-ttu-id="a2196-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a2196-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a2196-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a2196-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a2196-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2196-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a2196-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a2196-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a2196-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a2196-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a2196-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2196-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a2196-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a2196-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a2196-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a2196-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a2196-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a2196-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a2196-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2196-164">createdDateTime</span></span>|<span data-ttu-id="a2196-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2196-165">DateTimeOffset</span></span>|<span data-ttu-id="a2196-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a2196-166">DateTime the object was created.</span></span> <span data-ttu-id="a2196-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-168">description</span><span class="sxs-lookup"><span data-stu-id="a2196-168">description</span></span>|<span data-ttu-id="a2196-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a2196-169">String</span></span>|<span data-ttu-id="a2196-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2196-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2196-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a2196-172">displayName</span></span>|<span data-ttu-id="a2196-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a2196-173">String</span></span>|<span data-ttu-id="a2196-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2196-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2196-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-176">version</span><span class="sxs-lookup"><span data-stu-id="a2196-176">version</span></span>|<span data-ttu-id="a2196-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a2196-177">Int32</span></span>|<span data-ttu-id="a2196-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a2196-178">Version of the device configuration.</span></span> <span data-ttu-id="a2196-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2196-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2196-180">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a2196-180">teacherCertificateSettings</span></span>|<span data-ttu-id="a2196-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="a2196-181">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="a2196-182">Сертификаты Trusted Root и PFX для teacher</span><span class="sxs-lookup"><span data-stu-id="a2196-182">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="a2196-183">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a2196-183">studentCertificateSettings</span></span>|<span data-ttu-id="a2196-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="a2196-184">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="a2196-185">Сертификаты Trusted Root и PFX для студента</span><span class="sxs-lookup"><span data-stu-id="a2196-185">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="a2196-186">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="a2196-186">deviceCertificateSettings</span></span>|<span data-ttu-id="a2196-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md);</span><span class="sxs-lookup"><span data-stu-id="a2196-187">[iosEduCertificateSettings](../resources/intune-deviceconfig-ioseducertificatesettings.md)</span></span>|<span data-ttu-id="a2196-188">Сертификаты Trusted Root и PFX для устройства</span><span class="sxs-lookup"><span data-stu-id="a2196-188">The Trusted Root and PFX certificates for Device</span></span>|



## <a name="response"></a><span data-ttu-id="a2196-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2196-189">Response</span></span>
<span data-ttu-id="a2196-190">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a2196-190">If successful, this method returns a `200 OK` response code and an updated [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2196-191">Пример</span><span class="sxs-lookup"><span data-stu-id="a2196-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2196-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2196-192">Request</span></span>
<span data-ttu-id="a2196-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2196-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a2196-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2196-194">Response</span></span>
<span data-ttu-id="a2196-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2196-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




