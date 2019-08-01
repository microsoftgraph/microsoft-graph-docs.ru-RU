---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9948b6797232c6d21446c9432f9284f8ed298be8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976707"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="7c827-103">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="7c827-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="7c827-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c827-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c827-105">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="7c827-105">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c827-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7c827-106">Prerequisites</span></span>
<span data-ttu-id="7c827-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c827-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c827-109">Permission type</span></span>|<span data-ttu-id="7c827-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c827-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c827-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c827-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c827-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c827-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7c827-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c827-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c827-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c827-114">Not supported.</span></span>|
|<span data-ttu-id="7c827-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c827-115">Application</span></span>|<span data-ttu-id="7c827-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c827-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c827-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c827-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="7c827-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c827-118">Request headers</span></span>
|<span data-ttu-id="7c827-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c827-119">Header</span></span>|<span data-ttu-id="7c827-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7c827-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c827-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c827-121">Authorization</span></span>|<span data-ttu-id="7c827-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c827-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c827-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7c827-123">Accept</span></span>|<span data-ttu-id="7c827-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c827-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c827-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c827-125">Request body</span></span>
<span data-ttu-id="7c827-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c827-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c827-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c827-127">Response</span></span>
<span data-ttu-id="7c827-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c827-128">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c827-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7c827-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c827-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c827-130">Request</span></span>
<span data-ttu-id="7c827-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c827-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="7c827-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c827-132">Response</span></span>
<span data-ttu-id="7c827-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c827-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



