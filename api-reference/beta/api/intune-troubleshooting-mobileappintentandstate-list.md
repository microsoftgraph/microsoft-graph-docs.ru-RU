---
title: Список mobileAppIntentAndStates
description: Свойства списка и связей объектов mobileAppIntentAndState.
author: tfitzmac
ms.openlocfilehash: d8c26cc013714a755ac24242b7dad0dc26f1584c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323053"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="22e19-103">Список mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="22e19-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="22e19-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22e19-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22e19-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22e19-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22e19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22e19-107">Свойства списка и связей объектов [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="22e19-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22e19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22e19-108">Prerequisites</span></span>
<span data-ttu-id="22e19-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22e19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22e19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22e19-111">Permission type</span></span>|<span data-ttu-id="22e19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22e19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22e19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22e19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22e19-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="22e19-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22e19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22e19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22e19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e19-116">Not supported.</span></span>|
|<span data-ttu-id="22e19-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22e19-117">Application</span></span>|<span data-ttu-id="22e19-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22e19-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22e19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22e19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="22e19-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22e19-120">Request headers</span></span>
|<span data-ttu-id="22e19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22e19-121">Header</span></span>|<span data-ttu-id="22e19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22e19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22e19-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22e19-123">Authorization</span></span>|<span data-ttu-id="22e19-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22e19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22e19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22e19-125">Accept</span></span>|<span data-ttu-id="22e19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22e19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22e19-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22e19-127">Request body</span></span>
<span data-ttu-id="22e19-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22e19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22e19-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="22e19-129">Response</span></span>
<span data-ttu-id="22e19-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22e19-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22e19-131">Пример</span><span class="sxs-lookup"><span data-stu-id="22e19-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="22e19-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="22e19-132">Request</span></span>
<span data-ttu-id="22e19-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22e19-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="22e19-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="22e19-134">Response</span></span>
<span data-ttu-id="22e19-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="22e19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





