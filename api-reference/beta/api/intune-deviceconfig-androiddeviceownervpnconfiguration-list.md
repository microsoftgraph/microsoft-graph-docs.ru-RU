---
title: Список Андроиддевицеовнервпнконфигуратионс
description: Список свойств и связей объектов Андроиддевицеовнервпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e811c0362d02b637d167fea42c0c0014db2fe08b
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123311"
---
# <a name="list-androiddeviceownervpnconfigurations"></a><span data-ttu-id="409be-103">Список Андроиддевицеовнервпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="409be-103">List androidDeviceOwnerVpnConfigurations</span></span>

<span data-ttu-id="409be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="409be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="409be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="409be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="409be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="409be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="409be-107">Список свойств и связей объектов [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="409be-107">List properties and relationships of the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="409be-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="409be-108">Prerequisites</span></span>
<span data-ttu-id="409be-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="409be-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="409be-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="409be-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="409be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="409be-111">Permission type</span></span>|<span data-ttu-id="409be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="409be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="409be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="409be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="409be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="409be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="409be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="409be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="409be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="409be-116">Not supported.</span></span>|
|<span data-ttu-id="409be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="409be-117">Application</span></span>|<span data-ttu-id="409be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="409be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="409be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="409be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="409be-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="409be-120">Request headers</span></span>
|<span data-ttu-id="409be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="409be-121">Header</span></span>|<span data-ttu-id="409be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="409be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="409be-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="409be-123">Authorization</span></span>|<span data-ttu-id="409be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="409be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="409be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="409be-125">Accept</span></span>|<span data-ttu-id="409be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="409be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="409be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="409be-127">Request body</span></span>
<span data-ttu-id="409be-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="409be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="409be-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="409be-129">Response</span></span>
<span data-ttu-id="409be-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнервпнконфигуратион](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="409be-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="409be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="409be-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="409be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="409be-132">Request</span></span>
<span data-ttu-id="409be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="409be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="409be-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="409be-134">Response</span></span>
<span data-ttu-id="409be-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="409be-135">Here is an example of the response.</span></span> <span data-ttu-id="409be-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="409be-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="409be-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="409be-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2187

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
      "id": "972962e3-62e3-9729-e362-2997e3622997",
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
      "authenticationMethod": "usernameAndPassword",
      "connectionName": "Connection Name value",
      "role": "Role value",
      "realm": "Realm value",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "connectionType": "pulseSecure",
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "targetedPackageIds": [
        "Targeted Package Ids value"
      ],
      "alwaysOn": true,
      "alwaysOnLockdown": true
    }
  ]
}
```



