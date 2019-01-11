---
title: Получение windowsOfficeClientSecurityConfiguration
description: Получите объект windowsOfficeClientSecurityConfiguration политики безопасности.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c088f5a588d68a462adc6e7918336f687ae92137
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891296"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="06f07-103">Получение windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="06f07-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="06f07-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06f07-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06f07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06f07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06f07-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06f07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06f07-107">Получите объект [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) политики безопасности.</span><span class="sxs-lookup"><span data-stu-id="06f07-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06f07-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="06f07-108">Prerequisites</span></span>
<span data-ttu-id="06f07-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06f07-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06f07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06f07-111">Permission type</span></span>|<span data-ttu-id="06f07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06f07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06f07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06f07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06f07-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06f07-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06f07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06f07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06f07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06f07-116">Not supported.</span></span>|
|<span data-ttu-id="06f07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06f07-117">Application</span></span>|<span data-ttu-id="06f07-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06f07-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06f07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06f07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06f07-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06f07-120">Optional query parameters</span></span>
<span data-ttu-id="06f07-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06f07-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="06f07-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06f07-122">Request headers</span></span>
|<span data-ttu-id="06f07-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06f07-123">Header</span></span>|<span data-ttu-id="06f07-124">Значение</span><span class="sxs-lookup"><span data-stu-id="06f07-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06f07-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="06f07-125">Authorization</span></span>|<span data-ttu-id="06f07-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="06f07-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06f07-127">Accept</span><span class="sxs-lookup"><span data-stu-id="06f07-127">Accept</span></span>|<span data-ttu-id="06f07-128">application/json</span><span class="sxs-lookup"><span data-stu-id="06f07-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06f07-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06f07-129">Request body</span></span>
<span data-ttu-id="06f07-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06f07-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06f07-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="06f07-131">Response</span></span>
<span data-ttu-id="06f07-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="06f07-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06f07-133">Пример</span><span class="sxs-lookup"><span data-stu-id="06f07-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="06f07-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="06f07-134">Request</span></span>
<span data-ttu-id="06f07-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06f07-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="06f07-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="06f07-136">Response</span></span>
<span data-ttu-id="06f07-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="06f07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1152

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
    "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
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



