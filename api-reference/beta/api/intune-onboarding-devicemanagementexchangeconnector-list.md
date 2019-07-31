---
title: Список объектов deviceManagementExchangeConnector
description: Список свойств и связей объектов deviceManagementExchangeConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3c424fdd5c324cbbc3c0d25be6e6b0122b5b63d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984386"
---
# <a name="list-devicemanagementexchangeconnectors"></a><span data-ttu-id="64223-103">Список объектов deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="64223-103">List deviceManagementExchangeConnectors</span></span>

> <span data-ttu-id="64223-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64223-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64223-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64223-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64223-106">Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="64223-106">List properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64223-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64223-107">Prerequisites</span></span>
<span data-ttu-id="64223-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64223-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64223-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64223-110">Permission type</span></span>|<span data-ttu-id="64223-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64223-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64223-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64223-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64223-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64223-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="64223-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64223-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64223-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64223-115">Not supported.</span></span>|
|<span data-ttu-id="64223-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64223-116">Application</span></span>|<span data-ttu-id="64223-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64223-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64223-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64223-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="64223-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64223-119">Request headers</span></span>
|<span data-ttu-id="64223-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64223-120">Header</span></span>|<span data-ttu-id="64223-121">Значение</span><span class="sxs-lookup"><span data-stu-id="64223-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64223-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64223-122">Authorization</span></span>|<span data-ttu-id="64223-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64223-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64223-124">Accept</span><span class="sxs-lookup"><span data-stu-id="64223-124">Accept</span></span>|<span data-ttu-id="64223-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64223-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64223-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64223-126">Request body</span></span>
<span data-ttu-id="64223-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64223-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64223-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="64223-128">Response</span></span>
<span data-ttu-id="64223-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64223-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64223-130">Пример</span><span class="sxs-lookup"><span data-stu-id="64223-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="64223-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="64223-131">Request</span></span>
<span data-ttu-id="64223-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64223-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
```

### <a name="response"></a><span data-ttu-id="64223-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="64223-133">Response</span></span>
<span data-ttu-id="64223-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64223-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





