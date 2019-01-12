---
title: Список объектов mobileThreatDefenseConnector
description: Список свойств и связей объектов mobileThreatDefenseConnector.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 576aa6090fddc4c5425270ddf6d24b3590aafe7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945246"
---
# <a name="list-mobilethreatdefenseconnectors"></a><span data-ttu-id="f9975-103">Список объектов mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="f9975-103">List mobileThreatDefenseConnectors</span></span>

> <span data-ttu-id="f9975-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f9975-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9975-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9975-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9975-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f9975-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9975-107">Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="f9975-107">List properties and relationships of the [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9975-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f9975-108">Prerequisites</span></span>
<span data-ttu-id="f9975-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9975-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9975-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9975-111">Permission type</span></span>|<span data-ttu-id="f9975-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9975-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9975-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9975-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9975-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9975-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f9975-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9975-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9975-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9975-116">Not supported.</span></span>|
|<span data-ttu-id="f9975-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9975-117">Application</span></span>|<span data-ttu-id="f9975-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9975-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9975-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9975-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f9975-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9975-120">Request headers</span></span>
|<span data-ttu-id="f9975-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9975-121">Header</span></span>|<span data-ttu-id="f9975-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f9975-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9975-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9975-123">Authorization</span></span>|<span data-ttu-id="f9975-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f9975-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9975-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f9975-125">Accept</span></span>|<span data-ttu-id="f9975-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9975-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9975-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9975-127">Request body</span></span>
<span data-ttu-id="f9975-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9975-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9975-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9975-129">Response</span></span>
<span data-ttu-id="f9975-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f9975-130">If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/intune-onboarding-mobilethreatdefenseconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9975-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f9975-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9975-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9975-132">Request</span></span>
<span data-ttu-id="f9975-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9975-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```

### <a name="response"></a><span data-ttu-id="f9975-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9975-134">Response</span></span>
<span data-ttu-id="f9975-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f9975-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 764

{
  "value": [
    {
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
  ]
}
```





