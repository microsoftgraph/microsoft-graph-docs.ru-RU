---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 80425d2729fc44e7ee08e6848b68f3472b4b916c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900154"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="f8e7f-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="f8e7f-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="f8e7f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8e7f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8e7f-106">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f8e7f-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8e7f-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f8e7f-107">Prerequisites</span></span>
<span data-ttu-id="f8e7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e7f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8e7f-110">Permission type</span></span>|<span data-ttu-id="f8e7f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8e7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e7f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8e7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e7f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8e7f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f8e7f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8e7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e7f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-115">Not supported.</span></span>|
|<span data-ttu-id="f8e7f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8e7f-116">Application</span></span>|<span data-ttu-id="f8e7f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e7f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8e7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f8e7f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8e7f-119">Request headers</span></span>
|<span data-ttu-id="f8e7f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f8e7f-120">Header</span></span>|<span data-ttu-id="f8e7f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f8e7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e7f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8e7f-122">Authorization</span></span>|<span data-ttu-id="f8e7f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e7f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f8e7f-124">Accept</span></span>|<span data-ttu-id="f8e7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e7f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8e7f-126">Request body</span></span>
<span data-ttu-id="f8e7f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8e7f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8e7f-128">Response</span></span>
<span data-ttu-id="f8e7f-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e7f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f8e7f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8e7f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8e7f-131">Request</span></span>
<span data-ttu-id="f8e7f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="f8e7f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8e7f-133">Response</span></span>
<span data-ttu-id="f8e7f-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8e7f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




