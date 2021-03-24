---
title: Список androidDeviceOwnerWiFiConfigurations
description: Список свойств и связей объектов AndroidDeviceOwnerWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 33fb286f898df93b889e4c60efd892662964c563
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138437"
---
# <a name="list-androiddeviceownerwificonfigurations"></a><span data-ttu-id="a4dcf-103">Список androidDeviceOwnerWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="a4dcf-103">List androidDeviceOwnerWiFiConfigurations</span></span>

<span data-ttu-id="a4dcf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4dcf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4dcf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4dcf-107">Список свойств и связей [объектов AndroidDeviceOwnerWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4dcf-107">List properties and relationships of the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4dcf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4dcf-108">Prerequisites</span></span>
<span data-ttu-id="a4dcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4dcf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dcf-111">Permission type</span></span>|<span data-ttu-id="a4dcf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4dcf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4dcf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4dcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4dcf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dcf-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4dcf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4dcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4dcf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-116">Not supported.</span></span>|
|<span data-ttu-id="a4dcf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4dcf-117">Application</span></span>|<span data-ttu-id="a4dcf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dcf-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4dcf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4dcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4dcf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4dcf-120">Request headers</span></span>
|<span data-ttu-id="a4dcf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4dcf-121">Header</span></span>|<span data-ttu-id="a4dcf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4dcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4dcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4dcf-123">Authorization</span></span>|<span data-ttu-id="a4dcf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4dcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4dcf-125">Accept</span></span>|<span data-ttu-id="a4dcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4dcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4dcf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4dcf-127">Request body</span></span>
<span data-ttu-id="a4dcf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4dcf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dcf-129">Response</span></span>
<span data-ttu-id="a4dcf-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-130">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4dcf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a4dcf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4dcf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4dcf-132">Request</span></span>
<span data-ttu-id="a4dcf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a4dcf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dcf-134">Response</span></span>
<span data-ttu-id="a4dcf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4dcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1643

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
      "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
      "wiFiSecurityType": "wep",
      "preSharedKey": "Pre Shared Key value",
      "preSharedKeyIsSet": true
    }
  ]
}
```




