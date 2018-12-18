---
title: Список объектов deviceManagementTroubleshootingEvent
description: Список свойств и связей объектов deviceManagementTroubleshootingEvent.
author: tfitzmac
ms.openlocfilehash: 7d159e6f851c1e3635a85be2ab123436e267493b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325279"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="61f01-103">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="61f01-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="61f01-104">**Важно:** API бета-версии (/beta) в Microsoft Graph находятся в режиме предварительного просмотра и подлежат изменениям.</span><span class="sxs-lookup"><span data-stu-id="61f01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61f01-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61f01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61f01-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="61f01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61f01-107">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="61f01-107">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61f01-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="61f01-108">Prerequisites</span></span>
<span data-ttu-id="61f01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61f01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61f01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61f01-111">Permission type</span></span>|<span data-ttu-id="61f01-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="61f01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61f01-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61f01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61f01-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="61f01-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="61f01-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61f01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61f01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61f01-116">Not supported.</span></span>|
|<span data-ttu-id="61f01-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61f01-117">Application</span></span>|<span data-ttu-id="61f01-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61f01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61f01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61f01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="61f01-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61f01-120">Request headers</span></span>
|<span data-ttu-id="61f01-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61f01-121">Header</span></span>|<span data-ttu-id="61f01-122">Значение</span><span class="sxs-lookup"><span data-stu-id="61f01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61f01-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61f01-123">Authorization</span></span>|<span data-ttu-id="61f01-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="61f01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61f01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="61f01-125">Accept</span></span>|<span data-ttu-id="61f01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61f01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61f01-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61f01-127">Request body</span></span>
<span data-ttu-id="61f01-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61f01-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61f01-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="61f01-129">Response</span></span>
<span data-ttu-id="61f01-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="61f01-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61f01-131">Пример</span><span class="sxs-lookup"><span data-stu-id="61f01-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="61f01-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="61f01-132">Request</span></span>
<span data-ttu-id="61f01-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61f01-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="61f01-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="61f01-134">Response</span></span>
<span data-ttu-id="61f01-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="61f01-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





