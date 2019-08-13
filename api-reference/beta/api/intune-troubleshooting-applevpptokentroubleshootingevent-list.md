---
title: Список Апплевпптокентраублешутинжевентс
description: Список свойств и связей объектов Апплевпптокентраублешутинжевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ae9fb48fdae7658ba2c4f8de652b7e2481bb387f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350316"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="49d51-103">Список Апплевпптокентраублешутинжевентс</span><span class="sxs-lookup"><span data-stu-id="49d51-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="49d51-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49d51-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49d51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49d51-106">Список свойств и связей объектов [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="49d51-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49d51-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="49d51-107">Prerequisites</span></span>
<span data-ttu-id="49d51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d51-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49d51-110">Permission type</span></span>|<span data-ttu-id="49d51-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49d51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49d51-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49d51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49d51-113">\* \* TODO: определение областей \* \*</span><span class="sxs-lookup"><span data-stu-id="49d51-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="49d51-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49d51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49d51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d51-115">Not supported.</span></span>|
|<span data-ttu-id="49d51-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49d51-116">Application</span></span>|<span data-ttu-id="49d51-117">\* \* TODO: определение областей поддержка apponly \* \*</span><span class="sxs-lookup"><span data-stu-id="49d51-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="49d51-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49d51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="49d51-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49d51-119">Request headers</span></span>
|<span data-ttu-id="49d51-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49d51-120">Header</span></span>|<span data-ttu-id="49d51-121">Значение</span><span class="sxs-lookup"><span data-stu-id="49d51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49d51-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49d51-122">Authorization</span></span>|<span data-ttu-id="49d51-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49d51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49d51-124">Accept</span><span class="sxs-lookup"><span data-stu-id="49d51-124">Accept</span></span>|<span data-ttu-id="49d51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49d51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49d51-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49d51-126">Request body</span></span>
<span data-ttu-id="49d51-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49d51-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d51-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="49d51-128">Response</span></span>
<span data-ttu-id="49d51-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49d51-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49d51-130">Пример</span><span class="sxs-lookup"><span data-stu-id="49d51-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="49d51-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d51-131">Request</span></span>
<span data-ttu-id="49d51-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d51-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="49d51-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="49d51-133">Response</span></span>
<span data-ttu-id="49d51-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="49d51-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






