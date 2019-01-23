---
title: Список appleVppTokenTroubleshootingEvents
description: Свойства списка и связей объектов appleVppTokenTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ab20a752438d0a2a4685b51582f39b614d2b791
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428917"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="c33a0-103">Список appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="c33a0-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="c33a0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c33a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c33a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c33a0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c33a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33a0-107">Свойства списка и связей объектов [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="c33a0-107">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c33a0-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="c33a0-108">Prerequisites</span></span>
<span data-ttu-id="c33a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c33a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c33a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c33a0-111">Permission type</span></span>|<span data-ttu-id="c33a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c33a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c33a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c33a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c33a0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c33a0-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c33a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c33a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c33a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33a0-116">Not supported.</span></span>|
|<span data-ttu-id="c33a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c33a0-117">Application</span></span>|<span data-ttu-id="c33a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c33a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c33a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="c33a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c33a0-120">Request headers</span></span>
|<span data-ttu-id="c33a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c33a0-121">Header</span></span>|<span data-ttu-id="c33a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c33a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c33a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c33a0-123">Authorization</span></span>|<span data-ttu-id="c33a0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c33a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c33a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c33a0-125">Accept</span></span>|<span data-ttu-id="c33a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c33a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c33a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c33a0-127">Request body</span></span>
<span data-ttu-id="c33a0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c33a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c33a0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c33a0-129">Response</span></span>
<span data-ttu-id="c33a0-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c33a0-130">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c33a0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c33a0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c33a0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c33a0-132">Request</span></span>
<span data-ttu-id="c33a0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c33a0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="c33a0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c33a0-134">Response</span></span>
<span data-ttu-id="c33a0-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c33a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




