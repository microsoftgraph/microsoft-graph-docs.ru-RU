---
title: Получение windowsOfficeClientSecurityConfiguration
description: Получите объект windowsOfficeClientSecurityConfiguration политики безопасности.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a1619e7e1ed30afbc6b04f168f8e1fda2456e749
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409575"
---
# <a name="get-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="46839-103">Получение windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="46839-103">Get windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="46839-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46839-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46839-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46839-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46839-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46839-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46839-107">Получите объект [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) политики безопасности.</span><span class="sxs-lookup"><span data-stu-id="46839-107">Get a specific security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46839-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="46839-108">Prerequisites</span></span>
<span data-ttu-id="46839-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46839-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46839-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46839-111">Permission type</span></span>|<span data-ttu-id="46839-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46839-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46839-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46839-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46839-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46839-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="46839-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46839-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46839-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46839-116">Not supported.</span></span>|
|<span data-ttu-id="46839-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46839-117">Application</span></span>|<span data-ttu-id="46839-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46839-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46839-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46839-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{key}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46839-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46839-120">Optional query parameters</span></span>
<span data-ttu-id="46839-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="46839-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46839-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46839-122">Request headers</span></span>
|<span data-ttu-id="46839-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46839-123">Header</span></span>|<span data-ttu-id="46839-124">Значение</span><span class="sxs-lookup"><span data-stu-id="46839-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46839-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46839-125">Authorization</span></span>|<span data-ttu-id="46839-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46839-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46839-127">Accept</span><span class="sxs-lookup"><span data-stu-id="46839-127">Accept</span></span>|<span data-ttu-id="46839-128">application/json</span><span class="sxs-lookup"><span data-stu-id="46839-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46839-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46839-129">Request body</span></span>
<span data-ttu-id="46839-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46839-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46839-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="46839-131">Response</span></span>
<span data-ttu-id="46839-132">Успешно завершена, этот метод возвращает `200 OK` объект [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46839-132">If successful, this method returns a `200 OK` response code and [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46839-133">Пример</span><span class="sxs-lookup"><span data-stu-id="46839-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="46839-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="46839-134">Request</span></span>
<span data-ttu-id="46839-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46839-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="46839-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="46839-136">Response</span></span>
<span data-ttu-id="46839-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="46839-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



