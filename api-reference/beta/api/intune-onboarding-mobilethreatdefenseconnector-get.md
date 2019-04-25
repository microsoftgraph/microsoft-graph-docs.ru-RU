---
title: Получение объекта mobileThreatDefenseConnector
description: Чтение свойств и связей объекта mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d200e182cd694343bd197d1c620eed520a364e5b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528626"
---
# <a name="get-mobilethreatdefenseconnector"></a><span data-ttu-id="95983-103">Получение объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="95983-103">Get mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="95983-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95983-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95983-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95983-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95983-106">Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="95983-106">Read properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95983-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="95983-107">Prerequisites</span></span>
<span data-ttu-id="95983-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95983-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95983-110">Permission type</span></span>|<span data-ttu-id="95983-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95983-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95983-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95983-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95983-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95983-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="95983-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95983-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95983-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95983-115">Not supported.</span></span>|
|<span data-ttu-id="95983-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95983-116">Application</span></span>|<span data-ttu-id="95983-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95983-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95983-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95983-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95983-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95983-119">Optional query parameters</span></span>
<span data-ttu-id="95983-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95983-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95983-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95983-121">Request headers</span></span>
|<span data-ttu-id="95983-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95983-122">Header</span></span>|<span data-ttu-id="95983-123">Значение</span><span class="sxs-lookup"><span data-stu-id="95983-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95983-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95983-124">Authorization</span></span>|<span data-ttu-id="95983-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95983-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95983-126">Accept</span><span class="sxs-lookup"><span data-stu-id="95983-126">Accept</span></span>|<span data-ttu-id="95983-127">application/json</span><span class="sxs-lookup"><span data-stu-id="95983-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95983-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95983-128">Request body</span></span>
<span data-ttu-id="95983-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95983-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95983-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="95983-130">Response</span></span>
<span data-ttu-id="95983-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95983-131">If successful, this method returns a `200 OK` response code and [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95983-132">Пример</span><span class="sxs-lookup"><span data-stu-id="95983-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="95983-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="95983-133">Request</span></span>
<span data-ttu-id="95983-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95983-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

### <a name="response"></a><span data-ttu-id="95983-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="95983-135">Response</span></span>
<span data-ttu-id="95983-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95983-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





