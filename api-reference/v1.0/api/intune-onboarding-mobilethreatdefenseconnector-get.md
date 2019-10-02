---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21b0725f451aeca503c57fb61247394cfdaf39ad
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37362262"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="ece69-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="ece69-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="ece69-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ece69-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ece69-105">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="ece69-105">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ece69-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ece69-106">Prerequisites</span></span>
<span data-ttu-id="ece69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece69-109">Permission type</span></span>|<span data-ttu-id="ece69-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece69-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ece69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ece69-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ece69-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ece69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece69-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece69-114">Not supported.</span></span>|
|<span data-ttu-id="ece69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ece69-115">Application</span></span>|<span data-ttu-id="ece69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece69-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ece69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ece69-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ece69-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ece69-118">Optional query parameters</span></span>
<span data-ttu-id="ece69-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ece69-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece69-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ece69-120">Request headers</span></span>
|<span data-ttu-id="ece69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ece69-121">Header</span></span>|<span data-ttu-id="ece69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ece69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ece69-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ece69-123">Authorization</span></span>|<span data-ttu-id="ece69-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ece69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ece69-125">Accept</span></span>|<span data-ttu-id="ece69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ece69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece69-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ece69-127">Request body</span></span>
<span data-ttu-id="ece69-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ece69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece69-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ece69-129">Response</span></span>
<span data-ttu-id="ece69-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ece69-130">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ece69-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ece69-132">Request</span></span>
<span data-ttu-id="ece69-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ece69-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="ece69-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece69-134">Response</span></span>
<span data-ttu-id="ece69-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ece69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6
  }
}
```




