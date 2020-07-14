---
title: Получение Андроидворкпрофилевпнконфигуратион
description: Чтение свойств и связей объекта Андроидворкпрофилевпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbd15ddd8dec609a9325711fbca220a2f10d84b6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123213"
---
# <a name="get-androidworkprofilevpnconfiguration"></a><span data-ttu-id="5101c-103">Получение Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5101c-103">Get androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="5101c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5101c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5101c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5101c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5101c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5101c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5101c-107">Чтение свойств и связей объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5101c-107">Read properties and relationships of the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5101c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5101c-108">Prerequisites</span></span>
<span data-ttu-id="5101c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5101c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5101c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5101c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5101c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5101c-111">Permission type</span></span>|<span data-ttu-id="5101c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5101c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5101c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5101c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5101c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5101c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5101c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5101c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5101c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5101c-116">Not supported.</span></span>|
|<span data-ttu-id="5101c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5101c-117">Application</span></span>|<span data-ttu-id="5101c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5101c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5101c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5101c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5101c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5101c-120">Optional query parameters</span></span>
<span data-ttu-id="5101c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5101c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5101c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5101c-122">Request headers</span></span>
|<span data-ttu-id="5101c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5101c-123">Header</span></span>|<span data-ttu-id="5101c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5101c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5101c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5101c-125">Authorization</span></span>|<span data-ttu-id="5101c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5101c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5101c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5101c-127">Accept</span></span>|<span data-ttu-id="5101c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5101c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5101c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5101c-129">Request body</span></span>
<span data-ttu-id="5101c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5101c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5101c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5101c-131">Response</span></span>
<span data-ttu-id="5101c-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5101c-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5101c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5101c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5101c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5101c-134">Request</span></span>
<span data-ttu-id="5101c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5101c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5101c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5101c-136">Response</span></span>
<span data-ttu-id="5101c-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="5101c-137">Here is an example of the response.</span></span> <span data-ttu-id="5101c-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="5101c-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5101c-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5101c-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2436

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
    "id": "32910378-0378-3291-7803-913278039132",
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
    "connectionName": "Connection Name value",
    "connectionType": "pulseSecure",
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
    "fingerprint": "Fingerprint value",
    "customData": [
      {
        "@odata.type": "microsoft.graph.keyValue",
        "key": "Key value",
        "value": "Value value"
      }
    ],
    "customKeyValueData": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "authenticationMethod": "usernameAndPassword",
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
}
```



