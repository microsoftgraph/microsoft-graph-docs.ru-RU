---
title: Список объектов deviceManagementTroubleshootingEvent
description: Список свойств и связей объектов deviceManagementTroubleshootingEvent.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd36340ea09244948dbebcaadb9f8f6c33896477
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800174"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="ddc3b-103">Список объектов deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ddc3b-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="ddc3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddc3b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddc3b-106">Список свойств и связей объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="ddc3b-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddc3b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ddc3b-107">Prerequisites</span></span>
<span data-ttu-id="ddc3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddc3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddc3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddc3b-110">Permission type</span></span>|<span data-ttu-id="ddc3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddc3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddc3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddc3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddc3b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddc3b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ddc3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddc3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddc3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-115">Not supported.</span></span>|
|<span data-ttu-id="ddc3b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ddc3b-116">Application</span></span>|<span data-ttu-id="ddc3b-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddc3b-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddc3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddc3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ddc3b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddc3b-119">Request headers</span></span>
|<span data-ttu-id="ddc3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddc3b-120">Header</span></span>|<span data-ttu-id="ddc3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ddc3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddc3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddc3b-122">Authorization</span></span>|<span data-ttu-id="ddc3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddc3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ddc3b-124">Accept</span></span>|<span data-ttu-id="ddc3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddc3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddc3b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddc3b-126">Request body</span></span>
<span data-ttu-id="ddc3b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddc3b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ddc3b-128">Response</span></span>
<span data-ttu-id="ddc3b-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddc3b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ddc3b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddc3b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddc3b-131">Request</span></span>
<span data-ttu-id="ddc3b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="ddc3b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddc3b-133">Response</span></span>
<span data-ttu-id="ddc3b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddc3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
      "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
      "correlationId": "Correlation Id value",
      "troubleshootingErrorDetails": {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
        "context": "Context value",
        "failure": "Failure value",
        "failureDetails": "Failure Details value",
        "remediation": "Remediation value",
        "resources": [
          {
            "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
            "text": "Text value",
            "link": "Link value"
          }
        ]
      },
      "eventName": "Event Name value",
      "additionalInformation": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```




