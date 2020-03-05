---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efac6a3810793585f8210da8eab926372734c89a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457680"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="6be1e-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6be1e-103">Get deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="6be1e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6be1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6be1e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6be1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be1e-107">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="6be1e-107">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6be1e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6be1e-108">Prerequisites</span></span>
<span data-ttu-id="6be1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6be1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6be1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6be1e-111">Permission type</span></span>|<span data-ttu-id="6be1e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6be1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6be1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6be1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6be1e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be1e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6be1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6be1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6be1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6be1e-116">Not supported.</span></span>|
|<span data-ttu-id="6be1e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6be1e-117">Application</span></span>|<span data-ttu-id="6be1e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6be1e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6be1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6be1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6be1e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6be1e-120">Optional query parameters</span></span>
<span data-ttu-id="6be1e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6be1e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6be1e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6be1e-122">Request headers</span></span>
|<span data-ttu-id="6be1e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6be1e-123">Header</span></span>|<span data-ttu-id="6be1e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6be1e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6be1e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6be1e-125">Authorization</span></span>|<span data-ttu-id="6be1e-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6be1e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6be1e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6be1e-127">Accept</span></span>|<span data-ttu-id="6be1e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6be1e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6be1e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6be1e-129">Request body</span></span>
<span data-ttu-id="6be1e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6be1e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6be1e-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6be1e-131">Response</span></span>
<span data-ttu-id="6be1e-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6be1e-132">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6be1e-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6be1e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6be1e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6be1e-134">Request</span></span>
<span data-ttu-id="6be1e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6be1e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="6be1e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6be1e-136">Response</span></span>
<span data-ttu-id="6be1e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6be1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 972

{
  "value": {
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
}
```





