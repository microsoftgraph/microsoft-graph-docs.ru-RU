---
title: Получение windowsPhone81VpnConfiguration
description: Чтение свойств и связей объекта windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8fa0cc988aca601e4a609dfe785494aa064fae4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32512630"
---
# <a name="get-windowsphone81vpnconfiguration"></a><span data-ttu-id="a3297-103">Получение windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3297-103">Get windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="a3297-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3297-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3297-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3297-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3297-106">Чтение свойств и связей объекта [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a3297-106">Read properties and relationships of the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3297-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a3297-107">Prerequisites</span></span>
<span data-ttu-id="a3297-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3297-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3297-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3297-110">Permission type</span></span>|<span data-ttu-id="a3297-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3297-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3297-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3297-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3297-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3297-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3297-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3297-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3297-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3297-115">Not supported.</span></span>|
|<span data-ttu-id="a3297-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3297-116">Application</span></span>|<span data-ttu-id="a3297-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3297-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3297-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3297-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3297-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a3297-119">Optional query parameters</span></span>
<span data-ttu-id="a3297-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a3297-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3297-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3297-121">Request headers</span></span>
|<span data-ttu-id="a3297-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3297-122">Header</span></span>|<span data-ttu-id="a3297-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a3297-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3297-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3297-124">Authorization</span></span>|<span data-ttu-id="a3297-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3297-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3297-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a3297-126">Accept</span></span>|<span data-ttu-id="a3297-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3297-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3297-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a3297-128">Request body</span></span>
<span data-ttu-id="a3297-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a3297-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3297-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3297-130">Response</span></span>
<span data-ttu-id="a3297-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3297-131">If successful, this method returns a `200 OK` response code and [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3297-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a3297-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3297-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3297-133">Request</span></span>
<span data-ttu-id="a3297-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3297-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a3297-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3297-135">Response</span></span>
<span data-ttu-id="a3297-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3297-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1514

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
    "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "customXml": "Y3VzdG9tWG1s",
    "applyOnlyToWindows81": true,
    "connectionType": "f5EdgeClient",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "enableSplitTunneling": true,
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows81VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "automaticallyDetectProxySettings": true,
      "bypassProxyServerForLocalAddress": true
    },
    "bypassVpnOnCompanyWifi": true,
    "bypassVpnOnHomeWifi": true,
    "authenticationMethod": "usernameAndPassword",
    "rememberUserCredentials": true,
    "dnsSuffixSearchList": [
      "Dns Suffix Search List value"
    ]
  }
}
```





