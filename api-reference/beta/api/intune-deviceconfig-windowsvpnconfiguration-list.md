---
title: Список Виндовсвпнконфигуратионс
description: Список свойств и связей объектов Виндовсвпнконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eafd17c8a06dde2198f9729d8e8f48f58d139bf3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011391"
---
# <a name="list-windowsvpnconfigurations"></a><span data-ttu-id="62986-103">Список Виндовсвпнконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="62986-103">List windowsVpnConfigurations</span></span>

<span data-ttu-id="62986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62986-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62986-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62986-107">Список свойств и связей объектов [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="62986-107">List properties and relationships of the [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62986-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="62986-108">Prerequisites</span></span>
<span data-ttu-id="62986-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62986-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62986-111">Permission type</span></span>|<span data-ttu-id="62986-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62986-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62986-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62986-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62986-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="62986-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="62986-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62986-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62986-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62986-116">Not supported.</span></span>|
|<span data-ttu-id="62986-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62986-117">Application</span></span>|<span data-ttu-id="62986-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="62986-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62986-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62986-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="62986-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="62986-120">Request headers</span></span>
|<span data-ttu-id="62986-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62986-121">Header</span></span>|<span data-ttu-id="62986-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62986-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62986-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62986-123">Authorization</span></span>|<span data-ttu-id="62986-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="62986-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62986-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62986-125">Accept</span></span>|<span data-ttu-id="62986-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62986-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62986-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="62986-127">Request body</span></span>
<span data-ttu-id="62986-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="62986-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62986-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="62986-129">Response</span></span>
<span data-ttu-id="62986-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсвпнконфигуратион](../resources/intune-deviceconfig-windowsvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="62986-130">If successful, this method returns a `200 OK` response code and a collection of [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62986-131">Пример</span><span class="sxs-lookup"><span data-stu-id="62986-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="62986-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="62986-132">Request</span></span>
<span data-ttu-id="62986-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62986-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="62986-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="62986-134">Response</span></span>
<span data-ttu-id="62986-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="62986-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1673

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsVpnConfiguration",
      "id": "0d0e69cc-69cc-0d0e-cc69-0e0dcc690e0d",
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
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer",
          "description": "Description value",
          "address": "Address value",
          "isDefaultServer": true
        }
      ],
      "customXml": "Y3VzdG9tWG1s"
    }
  ]
}
```






