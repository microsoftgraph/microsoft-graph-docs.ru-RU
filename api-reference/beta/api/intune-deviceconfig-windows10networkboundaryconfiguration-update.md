---
title: Обновление windows10NetworkBoundaryConfiguration
description: Обновление свойств объекта Windows10NetworkBoundaryConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 789c366ee219104e9f0e17080771c580725f8981
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127615"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="3349d-103">Обновление windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="3349d-103">Update windows10NetworkBoundaryConfiguration</span></span>

<span data-ttu-id="3349d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3349d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3349d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3349d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3349d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3349d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3349d-107">Обновление свойств объекта [Windows10NetworkBoundaryConfiguration.](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3349d-107">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3349d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3349d-108">Prerequisites</span></span>
<span data-ttu-id="3349d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3349d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3349d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3349d-111">Permission type</span></span>|<span data-ttu-id="3349d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3349d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3349d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3349d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3349d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3349d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3349d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3349d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3349d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3349d-116">Not supported.</span></span>|
|<span data-ttu-id="3349d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3349d-117">Application</span></span>|<span data-ttu-id="3349d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3349d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3349d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3349d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3349d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3349d-120">Request headers</span></span>
|<span data-ttu-id="3349d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3349d-121">Header</span></span>|<span data-ttu-id="3349d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3349d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3349d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3349d-123">Authorization</span></span>|<span data-ttu-id="3349d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3349d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3349d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3349d-125">Accept</span></span>|<span data-ttu-id="3349d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3349d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3349d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3349d-127">Request body</span></span>
<span data-ttu-id="3349d-128">В теле запроса поставляем представление JSON для [объекта Windows10NetworkBoundaryConfiguration.](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3349d-128">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="3349d-129">В следующей таблице показаны свойства, необходимые при создании [windows10NetworkBoundaryConfiguration.](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3349d-129">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="3349d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3349d-130">Property</span></span>|<span data-ttu-id="3349d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3349d-131">Type</span></span>|<span data-ttu-id="3349d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3349d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3349d-133">id</span><span class="sxs-lookup"><span data-stu-id="3349d-133">id</span></span>|<span data-ttu-id="3349d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3349d-134">String</span></span>|<span data-ttu-id="3349d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3349d-135">Key of the entity.</span></span> <span data-ttu-id="3349d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3349d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3349d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3349d-138">DateTimeOffset</span></span>|<span data-ttu-id="3349d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3349d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3349d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3349d-141">roleScopeTagIds</span></span>|<span data-ttu-id="3349d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3349d-142">String collection</span></span>|<span data-ttu-id="3349d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3349d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3349d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3349d-145">supportsScopeTags</span></span>|<span data-ttu-id="3349d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3349d-146">Boolean</span></span>|<span data-ttu-id="3349d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3349d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3349d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3349d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3349d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3349d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3349d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3349d-150">This property is read-only.</span></span> <span data-ttu-id="3349d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3349d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3349d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3349d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3349d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3349d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3349d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3349d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3349d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3349d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3349d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3349d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3349d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3349d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3349d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3349d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3349d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3349d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3349d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3349d-164">createdDateTime</span></span>|<span data-ttu-id="3349d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3349d-165">DateTimeOffset</span></span>|<span data-ttu-id="3349d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3349d-166">DateTime the object was created.</span></span> <span data-ttu-id="3349d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-168">description</span><span class="sxs-lookup"><span data-stu-id="3349d-168">description</span></span>|<span data-ttu-id="3349d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3349d-169">String</span></span>|<span data-ttu-id="3349d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3349d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3349d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3349d-172">displayName</span></span>|<span data-ttu-id="3349d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3349d-173">String</span></span>|<span data-ttu-id="3349d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3349d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3349d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-176">version</span><span class="sxs-lookup"><span data-stu-id="3349d-176">version</span></span>|<span data-ttu-id="3349d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3349d-177">Int32</span></span>|<span data-ttu-id="3349d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3349d-178">Version of the device configuration.</span></span> <span data-ttu-id="3349d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3349d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3349d-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="3349d-180">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="3349d-181">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="3349d-181">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="3349d-182">Политика изоляции сети Windows</span><span class="sxs-lookup"><span data-stu-id="3349d-182">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="3349d-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="3349d-183">Response</span></span>
<span data-ttu-id="3349d-184">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3349d-184">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3349d-185">Пример</span><span class="sxs-lookup"><span data-stu-id="3349d-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="3349d-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="3349d-186">Request</span></span>
<span data-ttu-id="3349d-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3349d-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1919

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.ipRange"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="3349d-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="3349d-188">Response</span></span>
<span data-ttu-id="3349d-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3349d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2091

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.ipRange"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```




