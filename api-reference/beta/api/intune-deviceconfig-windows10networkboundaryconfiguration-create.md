---
title: Создание windows10NetworkBoundaryConfiguration
description: Создание нового объекта windows10NetworkBoundaryConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5004cb9808bd43ac70fc621ff97a395dfcbe604b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978082"
---
# <a name="create-windows10networkboundaryconfiguration"></a><span data-ttu-id="a3e0a-103">Создание windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3e0a-103">Create windows10NetworkBoundaryConfiguration</span></span>

> <span data-ttu-id="a3e0a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e0a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e0a-106">Создание нового объекта [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a3e0a-106">Create a new [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3e0a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3e0a-107">Prerequisites</span></span>
<span data-ttu-id="a3e0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3e0a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3e0a-110">Permission type</span></span>|<span data-ttu-id="a3e0a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3e0a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3e0a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3e0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3e0a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3e0a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3e0a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3e0a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3e0a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-115">Not supported.</span></span>|
|<span data-ttu-id="a3e0a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3e0a-116">Application</span></span>|<span data-ttu-id="a3e0a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3e0a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3e0a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3e0a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3e0a-119">Request headers</span></span>
|<span data-ttu-id="a3e0a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3e0a-120">Header</span></span>|<span data-ttu-id="a3e0a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a3e0a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3e0a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3e0a-122">Authorization</span></span>|<span data-ttu-id="a3e0a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3e0a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a3e0a-124">Accept</span></span>|<span data-ttu-id="a3e0a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3e0a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3e0a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3e0a-126">Request body</span></span>
<span data-ttu-id="a3e0a-127">В тексте запроса добавьте представление объекта windows10NetworkBoundaryConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-127">In the request body, supply a JSON representation for the windows10NetworkBoundaryConfiguration object.</span></span>

<span data-ttu-id="a3e0a-128">В следующей таблице приведены свойства, необходимые при создании windows10NetworkBoundaryConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-128">The following table shows the properties that are required when you create the windows10NetworkBoundaryConfiguration.</span></span>

|<span data-ttu-id="a3e0a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3e0a-129">Property</span></span>|<span data-ttu-id="a3e0a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a3e0a-130">Type</span></span>|<span data-ttu-id="a3e0a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a3e0a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e0a-132">id</span><span class="sxs-lookup"><span data-stu-id="a3e0a-132">id</span></span>|<span data-ttu-id="a3e0a-133">String</span><span class="sxs-lookup"><span data-stu-id="a3e0a-133">String</span></span>|<span data-ttu-id="a3e0a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-134">Key of the entity.</span></span> <span data-ttu-id="a3e0a-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e0a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a3e0a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e0a-137">DateTimeOffset</span></span>|<span data-ttu-id="a3e0a-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a3e0a-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3e0a-140">roleScopeTagIds</span></span>|<span data-ttu-id="a3e0a-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a3e0a-141">String collection</span></span>|<span data-ttu-id="a3e0a-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3e0a-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a3e0a-144">supportsScopeTags</span></span>|<span data-ttu-id="a3e0a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3e0a-145">Boolean</span></span>|<span data-ttu-id="a3e0a-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a3e0a-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a3e0a-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a3e0a-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-149">This property is read-only.</span></span> <span data-ttu-id="a3e0a-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3e0a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a3e0a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3e0a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a3e0a-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a3e0a-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3e0a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a3e0a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3e0a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a3e0a-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a3e0a-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="a3e0a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a3e0a-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="a3e0a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a3e0a-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a3e0a-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3e0a-163">createdDateTime</span></span>|<span data-ttu-id="a3e0a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3e0a-164">DateTimeOffset</span></span>|<span data-ttu-id="a3e0a-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-165">DateTime the object was created.</span></span> <span data-ttu-id="a3e0a-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-167">description</span><span class="sxs-lookup"><span data-stu-id="a3e0a-167">description</span></span>|<span data-ttu-id="a3e0a-168">String</span><span class="sxs-lookup"><span data-stu-id="a3e0a-168">String</span></span>|<span data-ttu-id="a3e0a-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3e0a-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a3e0a-171">displayName</span></span>|<span data-ttu-id="a3e0a-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a3e0a-172">String</span></span>|<span data-ttu-id="a3e0a-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3e0a-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-175">version</span><span class="sxs-lookup"><span data-stu-id="a3e0a-175">version</span></span>|<span data-ttu-id="a3e0a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a3e0a-176">Int32</span></span>|<span data-ttu-id="a3e0a-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-177">Version of the device configuration.</span></span> <span data-ttu-id="a3e0a-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3e0a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3e0a-179">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="a3e0a-179">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="a3e0a-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="a3e0a-180">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="a3e0a-181">Политика сетевой изоляции Windows</span><span class="sxs-lookup"><span data-stu-id="a3e0a-181">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="a3e0a-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e0a-182">Response</span></span>
<span data-ttu-id="a3e0a-183">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-183">If successful, this method returns a `201 Created` response code and a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3e0a-184">Пример</span><span class="sxs-lookup"><span data-stu-id="a3e0a-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3e0a-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3e0a-185">Request</span></span>
<span data-ttu-id="a3e0a-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-186">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3e0a-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3e0a-187">Response</span></span>
<span data-ttu-id="a3e0a-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3e0a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





