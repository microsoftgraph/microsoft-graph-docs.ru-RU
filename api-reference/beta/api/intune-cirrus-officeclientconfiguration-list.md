---
title: Список officeClientConfigurations
description: Получение всех политик.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9366cecbbbd34b8732982982253a4cb3bc77be8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402477"
---
# <a name="list-officeclientconfigurations"></a><span data-ttu-id="45add-103">Список officeClientConfigurations</span><span class="sxs-lookup"><span data-stu-id="45add-103">List officeClientConfigurations</span></span>

> <span data-ttu-id="45add-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45add-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45add-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45add-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45add-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45add-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45add-107">Получение всех политик.</span><span class="sxs-lookup"><span data-stu-id="45add-107">Get all policies.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45add-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="45add-108">Prerequisites</span></span>
<span data-ttu-id="45add-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45add-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45add-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45add-111">Permission type</span></span>|<span data-ttu-id="45add-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45add-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45add-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45add-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45add-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45add-114">DeviceManagementConfiguration.ReadWrite.All DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45add-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45add-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45add-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45add-116">Not supported.</span></span>|
|<span data-ttu-id="45add-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45add-117">Application</span></span>|<span data-ttu-id="45add-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45add-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45add-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45add-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45add-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45add-120">Request headers</span></span>
|<span data-ttu-id="45add-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45add-121">Header</span></span>|<span data-ttu-id="45add-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45add-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45add-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45add-123">Authorization</span></span>|<span data-ttu-id="45add-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45add-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45add-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45add-125">Accept</span></span>|<span data-ttu-id="45add-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45add-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45add-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45add-127">Request body</span></span>
<span data-ttu-id="45add-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45add-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45add-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="45add-129">Response</span></span>
<span data-ttu-id="45add-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45add-130">If successful, this method returns a `200 OK` response code and a collection of [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45add-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45add-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45add-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45add-132">Request</span></span>
<span data-ttu-id="45add-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45add-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a><span data-ttu-id="45add-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45add-134">Response</span></span>
<span data-ttu-id="45add-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45add-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



