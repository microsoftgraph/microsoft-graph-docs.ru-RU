---
title: Get appleVppTokenTroubleshootingEvent
description: Чтение свойств и связей объекта appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a24bf61294673d741bf9d448ed300fcac496d6fc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123373"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="07003-103">Get appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="07003-103">Get appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="07003-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07003-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07003-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07003-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07003-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07003-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07003-107">Чтение свойств и связей [объекта appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="07003-107">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07003-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07003-108">Prerequisites</span></span>
<span data-ttu-id="07003-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07003-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07003-111">Permission type</span></span>|<span data-ttu-id="07003-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07003-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07003-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07003-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07003-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07003-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="07003-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07003-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07003-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07003-116">Not supported.</span></span>|
|<span data-ttu-id="07003-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="07003-117">Application</span></span>|<span data-ttu-id="07003-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07003-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07003-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07003-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="07003-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="07003-120">Optional query parameters</span></span>
<span data-ttu-id="07003-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="07003-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07003-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07003-122">Request headers</span></span>
|<span data-ttu-id="07003-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07003-123">Header</span></span>|<span data-ttu-id="07003-124">Значение</span><span class="sxs-lookup"><span data-stu-id="07003-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07003-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="07003-125">Authorization</span></span>|<span data-ttu-id="07003-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07003-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07003-127">Accept</span><span class="sxs-lookup"><span data-stu-id="07003-127">Accept</span></span>|<span data-ttu-id="07003-128">application/json</span><span class="sxs-lookup"><span data-stu-id="07003-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07003-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07003-129">Request body</span></span>
<span data-ttu-id="07003-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07003-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07003-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="07003-131">Response</span></span>
<span data-ttu-id="07003-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07003-132">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07003-133">Пример</span><span class="sxs-lookup"><span data-stu-id="07003-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="07003-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="07003-134">Request</span></span>
<span data-ttu-id="07003-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07003-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="07003-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="07003-136">Response</span></span>
<span data-ttu-id="07003-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07003-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1003

{
  "value": {
    "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
    "id": "09295f26-5f26-0929-265f-2909265f2909",
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
    ],
    "tokenId": "Token Id value"
  }
}
```




