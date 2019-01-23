---
title: Список iosWiFiConfigurations
description: Свойства списка и связей объектов iosWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d7ad169613f022b656c248dd64aeefb6c12d40b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419970"
---
# <a name="list-ioswificonfigurations"></a><span data-ttu-id="6031f-103">Список iosWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="6031f-103">List iosWiFiConfigurations</span></span>

> <span data-ttu-id="6031f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6031f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6031f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6031f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6031f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6031f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6031f-107">Свойства списка и связей объектов [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6031f-107">List properties and relationships of the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6031f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="6031f-108">Prerequisites</span></span>
<span data-ttu-id="6031f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6031f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6031f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6031f-111">Permission type</span></span>|<span data-ttu-id="6031f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6031f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6031f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6031f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6031f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6031f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6031f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6031f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6031f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6031f-116">Not supported.</span></span>|
|<span data-ttu-id="6031f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6031f-117">Application</span></span>|<span data-ttu-id="6031f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6031f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6031f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6031f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6031f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6031f-120">Request headers</span></span>
|<span data-ttu-id="6031f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6031f-121">Header</span></span>|<span data-ttu-id="6031f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6031f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6031f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6031f-123">Authorization</span></span>|<span data-ttu-id="6031f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6031f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6031f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6031f-125">Accept</span></span>|<span data-ttu-id="6031f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6031f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6031f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6031f-127">Request body</span></span>
<span data-ttu-id="6031f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6031f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6031f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6031f-129">Response</span></span>
<span data-ttu-id="6031f-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6031f-130">If successful, this method returns a `200 OK` response code and a collection of [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6031f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6031f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6031f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6031f-132">Request</span></span>
<span data-ttu-id="6031f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6031f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6031f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6031f-134">Response</span></span>
<span data-ttu-id="6031f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6031f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
      "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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




