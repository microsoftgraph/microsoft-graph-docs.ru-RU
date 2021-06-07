---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb82886c6bea47d308188ff148740d9a69c3461b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752520"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="495b6-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="495b6-103">Get mobileThreatDefenseConnector</span></span>

<span data-ttu-id="495b6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="495b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="495b6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="495b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="495b6-106">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="495b6-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="495b6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="495b6-107">Prerequisites</span></span>
<span data-ttu-id="495b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="495b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="495b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="495b6-110">Permission type</span></span>|<span data-ttu-id="495b6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="495b6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="495b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="495b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="495b6-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="495b6-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="495b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="495b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="495b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="495b6-115">Not supported.</span></span>|
|<span data-ttu-id="495b6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="495b6-116">Application</span></span>|<span data-ttu-id="495b6-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="495b6-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="495b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="495b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="495b6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="495b6-119">Optional query parameters</span></span>
<span data-ttu-id="495b6-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="495b6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="495b6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="495b6-121">Request headers</span></span>
|<span data-ttu-id="495b6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="495b6-122">Header</span></span>|<span data-ttu-id="495b6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="495b6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="495b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="495b6-124">Authorization</span></span>|<span data-ttu-id="495b6-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="495b6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="495b6-126">Accept</span><span class="sxs-lookup"><span data-stu-id="495b6-126">Accept</span></span>|<span data-ttu-id="495b6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="495b6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="495b6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="495b6-128">Request body</span></span>
<span data-ttu-id="495b6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="495b6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="495b6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="495b6-130">Response</span></span>
<span data-ttu-id="495b6-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="495b6-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="495b6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="495b6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="495b6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="495b6-133">Request</span></span>
<span data-ttu-id="495b6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="495b6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="495b6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="495b6-135">Response</span></span>
<span data-ttu-id="495b6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="495b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




