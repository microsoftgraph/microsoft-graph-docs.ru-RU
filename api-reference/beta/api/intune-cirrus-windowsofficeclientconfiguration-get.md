---
title: Получение windowsOfficeClientConfiguration
description: Получите объект windowsOfficeClientConfiguration определенной политики не связанные с безопасностью.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a53fde0620e6240923dc4093a1a28d86a3c517e0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955760"
---
# <a name="get-windowsofficeclientconfiguration"></a><span data-ttu-id="87a44-103">Получение windowsOfficeClientConfiguration</span><span class="sxs-lookup"><span data-stu-id="87a44-103">Get windowsOfficeClientConfiguration</span></span>

> <span data-ttu-id="87a44-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87a44-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87a44-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87a44-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="87a44-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87a44-107">Получите объект [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) определенной политики не связанные с безопасностью.</span><span class="sxs-lookup"><span data-stu-id="87a44-107">Get a specific non-security policy [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87a44-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="87a44-108">Prerequisites</span></span>
<span data-ttu-id="87a44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87a44-111">Permission type</span></span>|<span data-ttu-id="87a44-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87a44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a44-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87a44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87a44-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87a44-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87a44-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87a44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a44-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a44-116">Not supported.</span></span>|
|<span data-ttu-id="87a44-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87a44-117">Application</span></span>|<span data-ttu-id="87a44-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87a44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a44-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87a44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87a44-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="87a44-120">Optional query parameters</span></span>
<span data-ttu-id="87a44-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="87a44-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87a44-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87a44-122">Request headers</span></span>
|<span data-ttu-id="87a44-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87a44-123">Header</span></span>|<span data-ttu-id="87a44-124">Значение</span><span class="sxs-lookup"><span data-stu-id="87a44-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a44-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87a44-125">Authorization</span></span>|<span data-ttu-id="87a44-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="87a44-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87a44-127">Accept</span><span class="sxs-lookup"><span data-stu-id="87a44-127">Accept</span></span>|<span data-ttu-id="87a44-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87a44-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a44-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87a44-129">Request body</span></span>
<span data-ttu-id="87a44-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87a44-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87a44-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="87a44-131">Response</span></span>
<span data-ttu-id="87a44-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87a44-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientConfiguration](../resources/intune-cirrus-windowsofficeclientconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a44-133">Пример</span><span class="sxs-lookup"><span data-stu-id="87a44-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="87a44-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="87a44-134">Request</span></span>
<span data-ttu-id="87a44-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87a44-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="87a44-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="87a44-136">Response</span></span>
<span data-ttu-id="87a44-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="87a44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1144

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
    "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
    "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
    "policyPayload": "<Unknown Primitive Type Edm.Stream>",
    "description": "Description value",
    "displayName": "Display Name value",
    "priority": 8,
    "userCheckinSummary": {
      "@odata.type": "microsoft.graph.officeUserCheckinSummary",
      "succeededUserCount": 2,
      "failedUserCount": 15
    },
    "checkinStatuses": [
      {
        "@odata.type": "microsoft.graph.officeClientCheckinStatus",
        "userPrincipalName": "User Principal Name value",
        "deviceName": "Device Name value",
        "devicePlatform": "Device Platform value",
        "devicePlatformVersion": "Device Platform Version value",
        "wasSuccessful": true,
        "userId": "User Id value",
        "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
        "errorMessage": "Error Message value",
        "appliedPolicies": [
          "Applied Policies value"
        ]
      }
    ]
  }
}
```



