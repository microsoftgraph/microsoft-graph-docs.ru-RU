---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d4d3148e8882aac0db0a25fb000955aaac5f6557
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838341"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="ab6fc-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ab6fc-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="ab6fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab6fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab6fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab6fc-107">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="ab6fc-107">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab6fc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ab6fc-108">Prerequisites</span></span>
<span data-ttu-id="ab6fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab6fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab6fc-111">Permission type</span></span>|<span data-ttu-id="ab6fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab6fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab6fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab6fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab6fc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab6fc-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ab6fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab6fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab6fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-116">Not supported.</span></span>|
|<span data-ttu-id="ab6fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab6fc-117">Application</span></span>|<span data-ttu-id="ab6fc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab6fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab6fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="ab6fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab6fc-120">Request headers</span></span>
|<span data-ttu-id="ab6fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab6fc-121">Header</span></span>|<span data-ttu-id="ab6fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab6fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab6fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab6fc-123">Authorization</span></span>|<span data-ttu-id="ab6fc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab6fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab6fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab6fc-125">Accept</span></span>|<span data-ttu-id="ab6fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab6fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab6fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab6fc-127">Request body</span></span>
<span data-ttu-id="ab6fc-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab6fc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab6fc-129">Response</span></span>
<span data-ttu-id="ab6fc-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-130">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab6fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ab6fc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab6fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab6fc-132">Request</span></span>
<span data-ttu-id="ab6fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="ab6fc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab6fc-134">Response</span></span>
<span data-ttu-id="ab6fc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ab6fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      }
    }
  ]
}
```





