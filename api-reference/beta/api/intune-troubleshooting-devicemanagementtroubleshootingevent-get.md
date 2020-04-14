---
title: Получение deviceManagementTroubleshootingEvent
description: Чтение свойств и связей объекта deviceManagementTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d02cca701c0e20d49ea9b84f230c90fe446a922
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43457452"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="20ff1-103">Получение deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="20ff1-103">Get deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="20ff1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20ff1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20ff1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20ff1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20ff1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20ff1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20ff1-107">Чтение свойств и связей объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span><span class="sxs-lookup"><span data-stu-id="20ff1-107">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20ff1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20ff1-108">Prerequisites</span></span>
<span data-ttu-id="20ff1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ff1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ff1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20ff1-111">Permission type</span></span>|<span data-ttu-id="20ff1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20ff1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20ff1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20ff1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20ff1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ff1-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="20ff1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20ff1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20ff1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20ff1-116">Not supported.</span></span>|
|<span data-ttu-id="20ff1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20ff1-117">Application</span></span>|<span data-ttu-id="20ff1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="20ff1-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20ff1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20ff1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20ff1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="20ff1-120">Optional query parameters</span></span>
<span data-ttu-id="20ff1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="20ff1-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20ff1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20ff1-122">Request headers</span></span>
|<span data-ttu-id="20ff1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20ff1-123">Header</span></span>|<span data-ttu-id="20ff1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="20ff1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20ff1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="20ff1-125">Authorization</span></span>|<span data-ttu-id="20ff1-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20ff1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20ff1-127">Accept</span><span class="sxs-lookup"><span data-stu-id="20ff1-127">Accept</span></span>|<span data-ttu-id="20ff1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="20ff1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20ff1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20ff1-129">Request body</span></span>
<span data-ttu-id="20ff1-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="20ff1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20ff1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="20ff1-131">Response</span></span>
<span data-ttu-id="20ff1-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20ff1-132">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20ff1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="20ff1-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="20ff1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="20ff1-134">Request</span></span>
<span data-ttu-id="20ff1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20ff1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="20ff1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="20ff1-136">Response</span></span>
<span data-ttu-id="20ff1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20ff1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



