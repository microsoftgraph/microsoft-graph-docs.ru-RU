---
title: Get deviceManagementExchangeConnector
description: Чтение свойств и связей объекта deviceManagementExchangeConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e8dbfde9950014adeee612bdf9b6ee39ed7ec55
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985643"
---
# <a name="get-devicemanagementexchangeconnector"></a><span data-ttu-id="b3aef-103">Get deviceManagementExchangeConnector</span><span class="sxs-lookup"><span data-stu-id="b3aef-103">Get deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="b3aef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3aef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3aef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3aef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3aef-106">Чтение свойств и связей объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b3aef-106">Read properties and relationships of the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3aef-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b3aef-107">Prerequisites</span></span>
<span data-ttu-id="b3aef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3aef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3aef-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3aef-110">Permission type</span></span>|<span data-ttu-id="b3aef-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3aef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3aef-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3aef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b3aef-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3aef-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b3aef-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3aef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3aef-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3aef-115">Not supported.</span></span>|
|<span data-ttu-id="b3aef-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3aef-116">Application</span></span>|<span data-ttu-id="b3aef-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3aef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3aef-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3aef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3aef-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3aef-119">Optional query parameters</span></span>
<span data-ttu-id="b3aef-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3aef-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3aef-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3aef-121">Request headers</span></span>
|<span data-ttu-id="b3aef-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3aef-122">Header</span></span>|<span data-ttu-id="b3aef-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b3aef-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3aef-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3aef-124">Authorization</span></span>|<span data-ttu-id="b3aef-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3aef-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3aef-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b3aef-126">Accept</span></span>|<span data-ttu-id="b3aef-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b3aef-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3aef-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3aef-128">Request body</span></span>
<span data-ttu-id="b3aef-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3aef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3aef-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3aef-130">Response</span></span>
<span data-ttu-id="b3aef-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b3aef-131">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3aef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b3aef-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3aef-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3aef-133">Request</span></span>
<span data-ttu-id="b3aef-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3aef-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

### <a name="response"></a><span data-ttu-id="b3aef-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3aef-135">Response</span></span>
<span data-ttu-id="b3aef-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3aef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 580

{
  "value": {
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
}
```




