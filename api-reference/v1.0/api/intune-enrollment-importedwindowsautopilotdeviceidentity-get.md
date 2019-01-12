---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e46771b73082ac8b1f3b70a6a694f3392417bc5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943517"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="6d9d1-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="6d9d1-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="6d9d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d9d1-105">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="6d9d1-105">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6d9d1-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6d9d1-106">Prerequisites</span></span>
<span data-ttu-id="6d9d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d9d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d9d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d9d1-109">Permission type</span></span>|<span data-ttu-id="6d9d1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d9d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d9d1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d9d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d9d1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d9d1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6d9d1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d9d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d9d1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-114">Not supported.</span></span>|
|<span data-ttu-id="6d9d1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d9d1-115">Application</span></span>|<span data-ttu-id="6d9d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d9d1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d9d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d9d1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6d9d1-118">Optional query parameters</span></span>
<span data-ttu-id="6d9d1-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6d9d1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d9d1-120">Request headers</span></span>
|<span data-ttu-id="6d9d1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d9d1-121">Header</span></span>|<span data-ttu-id="6d9d1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6d9d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d9d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d9d1-123">Authorization</span></span>|<span data-ttu-id="6d9d1-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6d9d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d9d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6d9d1-125">Accept</span></span>|<span data-ttu-id="6d9d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d9d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d9d1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d9d1-127">Request body</span></span>
<span data-ttu-id="6d9d1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d9d1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d9d1-129">Response</span></span>
<span data-ttu-id="6d9d1-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-130">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d9d1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6d9d1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d9d1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d9d1-132">Request</span></span>
<span data-ttu-id="6d9d1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="6d9d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d9d1-134">Response</span></span>
<span data-ttu-id="6d9d1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6d9d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": {
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
}
```



