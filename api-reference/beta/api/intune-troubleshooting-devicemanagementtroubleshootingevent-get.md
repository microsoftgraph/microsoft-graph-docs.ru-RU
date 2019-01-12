---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2f1a11b1c494ca5d233bcf962d053a11379edce3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975829"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="d46d3-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="d46d3-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="d46d3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d46d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d46d3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d46d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d46d3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d46d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d46d3-107">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="d46d3-107">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d46d3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d46d3-108">Prerequisites</span></span>
<span data-ttu-id="d46d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d46d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d46d3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d46d3-111">Permission type</span></span>|<span data-ttu-id="d46d3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d46d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d46d3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d46d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d46d3-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="d46d3-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d46d3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d46d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d46d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d46d3-116">Not supported.</span></span>|
|<span data-ttu-id="d46d3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d46d3-117">Application</span></span>|<span data-ttu-id="d46d3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d46d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d46d3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d46d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d46d3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d46d3-120">Optional query parameters</span></span>
<span data-ttu-id="d46d3-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d46d3-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d46d3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d46d3-122">Request headers</span></span>
|<span data-ttu-id="d46d3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d46d3-123">Header</span></span>|<span data-ttu-id="d46d3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d46d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d46d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d46d3-125">Authorization</span></span>|<span data-ttu-id="d46d3-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d46d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d46d3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d46d3-127">Accept</span></span>|<span data-ttu-id="d46d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d46d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d46d3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d46d3-129">Request body</span></span>
<span data-ttu-id="d46d3-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d46d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d46d3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d46d3-131">Response</span></span>
<span data-ttu-id="d46d3-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d46d3-132">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d46d3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d46d3-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d46d3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d46d3-134">Request</span></span>
<span data-ttu-id="d46d3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d46d3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="d46d3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d46d3-136">Response</span></span>
<span data-ttu-id="d46d3-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d46d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```





