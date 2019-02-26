---
title: Список объектов deviceManagementTroubleshootingEvent
description: Список свойств и связей объектов deviceManagementTroubleshootingEvent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cb62cfdf4857389510644c0a47d6cb3d5919272e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250203"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="378ab-103">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="378ab-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="378ab-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="378ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="378ab-105">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="378ab-105">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="378ab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="378ab-106">Prerequisites</span></span>
<span data-ttu-id="378ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="378ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="378ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="378ab-109">Permission type</span></span>|<span data-ttu-id="378ab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="378ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="378ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="378ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="378ab-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="378ab-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="378ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="378ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="378ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378ab-114">Not supported.</span></span>|
|<span data-ttu-id="378ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="378ab-115">Application</span></span>|<span data-ttu-id="378ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="378ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="378ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="378ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="378ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="378ab-118">Request headers</span></span>
|<span data-ttu-id="378ab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="378ab-119">Header</span></span>|<span data-ttu-id="378ab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="378ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="378ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="378ab-121">Authorization</span></span>|<span data-ttu-id="378ab-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="378ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="378ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="378ab-123">Accept</span></span>|<span data-ttu-id="378ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="378ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="378ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="378ab-125">Request body</span></span>
<span data-ttu-id="378ab-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="378ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="378ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="378ab-127">Response</span></span>
<span data-ttu-id="378ab-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="378ab-128">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="378ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="378ab-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="378ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="378ab-130">Request</span></span>
<span data-ttu-id="378ab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="378ab-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="378ab-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="378ab-132">Response</span></span>
<span data-ttu-id="378ab-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="378ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



