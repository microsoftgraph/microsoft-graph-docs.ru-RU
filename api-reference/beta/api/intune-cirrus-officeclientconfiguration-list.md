---
title: Список officeClientConfigurations
description: Получение всех политик.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: aa77b55906bdf79cb4c5e493d99d63622785f393
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954514"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="a90e9-103">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="a90e9-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="a90e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a90e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a90e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a90e9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a90e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a90e9-107">Получение всех политик.</span><span class="sxs-lookup"><span data-stu-id="a90e9-107">Get all policies.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a90e9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a90e9-108">Prerequisites</span></span>
<span data-ttu-id="a90e9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a90e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a90e9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a90e9-111">Permission type</span></span>|<span data-ttu-id="a90e9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a90e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a90e9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a90e9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a90e9-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a90e9-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a90e9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a90e9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a90e9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90e9-116">Not supported.</span></span>|
|<span data-ttu-id="a90e9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a90e9-117">Application</span></span>|<span data-ttu-id="a90e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a90e9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a90e9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a90e9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a90e9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a90e9-120">Request headers</span></span>
|<span data-ttu-id="a90e9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a90e9-121">Header</span></span>|<span data-ttu-id="a90e9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a90e9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a90e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a90e9-123">Authorization</span></span>|<span data-ttu-id="a90e9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a90e9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a90e9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a90e9-125">Accept</span></span>|<span data-ttu-id="a90e9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a90e9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a90e9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a90e9-127">Request body</span></span>
<span data-ttu-id="a90e9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a90e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a90e9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90e9-129">Response</span></span>
<span data-ttu-id="a90e9-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a90e9-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a90e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a90e9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a90e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a90e9-132">Request</span></span>
<span data-ttu-id="a90e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a90e9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="a90e9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a90e9-134">Response</span></span>
<span data-ttu-id="a90e9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a90e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1207

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeClientConfiguration",
      "id": "362ce0f0-e0f0-362c-f0e0-2c36f0e02c36",
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
  ]
}
```



