---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3329c7f48e94773658649caf939b4e90c816cd2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259068"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="e9d2c-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="e9d2c-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="e9d2c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9d2c-105">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="e9d2c-105">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9d2c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e9d2c-106">Prerequisites</span></span>
<span data-ttu-id="e9d2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e9d2c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9d2c-109">Permission type</span></span>|<span data-ttu-id="e9d2c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9d2c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9d2c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9d2c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9d2c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9d2c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e9d2c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9d2c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9d2c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-114">Not supported.</span></span>|
|<span data-ttu-id="e9d2c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9d2c-115">Application</span></span>|<span data-ttu-id="e9d2c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9d2c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9d2c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9d2c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e9d2c-118">Optional query parameters</span></span>
<span data-ttu-id="e9d2c-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9d2c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9d2c-120">Request headers</span></span>
|<span data-ttu-id="e9d2c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9d2c-121">Header</span></span>|<span data-ttu-id="e9d2c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e9d2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9d2c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9d2c-123">Authorization</span></span>|<span data-ttu-id="e9d2c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e9d2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9d2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9d2c-125">Accept</span></span>|<span data-ttu-id="e9d2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9d2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9d2c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9d2c-127">Request body</span></span>
<span data-ttu-id="e9d2c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9d2c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9d2c-129">Response</span></span>
<span data-ttu-id="e9d2c-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-130">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9d2c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e9d2c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9d2c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9d2c-132">Request</span></span>
<span data-ttu-id="e9d2c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="e9d2c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9d2c-134">Response</span></span>
<span data-ttu-id="e9d2c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9d2c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



