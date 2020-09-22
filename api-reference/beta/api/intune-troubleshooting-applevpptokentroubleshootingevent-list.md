---
title: Список Апплевпптокентраублешутинжевентс
description: Список свойств и связей объектов Апплевпптокентраублешутинжевент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfcaacf8dce192b7d8cb2288e19c0ea6fe725a57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999631"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="04100-103">Список Апплевпптокентраублешутинжевентс</span><span class="sxs-lookup"><span data-stu-id="04100-103">List appleVppTokenTroubleshootingEvents</span></span>

<span data-ttu-id="04100-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04100-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04100-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04100-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04100-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04100-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04100-107">Список свойств и связей объектов [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="04100-107">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04100-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="04100-108">Prerequisites</span></span>
<span data-ttu-id="04100-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04100-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04100-111">Permission type</span></span>|<span data-ttu-id="04100-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04100-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04100-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="04100-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="04100-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04100-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04100-116">Not supported.</span></span>|
|<span data-ttu-id="04100-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04100-117">Application</span></span>|<span data-ttu-id="04100-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="04100-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04100-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="04100-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04100-120">Request headers</span></span>
|<span data-ttu-id="04100-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04100-121">Header</span></span>|<span data-ttu-id="04100-122">Значение</span><span class="sxs-lookup"><span data-stu-id="04100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04100-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04100-123">Authorization</span></span>|<span data-ttu-id="04100-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04100-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04100-125">Accept</span></span>|<span data-ttu-id="04100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04100-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04100-127">Request body</span></span>
<span data-ttu-id="04100-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04100-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04100-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="04100-129">Response</span></span>
<span data-ttu-id="04100-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04100-130">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04100-131">Пример</span><span class="sxs-lookup"><span data-stu-id="04100-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="04100-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="04100-132">Request</span></span>
<span data-ttu-id="04100-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04100-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="04100-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="04100-134">Response</span></span>
<span data-ttu-id="04100-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04100-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






