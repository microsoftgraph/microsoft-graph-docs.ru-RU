---
title: Создание windows10NetworkBoundaryConfiguration
description: Создание нового объекта windows10NetworkBoundaryConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ad6d656d4d9aa652bd8c17026f267cad0b52010
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42478948"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="ab733-103">Создание windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab733-103">Create windows10NetworkBoundaryConfiguration</span></span>

<span data-ttu-id="ab733-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab733-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab733-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab733-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab733-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab733-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab733-107">Создание нового объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab733-107">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab733-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ab733-108">Prerequisites</span></span>
<span data-ttu-id="ab733-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab733-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab733-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab733-111">Permission type</span></span>|<span data-ttu-id="ab733-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab733-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab733-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab733-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab733-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab733-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab733-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab733-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab733-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab733-116">Not supported.</span></span>|
|<span data-ttu-id="ab733-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab733-117">Application</span></span>|<span data-ttu-id="ab733-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab733-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab733-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab733-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab733-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ab733-120">Request headers</span></span>
|<span data-ttu-id="ab733-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab733-121">Header</span></span>|<span data-ttu-id="ab733-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab733-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab733-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab733-123">Authorization</span></span>|<span data-ttu-id="ab733-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab733-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab733-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab733-125">Accept</span></span>|<span data-ttu-id="ab733-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab733-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab733-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab733-127">Request body</span></span>
<span data-ttu-id="ab733-128">В тексте запроса добавьте представление объекта windows10NetworkBoundaryConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab733-128">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="ab733-129">В следующей таблице приведены свойства, необходимые при создании windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ab733-129">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="ab733-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab733-130">Property</span></span>|<span data-ttu-id="ab733-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ab733-131">Type</span></span>|<span data-ttu-id="ab733-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ab733-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab733-133">id</span><span class="sxs-lookup"><span data-stu-id="ab733-133">id</span></span>|<span data-ttu-id="ab733-134">String</span><span class="sxs-lookup"><span data-stu-id="ab733-134">String</span></span>|<span data-ttu-id="ab733-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ab733-135">Key of the entity.</span></span> <span data-ttu-id="ab733-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab733-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab733-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab733-138">DateTimeOffset</span></span>|<span data-ttu-id="ab733-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ab733-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab733-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab733-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab733-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ab733-142">String collection</span></span>|<span data-ttu-id="ab733-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ab733-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab733-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="ab733-145">supportsScopeTags</span></span>|<span data-ttu-id="ab733-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ab733-146">Boolean</span></span>|<span data-ttu-id="ab733-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ab733-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab733-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="ab733-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab733-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ab733-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab733-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab733-150">This property is read-only.</span></span> <span data-ttu-id="ab733-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab733-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ab733-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab733-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ab733-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab733-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ab733-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab733-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ab733-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab733-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ab733-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab733-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ab733-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab733-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ab733-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab733-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ab733-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ab733-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ab733-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab733-164">createdDateTime</span></span>|<span data-ttu-id="ab733-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab733-165">DateTimeOffset</span></span>|<span data-ttu-id="ab733-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ab733-166">DateTime the object was created.</span></span> <span data-ttu-id="ab733-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-168">description</span><span class="sxs-lookup"><span data-stu-id="ab733-168">description</span></span>|<span data-ttu-id="ab733-169">String</span><span class="sxs-lookup"><span data-stu-id="ab733-169">String</span></span>|<span data-ttu-id="ab733-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab733-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab733-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ab733-172">displayName</span></span>|<span data-ttu-id="ab733-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ab733-173">String</span></span>|<span data-ttu-id="ab733-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab733-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab733-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-176">version</span><span class="sxs-lookup"><span data-stu-id="ab733-176">version</span></span>|<span data-ttu-id="ab733-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ab733-177">Int32</span></span>|<span data-ttu-id="ab733-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ab733-178">Version of the device configuration.</span></span> <span data-ttu-id="ab733-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab733-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab733-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ab733-180">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="ab733-181">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ab733-181">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="ab733-182">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="ab733-182">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="ab733-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab733-183">Response</span></span>
<span data-ttu-id="ab733-184">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab733-184">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab733-185">Пример</span><span class="sxs-lookup"><span data-stu-id="ab733-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab733-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab733-186">Request</span></span>
<span data-ttu-id="ab733-187">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab733-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2017

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
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
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

### <a name="response"></a><span data-ttu-id="ab733-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab733-188">Response</span></span>
<span data-ttu-id="ab733-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab733-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2189

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
        "@odata.type": "microsoft.graph.iPv6Range",
        "lowerAddress": "Lower Address value",
        "upperAddress": "Upper Address value"
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





