---
title: Список windowsPhone81VpnConfigurations
description: Свойства списка и связей объектов windowsPhone81VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 86fa5b81de341b0881ccc3d8fa8a8b713eb043bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417163"
---
# <a name="list-windowsphone81vpnconfigurations"></a><span data-ttu-id="ca1fe-103">Список windowsPhone81VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="ca1fe-103">List windowsPhone81VpnConfigurations</span></span>

> <span data-ttu-id="ca1fe-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca1fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca1fe-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca1fe-107">Свойства списка и связей объектов [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ca1fe-107">List properties and relationships of the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca1fe-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ca1fe-108">Prerequisites</span></span>
<span data-ttu-id="ca1fe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca1fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca1fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca1fe-111">Permission type</span></span>|<span data-ttu-id="ca1fe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca1fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca1fe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca1fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca1fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca1fe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ca1fe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca1fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca1fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-116">Not supported.</span></span>|
|<span data-ttu-id="ca1fe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca1fe-117">Application</span></span>|<span data-ttu-id="ca1fe-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca1fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca1fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca1fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca1fe-120">Request headers</span></span>
|<span data-ttu-id="ca1fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca1fe-121">Header</span></span>|<span data-ttu-id="ca1fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca1fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca1fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca1fe-123">Authorization</span></span>|<span data-ttu-id="ca1fe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca1fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca1fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca1fe-125">Accept</span></span>|<span data-ttu-id="ca1fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca1fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca1fe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca1fe-127">Request body</span></span>
<span data-ttu-id="ca1fe-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca1fe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca1fe-129">Response</span></span>
<span data-ttu-id="ca1fe-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca1fe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ca1fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca1fe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca1fe-132">Request</span></span>
<span data-ttu-id="ca1fe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ca1fe-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca1fe-134">Response</span></span>
<span data-ttu-id="ca1fe-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ca1fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1608

{
  "value": [
    {
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
  ]
}
```




