---
title: Получение appleVppTokenTroubleshootingEvent
description: Чтение свойства и связи объекта appleVppTokenTroubleshootingEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fce083d7a29f8cf0e69c0fb81d0c0cc13f8e58dd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430712"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="1f6ab-103">Получение appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="1f6ab-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="1f6ab-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f6ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f6ab-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f6ab-107">Чтение свойства и связи объекта [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="1f6ab-107">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f6ab-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="1f6ab-108">Prerequisites</span></span>
<span data-ttu-id="1f6ab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f6ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f6ab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f6ab-111">Permission type</span></span>|<span data-ttu-id="1f6ab-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f6ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f6ab-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f6ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f6ab-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f6ab-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1f6ab-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f6ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f6ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-116">Not supported.</span></span>|
|<span data-ttu-id="1f6ab-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f6ab-117">Application</span></span>|<span data-ttu-id="1f6ab-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f6ab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f6ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f6ab-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1f6ab-120">Optional query parameters</span></span>
<span data-ttu-id="1f6ab-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f6ab-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f6ab-122">Request headers</span></span>
|<span data-ttu-id="1f6ab-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f6ab-123">Header</span></span>|<span data-ttu-id="1f6ab-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1f6ab-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f6ab-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f6ab-125">Authorization</span></span>|<span data-ttu-id="1f6ab-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1f6ab-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f6ab-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1f6ab-127">Accept</span></span>|<span data-ttu-id="1f6ab-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1f6ab-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f6ab-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f6ab-129">Request body</span></span>
<span data-ttu-id="1f6ab-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f6ab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f6ab-131">Response</span></span>
<span data-ttu-id="1f6ab-132">Успешно завершена, этот метод возвращает `200 OK` объект [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-132">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f6ab-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1f6ab-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f6ab-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f6ab-134">Request</span></span>
<span data-ttu-id="1f6ab-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="1f6ab-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f6ab-136">Response</span></span>
<span data-ttu-id="1f6ab-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1f6ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




