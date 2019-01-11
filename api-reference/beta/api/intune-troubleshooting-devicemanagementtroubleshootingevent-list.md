---
title: Список объектов deviceManagementTroubleshootingEvent
description: Список свойств и связей объектов deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e3ea9749fc67ef338c0b1ca20703208f3aee86a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885220"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="772df-103">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="772df-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="772df-104">**Важно:** API бета-версии (/beta) в Microsoft Graph находятся в режиме предварительного просмотра и подлежат изменениям.</span><span class="sxs-lookup"><span data-stu-id="772df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="772df-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="772df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="772df-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="772df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="772df-107">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="772df-107">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="772df-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="772df-108">Prerequisites</span></span>
<span data-ttu-id="772df-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="772df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="772df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="772df-111">Permission type</span></span>|<span data-ttu-id="772df-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="772df-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="772df-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="772df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="772df-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="772df-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="772df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="772df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="772df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="772df-116">Not supported.</span></span>|
|<span data-ttu-id="772df-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="772df-117">Application</span></span>|<span data-ttu-id="772df-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="772df-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="772df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="772df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="772df-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="772df-120">Request headers</span></span>
|<span data-ttu-id="772df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="772df-121">Header</span></span>|<span data-ttu-id="772df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="772df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="772df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="772df-123">Authorization</span></span>|<span data-ttu-id="772df-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="772df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="772df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="772df-125">Accept</span></span>|<span data-ttu-id="772df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="772df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="772df-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="772df-127">Request body</span></span>
<span data-ttu-id="772df-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="772df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="772df-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="772df-129">Response</span></span>
<span data-ttu-id="772df-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="772df-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="772df-131">Пример</span><span class="sxs-lookup"><span data-stu-id="772df-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="772df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="772df-132">Request</span></span>
<span data-ttu-id="772df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="772df-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="772df-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="772df-134">Response</span></span>
<span data-ttu-id="772df-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="772df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```





