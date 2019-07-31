---
title: Получение Апплевпптокентраублешутинжевент
description: Чтение свойств и связей объекта Апплевпптокентраублешутинжевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c5897b48984b944a0372d3ddaf2ce33ee6bcfa8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979514"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="4f355-103">Получение Апплевпптокентраублешутинжевент</span><span class="sxs-lookup"><span data-stu-id="4f355-103">Get appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="4f355-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f355-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f355-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f355-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f355-106">Чтение свойств и связей объекта [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) .</span><span class="sxs-lookup"><span data-stu-id="4f355-106">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f355-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f355-107">Prerequisites</span></span>
<span data-ttu-id="4f355-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f355-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f355-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f355-110">Permission type</span></span>|<span data-ttu-id="4f355-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f355-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f355-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f355-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f355-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f355-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4f355-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f355-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f355-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f355-115">Not supported.</span></span>|
|<span data-ttu-id="4f355-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f355-116">Application</span></span>|<span data-ttu-id="4f355-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f355-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f355-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f355-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f355-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f355-119">Optional query parameters</span></span>
<span data-ttu-id="4f355-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f355-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f355-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f355-121">Request headers</span></span>
|<span data-ttu-id="4f355-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f355-122">Header</span></span>|<span data-ttu-id="4f355-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4f355-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f355-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f355-124">Authorization</span></span>|<span data-ttu-id="4f355-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f355-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f355-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4f355-126">Accept</span></span>|<span data-ttu-id="4f355-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4f355-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f355-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f355-128">Request body</span></span>
<span data-ttu-id="4f355-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f355-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f355-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f355-130">Response</span></span>
<span data-ttu-id="4f355-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [апплевпптокентраублешутинжевент](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f355-131">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f355-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4f355-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f355-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f355-133">Request</span></span>
<span data-ttu-id="4f355-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f355-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="4f355-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f355-135">Response</span></span>
<span data-ttu-id="4f355-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f355-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





