---
title: Список macOSWiFiConfigurations
description: Список свойств и связей объектов macOSWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dbd52a086f02fad8783b9d167f4ff879da14efe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127888"
---
# <a name="list-macoswificonfigurations"></a><span data-ttu-id="e9918-103">Список macOSWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="e9918-103">List macOSWiFiConfigurations</span></span>

<span data-ttu-id="e9918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9918-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9918-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9918-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9918-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9918-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9918-107">Список свойств и связей объектов [macOSWiFiConfiguration.](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e9918-107">List properties and relationships of the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9918-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e9918-108">Prerequisites</span></span>
<span data-ttu-id="e9918-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9918-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9918-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9918-111">Permission type</span></span>|<span data-ttu-id="e9918-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9918-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9918-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9918-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9918-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9918-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9918-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9918-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9918-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9918-116">Not supported.</span></span>|
|<span data-ttu-id="e9918-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e9918-117">Application</span></span>|<span data-ttu-id="e9918-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9918-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9918-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9918-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e9918-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9918-120">Request headers</span></span>
|<span data-ttu-id="e9918-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9918-121">Header</span></span>|<span data-ttu-id="e9918-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9918-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9918-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9918-123">Authorization</span></span>|<span data-ttu-id="e9918-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9918-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9918-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9918-125">Accept</span></span>|<span data-ttu-id="e9918-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9918-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9918-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9918-127">Request body</span></span>
<span data-ttu-id="e9918-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9918-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9918-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9918-129">Response</span></span>
<span data-ttu-id="e9918-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9918-130">If successful, this method returns a `200 OK` response code and a collection of [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9918-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9918-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9918-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9918-132">Request</span></span>
<span data-ttu-id="e9918-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9918-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e9918-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9918-134">Response</span></span>
<span data-ttu-id="e9918-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9918-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1823

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
      "id": "471203fb-03fb-4712-fb03-1247fb031247",
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
      "networkName": "Network Name value",
      "ssid": "Ssid value",
      "connectAutomatically": true,
      "connectWhenNetworkNameIsHidden": true,
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```




