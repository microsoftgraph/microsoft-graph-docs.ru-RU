---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4b60c8ba43b96419e61fa0626dfcca05f23e0c2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965951"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="b3229-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="b3229-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="b3229-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3229-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3229-105">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b3229-105">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3229-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b3229-106">Prerequisites</span></span>
<span data-ttu-id="b3229-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3229-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3229-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3229-109">Permission type</span></span>|<span data-ttu-id="b3229-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3229-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3229-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3229-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3229-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3229-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b3229-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3229-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3229-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3229-114">Not supported.</span></span>|
|<span data-ttu-id="b3229-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3229-115">Application</span></span>|<span data-ttu-id="b3229-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3229-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3229-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3229-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3229-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3229-118">Optional query parameters</span></span>
<span data-ttu-id="b3229-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3229-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3229-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3229-120">Request headers</span></span>
|<span data-ttu-id="b3229-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b3229-121">Header</span></span>|<span data-ttu-id="b3229-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b3229-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3229-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3229-123">Authorization</span></span>|<span data-ttu-id="b3229-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3229-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3229-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3229-125">Accept</span></span>|<span data-ttu-id="b3229-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3229-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3229-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3229-127">Request body</span></span>
<span data-ttu-id="b3229-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3229-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3229-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3229-129">Response</span></span>
<span data-ttu-id="b3229-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b3229-130">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3229-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b3229-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3229-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3229-132">Request</span></span>
<span data-ttu-id="b3229-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3229-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="b3229-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3229-134">Response</span></span>
<span data-ttu-id="b3229-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3229-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



