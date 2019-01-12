---
title: Получение deviceManagementExchangeOnPremisesPolicy
description: Чтение свойства и связи объекта deviceManagementExchangeOnPremisesPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a7182e3064aaab99cbe5caab795d8de03f47bff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970495"
---
# <a name="get-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="676f8-103">Получение deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="676f8-103">Get deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="676f8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="676f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="676f8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="676f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="676f8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="676f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="676f8-107">Чтение свойства и связи объекта [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="676f8-107">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="676f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="676f8-108">Prerequisites</span></span>
<span data-ttu-id="676f8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="676f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="676f8-111">Permission type</span></span>|<span data-ttu-id="676f8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="676f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="676f8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="676f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="676f8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="676f8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="676f8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="676f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="676f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="676f8-116">Not supported.</span></span>|
|<span data-ttu-id="676f8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="676f8-117">Application</span></span>|<span data-ttu-id="676f8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="676f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="676f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="676f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/exchangeOnPremisesPolicy
GET /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="676f8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="676f8-120">Optional query parameters</span></span>
<span data-ttu-id="676f8-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="676f8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="676f8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="676f8-122">Request headers</span></span>
|<span data-ttu-id="676f8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="676f8-123">Header</span></span>|<span data-ttu-id="676f8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="676f8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="676f8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="676f8-125">Authorization</span></span>|<span data-ttu-id="676f8-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="676f8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="676f8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="676f8-127">Accept</span></span>|<span data-ttu-id="676f8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="676f8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="676f8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="676f8-129">Request body</span></span>
<span data-ttu-id="676f8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="676f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="676f8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="676f8-131">Response</span></span>
<span data-ttu-id="676f8-132">Успешно завершена, этот метод возвращает `200 OK` объект [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="676f8-132">If successful, this method returns a `200 OK` response code and [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="676f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="676f8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="676f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="676f8-134">Request</span></span>
<span data-ttu-id="676f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="676f8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
```

### <a name="response"></a><span data-ttu-id="676f8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="676f8-136">Response</span></span>
<span data-ttu-id="676f8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="676f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
    "id": "16e76336-6336-16e7-3663-e7163663e716",
    "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
    "defaultAccessLevel": "allow",
    "accessRules": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
        "deviceClass": {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
          "name": "Name value",
          "type": "model"
        },
        "accessLevel": "allow"
      }
    ],
    "knownDeviceClasses": [
      {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      }
    ]
  }
}
```





