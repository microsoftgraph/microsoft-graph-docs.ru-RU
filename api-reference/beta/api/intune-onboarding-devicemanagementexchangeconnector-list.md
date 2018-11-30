---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
ms.openlocfilehash: d962a657e409370d398fd6167f7a141e070c9e3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077619"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="ad826-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="ad826-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="ad826-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad826-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad826-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad826-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad826-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad826-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad826-107">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ad826-107">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad826-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad826-108">Prerequisites</span></span>
<span data-ttu-id="ad826-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad826-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad826-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad826-111">Permission type</span></span>|<span data-ttu-id="ad826-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad826-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad826-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad826-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad826-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad826-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ad826-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad826-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad826-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad826-116">Not supported.</span></span>|
|<span data-ttu-id="ad826-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad826-117">Application</span></span>|<span data-ttu-id="ad826-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad826-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad826-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad826-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ad826-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad826-120">Request headers</span></span>
|<span data-ttu-id="ad826-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad826-121">Header</span></span>|<span data-ttu-id="ad826-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad826-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad826-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad826-123">Authorization</span></span>|<span data-ttu-id="ad826-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ad826-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad826-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad826-125">Accept</span></span>|<span data-ttu-id="ad826-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad826-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad826-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad826-127">Request body</span></span>
<span data-ttu-id="ad826-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad826-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad826-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad826-129">Response</span></span>
<span data-ttu-id="ad826-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad826-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad826-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad826-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad826-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad826-132">Request</span></span>
<span data-ttu-id="ad826-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad826-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="ad826-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad826-134">Response</span></span>
<span data-ttu-id="ad826-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ad826-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





