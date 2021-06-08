---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb61e90d6b76b90b693a92d4caef09539321cb09
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757984"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="2d7e4-103">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="2d7e4-103">List mobileThreatDefenseConnectors</span></span>

<span data-ttu-id="2d7e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d7e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d7e4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d7e4-106">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="2d7e4-106">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d7e4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2d7e4-107">Prerequisites</span></span>
<span data-ttu-id="2d7e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d7e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d7e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d7e4-110">Permission type</span></span>|<span data-ttu-id="2d7e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d7e4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d7e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d7e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d7e4-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d7e4-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d7e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d7e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d7e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-115">Not supported.</span></span>|
|<span data-ttu-id="2d7e4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2d7e4-116">Application</span></span>|<span data-ttu-id="2d7e4-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d7e4-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d7e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d7e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="2d7e4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2d7e4-119">Request headers</span></span>
|<span data-ttu-id="2d7e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d7e4-120">Header</span></span>|<span data-ttu-id="2d7e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d7e4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d7e4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d7e4-122">Authorization</span></span>|<span data-ttu-id="2d7e4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d7e4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2d7e4-124">Accept</span></span>|<span data-ttu-id="2d7e4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d7e4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d7e4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d7e4-126">Request body</span></span>
<span data-ttu-id="2d7e4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d7e4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d7e4-128">Response</span></span>
<span data-ttu-id="2d7e4-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-129">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d7e4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d7e4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d7e4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d7e4-131">Request</span></span>
<span data-ttu-id="2d7e4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="2d7e4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d7e4-133">Response</span></span>
<span data-ttu-id="2d7e4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d7e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 536

{
  "value": [
    {
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
  ]
}
```




