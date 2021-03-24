---
title: Обновление iosTrustedRootCertificate
description: Обновление свойств объекта iosTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a2a861e3444d61f5b69491eb0f964c4e3092bc9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147703"
---
# <a name="update-iostrustedrootcertificate"></a><span data-ttu-id="a6f93-103">Обновление iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a6f93-103">Update iosTrustedRootCertificate</span></span>

<span data-ttu-id="a6f93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6f93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6f93-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6f93-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6f93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f93-107">Обновление свойств объекта [iosTrustedRootCertificate.](../resources/intune-deviceconfig-iostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="a6f93-107">Update the properties of a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f93-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a6f93-108">Prerequisites</span></span>
<span data-ttu-id="a6f93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6f93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f93-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6f93-111">Permission type</span></span>|<span data-ttu-id="a6f93-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6f93-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f93-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6f93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f93-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f93-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6f93-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6f93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6f93-116">Not supported.</span></span>|
|<span data-ttu-id="a6f93-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a6f93-117">Application</span></span>|<span data-ttu-id="a6f93-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6f93-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f93-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6f93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="a6f93-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6f93-120">Request headers</span></span>
|<span data-ttu-id="a6f93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6f93-121">Header</span></span>|<span data-ttu-id="a6f93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a6f93-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f93-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6f93-123">Authorization</span></span>|<span data-ttu-id="a6f93-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6f93-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f93-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6f93-125">Accept</span></span>|<span data-ttu-id="a6f93-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f93-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f93-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6f93-127">Request body</span></span>
<span data-ttu-id="a6f93-128">В теле запроса поставляем представление JSON для [объекта iosTrustedRootCertificate.](../resources/intune-deviceconfig-iostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="a6f93-128">In the request body, supply a JSON representation for the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="a6f93-129">В следующей таблице показаны свойства, необходимые при создании [iosTrustedRootCertificate.](../resources/intune-deviceconfig-iostrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="a6f93-129">The following table shows the properties that are required when you create the [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>

|<span data-ttu-id="a6f93-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6f93-130">Property</span></span>|<span data-ttu-id="a6f93-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a6f93-131">Type</span></span>|<span data-ttu-id="a6f93-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a6f93-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6f93-133">id</span><span class="sxs-lookup"><span data-stu-id="a6f93-133">id</span></span>|<span data-ttu-id="a6f93-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a6f93-134">String</span></span>|<span data-ttu-id="a6f93-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a6f93-135">Key of the entity.</span></span> <span data-ttu-id="a6f93-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6f93-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a6f93-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6f93-138">DateTimeOffset</span></span>|<span data-ttu-id="a6f93-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a6f93-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a6f93-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a6f93-141">roleScopeTagIds</span></span>|<span data-ttu-id="a6f93-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a6f93-142">String collection</span></span>|<span data-ttu-id="a6f93-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="a6f93-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a6f93-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a6f93-145">supportsScopeTags</span></span>|<span data-ttu-id="a6f93-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6f93-146">Boolean</span></span>|<span data-ttu-id="a6f93-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a6f93-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a6f93-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="a6f93-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a6f93-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a6f93-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a6f93-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6f93-150">This property is read-only.</span></span> <span data-ttu-id="a6f93-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6f93-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a6f93-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a6f93-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a6f93-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a6f93-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a6f93-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6f93-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a6f93-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a6f93-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a6f93-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a6f93-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a6f93-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6f93-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a6f93-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a6f93-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a6f93-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a6f93-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a6f93-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6f93-164">createdDateTime</span></span>|<span data-ttu-id="a6f93-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6f93-165">DateTimeOffset</span></span>|<span data-ttu-id="a6f93-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a6f93-166">DateTime the object was created.</span></span> <span data-ttu-id="a6f93-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-168">description</span><span class="sxs-lookup"><span data-stu-id="a6f93-168">description</span></span>|<span data-ttu-id="a6f93-169">Строка</span><span class="sxs-lookup"><span data-stu-id="a6f93-169">String</span></span>|<span data-ttu-id="a6f93-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6f93-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6f93-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a6f93-172">displayName</span></span>|<span data-ttu-id="a6f93-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a6f93-173">String</span></span>|<span data-ttu-id="a6f93-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6f93-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6f93-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-176">version</span><span class="sxs-lookup"><span data-stu-id="a6f93-176">version</span></span>|<span data-ttu-id="a6f93-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a6f93-177">Int32</span></span>|<span data-ttu-id="a6f93-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6f93-178">Version of the device configuration.</span></span> <span data-ttu-id="a6f93-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6f93-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6f93-180">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a6f93-180">trustedRootCertificate</span></span>|<span data-ttu-id="a6f93-181">Binary</span><span class="sxs-lookup"><span data-stu-id="a6f93-181">Binary</span></span>|<span data-ttu-id="a6f93-182">Надежный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="a6f93-182">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="a6f93-183">certFileName</span><span class="sxs-lookup"><span data-stu-id="a6f93-183">certFileName</span></span>|<span data-ttu-id="a6f93-184">Строка</span><span class="sxs-lookup"><span data-stu-id="a6f93-184">String</span></span>|<span data-ttu-id="a6f93-185">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="a6f93-185">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="a6f93-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f93-186">Response</span></span>
<span data-ttu-id="a6f93-187">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a6f93-187">If successful, this method returns a `200 OK` response code and an updated [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6f93-188">Пример</span><span class="sxs-lookup"><span data-stu-id="a6f93-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f93-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6f93-189">Request</span></span>
<span data-ttu-id="a6f93-190">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6f93-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 1136

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6f93-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6f93-191">Response</span></span>
<span data-ttu-id="a6f93-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6f93-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1308

{
  "@odata.type": "#microsoft.graph.iosTrustedRootCertificate",
  "id": "9bc72bb8-2bb8-9bc7-b82b-c79bb82bc79b",
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
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




