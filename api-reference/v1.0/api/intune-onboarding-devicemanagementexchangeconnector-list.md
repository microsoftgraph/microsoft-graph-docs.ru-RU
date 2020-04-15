---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 49f64e99b6537e9f1a0441bffd7ccb8f0fffd676
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451794"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="9a019-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="9a019-103">List deviceManagementExchangeConnectors</span></span>

<span data-ttu-id="9a019-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a019-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a019-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a019-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a019-106">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="9a019-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a019-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9a019-107">Prerequisites</span></span>
<span data-ttu-id="9a019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a019-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a019-110">Permission type</span></span>|<span data-ttu-id="9a019-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a019-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a019-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a019-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9a019-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a019-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9a019-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a019-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a019-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a019-115">Not supported.</span></span>|
|<span data-ttu-id="9a019-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a019-116">Application</span></span>|<span data-ttu-id="9a019-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a019-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a019-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a019-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="9a019-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a019-119">Request headers</span></span>
|<span data-ttu-id="9a019-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a019-120">Header</span></span>|<span data-ttu-id="9a019-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9a019-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a019-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a019-122">Authorization</span></span>|<span data-ttu-id="9a019-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a019-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a019-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9a019-124">Accept</span></span>|<span data-ttu-id="9a019-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9a019-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a019-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a019-126">Request body</span></span>
<span data-ttu-id="9a019-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a019-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a019-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a019-128">Response</span></span>
<span data-ttu-id="9a019-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a019-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a019-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9a019-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a019-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a019-131">Request</span></span>
<span data-ttu-id="9a019-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a019-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="9a019-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a019-133">Response</span></span>
<span data-ttu-id="9a019-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a019-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






