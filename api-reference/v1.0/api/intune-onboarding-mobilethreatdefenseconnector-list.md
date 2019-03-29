---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 103c9bd84c1c7c798b008c394ec855aaf6e0c89d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969822"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="58cea-103">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="58cea-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="58cea-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58cea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58cea-105">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="58cea-105">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58cea-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58cea-106">Prerequisites</span></span>
<span data-ttu-id="58cea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58cea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58cea-109">Permission type</span></span>|<span data-ttu-id="58cea-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58cea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58cea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58cea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="58cea-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="58cea-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="58cea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58cea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58cea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58cea-114">Not supported.</span></span>|
|<span data-ttu-id="58cea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58cea-115">Application</span></span>|<span data-ttu-id="58cea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58cea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58cea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58cea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="58cea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58cea-118">Request headers</span></span>
|<span data-ttu-id="58cea-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58cea-119">Header</span></span>|<span data-ttu-id="58cea-120">Значение</span><span class="sxs-lookup"><span data-stu-id="58cea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58cea-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58cea-121">Authorization</span></span>|<span data-ttu-id="58cea-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58cea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58cea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="58cea-123">Accept</span></span>|<span data-ttu-id="58cea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58cea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58cea-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58cea-125">Request body</span></span>
<span data-ttu-id="58cea-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58cea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58cea-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="58cea-127">Response</span></span>
<span data-ttu-id="58cea-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58cea-128">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58cea-129">Пример</span><span class="sxs-lookup"><span data-stu-id="58cea-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="58cea-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="58cea-130">Request</span></span>
<span data-ttu-id="58cea-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58cea-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="58cea-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="58cea-132">Response</span></span>
<span data-ttu-id="58cea-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58cea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



