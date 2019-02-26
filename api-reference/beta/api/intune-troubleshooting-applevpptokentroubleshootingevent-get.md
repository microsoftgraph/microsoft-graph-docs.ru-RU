---
title: Получение Апплевпптокентраублешутинжевент
description: Чтение свойств и связей объекта Апплевпптокентраублешутинжевент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef73f390a7b331a9c3c9b98f9c0c3d701b379182
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174342"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="514f1-103">Получение Апплевпптокентраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="514f1-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="514f1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="514f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="514f1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="514f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="514f1-106">Чтение свойств и связей объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="514f1-106">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="514f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="514f1-107">Prerequisites</span></span>
<span data-ttu-id="514f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="514f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="514f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="514f1-110">Permission type</span></span>|<span data-ttu-id="514f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="514f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="514f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="514f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="514f1-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="514f1-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="514f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="514f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="514f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="514f1-115">Not supported.</span></span>|
|<span data-ttu-id="514f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="514f1-116">Application</span></span>|<span data-ttu-id="514f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="514f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="514f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="514f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="514f1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="514f1-119">Optional query parameters</span></span>
<span data-ttu-id="514f1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="514f1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="514f1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="514f1-121">Request headers</span></span>
|<span data-ttu-id="514f1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="514f1-122">Header</span></span>|<span data-ttu-id="514f1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="514f1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="514f1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="514f1-124">Authorization</span></span>|<span data-ttu-id="514f1-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="514f1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="514f1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="514f1-126">Accept</span></span>|<span data-ttu-id="514f1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="514f1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="514f1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="514f1-128">Request body</span></span>
<span data-ttu-id="514f1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="514f1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="514f1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="514f1-130">Response</span></span>
<span data-ttu-id="514f1-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="514f1-131">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="514f1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="514f1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="514f1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="514f1-133">Request</span></span>
<span data-ttu-id="514f1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="514f1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="514f1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="514f1-135">Response</span></span>
<span data-ttu-id="514f1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="514f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




