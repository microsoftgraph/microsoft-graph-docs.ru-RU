---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 554115ef2cc26809f34dd717a281646f9dcc98e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920277"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="3bf2c-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="3bf2c-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="3bf2c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bf2c-105">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="3bf2c-105">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bf2c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3bf2c-106">Prerequisites</span></span>
<span data-ttu-id="3bf2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bf2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf2c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf2c-109">Permission type</span></span>|<span data-ttu-id="3bf2c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bf2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bf2c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bf2c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bf2c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bf2c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3bf2c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bf2c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bf2c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-114">Not supported.</span></span>|
|<span data-ttu-id="3bf2c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bf2c-115">Application</span></span>|<span data-ttu-id="3bf2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bf2c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bf2c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="3bf2c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bf2c-118">Request headers</span></span>
|<span data-ttu-id="3bf2c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bf2c-119">Header</span></span>|<span data-ttu-id="3bf2c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3bf2c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bf2c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf2c-121">Authorization</span></span>|<span data-ttu-id="3bf2c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3bf2c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bf2c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3bf2c-123">Accept</span></span>|<span data-ttu-id="3bf2c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3bf2c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bf2c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3bf2c-125">Request body</span></span>
<span data-ttu-id="3bf2c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bf2c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bf2c-127">Response</span></span>
<span data-ttu-id="3bf2c-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bf2c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3bf2c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bf2c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bf2c-130">Request</span></span>
<span data-ttu-id="3bf2c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="3bf2c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bf2c-132">Response</span></span>
<span data-ttu-id="3bf2c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3bf2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



