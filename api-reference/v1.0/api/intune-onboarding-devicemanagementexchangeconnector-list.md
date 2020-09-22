---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a28b378a9c40b7d47261d10f6f54b7ec89d37a19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075114"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="5388e-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="5388e-103">List deviceManagementExchangeConnectors</span></span>

<span data-ttu-id="5388e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5388e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5388e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5388e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5388e-106">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="5388e-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5388e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5388e-107">Prerequisites</span></span>
<span data-ttu-id="5388e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5388e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5388e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5388e-110">Permission type</span></span>|<span data-ttu-id="5388e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5388e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5388e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5388e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5388e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5388e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5388e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5388e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5388e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5388e-115">Not supported.</span></span>|
|<span data-ttu-id="5388e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5388e-116">Application</span></span>|<span data-ttu-id="5388e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5388e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5388e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5388e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="5388e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5388e-119">Request headers</span></span>
|<span data-ttu-id="5388e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5388e-120">Header</span></span>|<span data-ttu-id="5388e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5388e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5388e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5388e-122">Authorization</span></span>|<span data-ttu-id="5388e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5388e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5388e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5388e-124">Accept</span></span>|<span data-ttu-id="5388e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5388e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5388e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5388e-126">Request body</span></span>
<span data-ttu-id="5388e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5388e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5388e-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5388e-128">Response</span></span>
<span data-ttu-id="5388e-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5388e-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5388e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5388e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5388e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5388e-131">Request</span></span>
<span data-ttu-id="5388e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5388e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="5388e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5388e-133">Response</span></span>
<span data-ttu-id="5388e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5388e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









