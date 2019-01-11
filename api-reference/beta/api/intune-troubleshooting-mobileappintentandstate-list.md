---
title: Список mobileAppIntentAndStates
description: Свойства списка и связей объектов mobileAppIntentAndState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 95fd038a37b81168fd0381d44bbdb2a29d604d0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841449"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="6cc04-103">Список mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="6cc04-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="6cc04-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6cc04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cc04-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cc04-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6cc04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cc04-107">Свойства списка и связей объектов [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="6cc04-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6cc04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6cc04-108">Prerequisites</span></span>
<span data-ttu-id="6cc04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cc04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cc04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cc04-111">Permission type</span></span>|<span data-ttu-id="6cc04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cc04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cc04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cc04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cc04-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cc04-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6cc04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cc04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cc04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc04-116">Not supported.</span></span>|
|<span data-ttu-id="6cc04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cc04-117">Application</span></span>|<span data-ttu-id="6cc04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cc04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cc04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="6cc04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cc04-120">Request headers</span></span>
|<span data-ttu-id="6cc04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cc04-121">Header</span></span>|<span data-ttu-id="6cc04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6cc04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cc04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cc04-123">Authorization</span></span>|<span data-ttu-id="6cc04-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6cc04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cc04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cc04-125">Accept</span></span>|<span data-ttu-id="6cc04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cc04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cc04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6cc04-127">Request body</span></span>
<span data-ttu-id="6cc04-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cc04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cc04-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cc04-129">Response</span></span>
<span data-ttu-id="6cc04-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6cc04-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cc04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6cc04-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6cc04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cc04-132">Request</span></span>
<span data-ttu-id="6cc04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cc04-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="6cc04-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cc04-134">Response</span></span>
<span data-ttu-id="6cc04-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6cc04-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```





