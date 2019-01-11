---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3814e5d971cd0a1c04a654cb135edc6b15c22603
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884206"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="59978-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="59978-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="59978-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59978-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59978-105">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="59978-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="59978-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="59978-106">Prerequisites</span></span>
<span data-ttu-id="59978-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59978-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59978-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59978-109">Permission type</span></span>|<span data-ttu-id="59978-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59978-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59978-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59978-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59978-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="59978-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="59978-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59978-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59978-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59978-114">Not supported.</span></span>|
|<span data-ttu-id="59978-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59978-115">Application</span></span>|<span data-ttu-id="59978-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59978-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="59978-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59978-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="59978-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59978-118">Request headers</span></span>
|<span data-ttu-id="59978-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59978-119">Header</span></span>|<span data-ttu-id="59978-120">Значение</span><span class="sxs-lookup"><span data-stu-id="59978-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59978-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="59978-121">Authorization</span></span>|<span data-ttu-id="59978-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="59978-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59978-123">Accept</span><span class="sxs-lookup"><span data-stu-id="59978-123">Accept</span></span>|<span data-ttu-id="59978-124">application/json</span><span class="sxs-lookup"><span data-stu-id="59978-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59978-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="59978-125">Request body</span></span>
<span data-ttu-id="59978-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59978-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59978-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="59978-127">Response</span></span>
<span data-ttu-id="59978-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="59978-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59978-129">Пример</span><span class="sxs-lookup"><span data-stu-id="59978-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="59978-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="59978-130">Request</span></span>
<span data-ttu-id="59978-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59978-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="59978-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="59978-132">Response</span></span>
<span data-ttu-id="59978-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="59978-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
      "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "status": "connectionPending",
      "primarySmtpAddress": "Primary Smtp Address value",
      "serverName": "Server Name value",
      "connectorServerName": "Connector Server Name value",
      "exchangeConnectorType": "hosted",
      "version": "Version value",
      "exchangeAlias": "Exchange Alias value",
      "exchangeOrganization": "Exchange Organization value"
    }
  ]
}
```



