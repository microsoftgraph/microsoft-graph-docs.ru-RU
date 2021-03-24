---
title: Список appleVppTokenTroubleshootingEvents
description: Список свойств и связей объектов appleVppTokenTroubleshootingEvent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45ddfa25929e4ec536d88ba128acc78813354d22
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123457"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="969e3-103">Список appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="969e3-103">List appleVppTokenTroubleshootingEvents</span></span>

<span data-ttu-id="969e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="969e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="969e3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="969e3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="969e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="969e3-107">Список свойств и связей [объектов appleVppTokenTroubleshootingEvent.](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="969e3-107">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="969e3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="969e3-108">Prerequisites</span></span>
<span data-ttu-id="969e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969e3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="969e3-111">Permission type</span></span>|<span data-ttu-id="969e3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="969e3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="969e3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="969e3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="969e3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969e3-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="969e3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="969e3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="969e3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969e3-116">Not supported.</span></span>|
|<span data-ttu-id="969e3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="969e3-117">Application</span></span>|<span data-ttu-id="969e3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="969e3-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="969e3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="969e3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="969e3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="969e3-120">Request headers</span></span>
|<span data-ttu-id="969e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="969e3-121">Header</span></span>|<span data-ttu-id="969e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="969e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="969e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="969e3-123">Authorization</span></span>|<span data-ttu-id="969e3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="969e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="969e3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="969e3-125">Accept</span></span>|<span data-ttu-id="969e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="969e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="969e3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="969e3-127">Request body</span></span>
<span data-ttu-id="969e3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="969e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="969e3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="969e3-129">Response</span></span>
<span data-ttu-id="969e3-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="969e3-130">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969e3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="969e3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="969e3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="969e3-132">Request</span></span>
<span data-ttu-id="969e3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="969e3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="969e3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="969e3-134">Response</span></span>
<span data-ttu-id="969e3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="969e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1071

{
  "value": [
    {
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
  ]
}
```




