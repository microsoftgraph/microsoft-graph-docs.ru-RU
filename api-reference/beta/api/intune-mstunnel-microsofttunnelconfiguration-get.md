---
title: Получение Микрософттуннелконфигуратион
description: Чтение свойств и связей объекта Микрософттуннелконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e704513d6479b4953204fee66590f2fd8fe55c86
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242351"
---
# <a name="get-microsofttunnelconfiguration"></a><span data-ttu-id="10ff5-103">Получение Микрософттуннелконфигуратион</span><span class="sxs-lookup"><span data-stu-id="10ff5-103">Get microsoftTunnelConfiguration</span></span>

<span data-ttu-id="10ff5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ff5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10ff5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ff5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10ff5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10ff5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ff5-107">Чтение свойств и связей объекта [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="10ff5-107">Read properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10ff5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="10ff5-108">Prerequisites</span></span>
<span data-ttu-id="10ff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ff5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ff5-111">Permission type</span></span>|<span data-ttu-id="10ff5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ff5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10ff5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ff5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10ff5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="10ff5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="10ff5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ff5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ff5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ff5-116">Not supported.</span></span>|
|<span data-ttu-id="10ff5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="10ff5-117">Application</span></span>|<span data-ttu-id="10ff5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="10ff5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10ff5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ff5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10ff5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10ff5-120">Optional query parameters</span></span>
<span data-ttu-id="10ff5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10ff5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ff5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ff5-122">Request headers</span></span>
|<span data-ttu-id="10ff5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10ff5-123">Header</span></span>|<span data-ttu-id="10ff5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="10ff5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10ff5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10ff5-125">Authorization</span></span>|<span data-ttu-id="10ff5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10ff5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10ff5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="10ff5-127">Accept</span></span>|<span data-ttu-id="10ff5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="10ff5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ff5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ff5-129">Request body</span></span>
<span data-ttu-id="10ff5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10ff5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ff5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ff5-131">Response</span></span>
<span data-ttu-id="10ff5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10ff5-132">If successful, this method returns a `200 OK` response code and [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ff5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="10ff5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="10ff5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ff5-134">Request</span></span>
<span data-ttu-id="10ff5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ff5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

### <a name="response"></a><span data-ttu-id="10ff5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ff5-136">Response</span></span>
<span data-ttu-id="10ff5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10ff5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 876

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
    "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
    "displayName": "Display Name value",
    "description": "Description value",
    "network": "Network value",
    "dnsServers": [
      "Dns Servers value"
    ],
    "defaultDomainSuffix": "Default Domain Suffix value",
    "routesInclude": [
      "Routes Include value"
    ],
    "routesExclude": [
      "Routes Exclude value"
    ],
    "splitDNS": [
      "Split DNS value"
    ],
    "listenPort": 10,
    "advancedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




