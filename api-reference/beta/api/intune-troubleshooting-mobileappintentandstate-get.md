---
title: Получение mobileAppIntentAndState
description: Чтение свойства и связи объекта mobileAppIntentAndState.
author: tfitzmac
ms.openlocfilehash: 18a73a1ca4c8c832ff4d69c1a61c876f4d88e2a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352670"
---
# <a name="get-mobileappintentandstate"></a><span data-ttu-id="ff2fa-103">Получение mobileAppIntentAndState</span><span class="sxs-lookup"><span data-stu-id="ff2fa-103">Get mobileAppIntentAndState</span></span>

> <span data-ttu-id="ff2fa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff2fa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff2fa-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff2fa-107">Чтение свойства и связи объекта [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) .</span><span class="sxs-lookup"><span data-stu-id="ff2fa-107">Read properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff2fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ff2fa-108">Prerequisites</span></span>
<span data-ttu-id="ff2fa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff2fa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff2fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff2fa-111">Permission type</span></span>|<span data-ttu-id="ff2fa-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff2fa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff2fa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff2fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff2fa-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff2fa-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ff2fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff2fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff2fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-116">Not supported.</span></span>|
|<span data-ttu-id="ff2fa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff2fa-117">Application</span></span>|<span data-ttu-id="ff2fa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff2fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff2fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff2fa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff2fa-120">Optional query parameters</span></span>
<span data-ttu-id="ff2fa-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff2fa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff2fa-122">Request headers</span></span>
|<span data-ttu-id="ff2fa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff2fa-123">Header</span></span>|<span data-ttu-id="ff2fa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ff2fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff2fa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff2fa-125">Authorization</span></span>|<span data-ttu-id="ff2fa-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff2fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff2fa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ff2fa-127">Accept</span></span>|<span data-ttu-id="ff2fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff2fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff2fa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff2fa-129">Request body</span></span>
<span data-ttu-id="ff2fa-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff2fa-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff2fa-131">Response</span></span>
<span data-ttu-id="ff2fa-132">Успешно завершена, этот метод возвращает `200 OK` объект [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-132">If successful, this method returns a `200 OK` response code and [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff2fa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ff2fa-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff2fa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff2fa-134">Request</span></span>
<span data-ttu-id="ff2fa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates/{mobileAppIntentAndStateId}
```

### <a name="response"></a><span data-ttu-id="ff2fa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff2fa-136">Response</span></span>
<span data-ttu-id="ff2fa-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff2fa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 943

{
  "value": {
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
}
```





