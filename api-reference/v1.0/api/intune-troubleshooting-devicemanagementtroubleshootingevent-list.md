---
title: Список объектов deviceManagementTroubleshootingEvent
description: Список свойств и связей объектов deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78ac4f5d2c5eb076745f90d45143b7b7a683cca5
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732883"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="99916-103">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="99916-103">List deviceManagementTroubleshootingEvents</span></span>

<span data-ttu-id="99916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99916-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99916-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99916-106">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="99916-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99916-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="99916-107">Prerequisites</span></span>
<span data-ttu-id="99916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99916-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99916-110">Permission type</span></span>|<span data-ttu-id="99916-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99916-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99916-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99916-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99916-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="99916-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="99916-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99916-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99916-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99916-115">Not supported.</span></span>|
|<span data-ttu-id="99916-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99916-116">Application</span></span>|<span data-ttu-id="99916-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99916-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99916-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99916-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="99916-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99916-119">Request headers</span></span>
|<span data-ttu-id="99916-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99916-120">Header</span></span>|<span data-ttu-id="99916-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99916-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99916-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="99916-122">Authorization</span></span>|<span data-ttu-id="99916-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99916-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99916-124">Accept</span><span class="sxs-lookup"><span data-stu-id="99916-124">Accept</span></span>|<span data-ttu-id="99916-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99916-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99916-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99916-126">Request body</span></span>
<span data-ttu-id="99916-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99916-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99916-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="99916-128">Response</span></span>
<span data-ttu-id="99916-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99916-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99916-130">Пример</span><span class="sxs-lookup"><span data-stu-id="99916-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="99916-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="99916-131">Request</span></span>
<span data-ttu-id="99916-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99916-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="99916-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="99916-133">Response</span></span>
<span data-ttu-id="99916-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99916-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









