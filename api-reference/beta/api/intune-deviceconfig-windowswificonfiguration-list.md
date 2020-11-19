---
title: Список Виндовсвификонфигуратионс
description: Список свойств и связей объектов Виндовсвификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce93d88580c0331f611514a1ba153019ad9212bb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49296442"
---
# <a name="list-windowswificonfigurations"></a><span data-ttu-id="d6a53-103">Список Виндовсвификонфигуратионс</span><span class="sxs-lookup"><span data-stu-id="d6a53-103">List windowsWifiConfigurations</span></span>

<span data-ttu-id="d6a53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6a53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6a53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6a53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6a53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6a53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6a53-107">Список свойств и связей объектов [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d6a53-107">List properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6a53-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6a53-108">Prerequisites</span></span>
<span data-ttu-id="d6a53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6a53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6a53-111">Permission type</span></span>|<span data-ttu-id="d6a53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6a53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6a53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6a53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6a53-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6a53-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6a53-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6a53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6a53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6a53-116">Not supported.</span></span>|
|<span data-ttu-id="d6a53-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6a53-117">Application</span></span>|<span data-ttu-id="d6a53-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6a53-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6a53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6a53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6a53-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6a53-120">Request headers</span></span>
|<span data-ttu-id="d6a53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6a53-121">Header</span></span>|<span data-ttu-id="d6a53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d6a53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6a53-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6a53-123">Authorization</span></span>|<span data-ttu-id="d6a53-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6a53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6a53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6a53-125">Accept</span></span>|<span data-ttu-id="d6a53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6a53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6a53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6a53-127">Request body</span></span>
<span data-ttu-id="d6a53-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6a53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6a53-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6a53-129">Response</span></span>
<span data-ttu-id="d6a53-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6a53-130">If successful, this method returns a `200 OK` response code and a collection of [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6a53-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d6a53-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6a53-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6a53-132">Request</span></span>
<span data-ttu-id="d6a53-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6a53-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d6a53-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6a53-134">Response</span></span>
<span data-ttu-id="d6a53-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6a53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1944

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
      "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
      "preSharedKey": "Pre Shared Key value",
      "wifiSecurityType": "wpaPersonal",
      "meteredConnectionLimit": "fixed",
      "ssid": "Ssid value",
      "networkName": "Network Name value",
      "connectAutomatically": true,
      "connectToPreferredNetwork": true,
      "connectWhenNetworkNameIsHidden": true,
      "proxySetting": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "forceFIPSCompliance": true
    }
  ]
}
```




