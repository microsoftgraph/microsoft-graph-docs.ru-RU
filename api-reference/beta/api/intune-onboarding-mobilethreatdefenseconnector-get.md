---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd732a5fbb52a1c0aff63811db4a2b9a076b25d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352611"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="376e8-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="376e8-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="376e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="376e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="376e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="376e8-106">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="376e8-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="376e8-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="376e8-107">Prerequisites</span></span>
<span data-ttu-id="376e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="376e8-110">Permission type</span></span>|<span data-ttu-id="376e8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="376e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="376e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="376e8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="376e8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="376e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="376e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376e8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="376e8-115">Not supported.</span></span>|
|<span data-ttu-id="376e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="376e8-116">Application</span></span>|<span data-ttu-id="376e8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="376e8-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="376e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="376e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="376e8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="376e8-119">Optional query parameters</span></span>
<span data-ttu-id="376e8-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="376e8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="376e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="376e8-121">Request headers</span></span>
|<span data-ttu-id="376e8-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="376e8-122">Header</span></span>|<span data-ttu-id="376e8-123">Значение</span><span class="sxs-lookup"><span data-stu-id="376e8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376e8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="376e8-124">Authorization</span></span>|<span data-ttu-id="376e8-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="376e8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376e8-126">Accept</span><span class="sxs-lookup"><span data-stu-id="376e8-126">Accept</span></span>|<span data-ttu-id="376e8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="376e8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376e8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="376e8-128">Request body</span></span>
<span data-ttu-id="376e8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="376e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="376e8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="376e8-130">Response</span></span>
<span data-ttu-id="376e8-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="376e8-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="376e8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="376e8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="376e8-133">Request</span></span>
<span data-ttu-id="376e8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="376e8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="376e8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="376e8-135">Response</span></span>
<span data-ttu-id="376e8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="376e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 720

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
    "id": "e4bede14-de14-e4be-14de-bee414debee4",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "available",
    "androidEnabled": true,
    "iosEnabled": true,
    "windowsEnabled": true,
    "macEnabled": true,
    "androidDeviceBlockedOnMissingPartnerData": true,
    "iosDeviceBlockedOnMissingPartnerData": true,
    "windowsDeviceBlockedOnMissingPartnerData": true,
    "macDeviceBlockedOnMissingPartnerData": true,
    "partnerUnsupportedOsVersionBlocked": true,
    "partnerUnresponsivenessThresholdInDays": 6,
    "allowPartnerToCollectIOSApplicationMetadata": true
  }
}
```






