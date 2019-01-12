---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fbc0944c27ffb9f03bd4c3e860440fed57d1e4e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960037"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="05d69-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="05d69-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="05d69-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05d69-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05d69-105">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="05d69-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05d69-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05d69-106">Prerequisites</span></span>
<span data-ttu-id="05d69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05d69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05d69-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05d69-109">Permission type</span></span>|<span data-ttu-id="05d69-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05d69-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05d69-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05d69-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05d69-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="05d69-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="05d69-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05d69-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05d69-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05d69-114">Not supported.</span></span>|
|<span data-ttu-id="05d69-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05d69-115">Application</span></span>|<span data-ttu-id="05d69-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05d69-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05d69-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05d69-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05d69-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05d69-118">Optional query parameters</span></span>
<span data-ttu-id="05d69-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05d69-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="05d69-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05d69-120">Request headers</span></span>
|<span data-ttu-id="05d69-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05d69-121">Header</span></span>|<span data-ttu-id="05d69-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05d69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05d69-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05d69-123">Authorization</span></span>|<span data-ttu-id="05d69-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05d69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05d69-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05d69-125">Accept</span></span>|<span data-ttu-id="05d69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05d69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05d69-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05d69-127">Request body</span></span>
<span data-ttu-id="05d69-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05d69-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05d69-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="05d69-129">Response</span></span>
<span data-ttu-id="05d69-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05d69-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05d69-131">Пример</span><span class="sxs-lookup"><span data-stu-id="05d69-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="05d69-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="05d69-132">Request</span></span>
<span data-ttu-id="05d69-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05d69-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="05d69-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="05d69-134">Response</span></span>
<span data-ttu-id="05d69-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="05d69-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



