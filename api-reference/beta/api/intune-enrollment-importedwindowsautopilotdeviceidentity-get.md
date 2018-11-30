---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
ms.openlocfilehash: be98ceb835469301184bc12a782ecae57340db70
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081788"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="d8a1f-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d8a1f-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="d8a1f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8a1f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8a1f-107">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d8a1f-107">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8a1f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a1f-108">Prerequisites</span></span>
<span data-ttu-id="d8a1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8a1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8a1f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a1f-111">Permission type</span></span>|<span data-ttu-id="d8a1f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8a1f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8a1f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8a1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8a1f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8a1f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d8a1f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8a1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8a1f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-116">Not supported.</span></span>|
|<span data-ttu-id="d8a1f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8a1f-117">Application</span></span>|<span data-ttu-id="d8a1f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8a1f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8a1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8a1f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8a1f-120">Optional query parameters</span></span>
<span data-ttu-id="d8a1f-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d8a1f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8a1f-122">Request headers</span></span>
|<span data-ttu-id="d8a1f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8a1f-123">Header</span></span>|<span data-ttu-id="d8a1f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a1f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8a1f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8a1f-125">Authorization</span></span>|<span data-ttu-id="d8a1f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="d8a1f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8a1f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d8a1f-127">Accept</span></span>|<span data-ttu-id="d8a1f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d8a1f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8a1f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8a1f-129">Request body</span></span>
<span data-ttu-id="d8a1f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8a1f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8a1f-131">Response</span></span>
<span data-ttu-id="d8a1f-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-132">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8a1f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d8a1f-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8a1f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8a1f-134">Request</span></span>
<span data-ttu-id="d8a1f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8a1f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="d8a1f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8a1f-136">Response</span></span>
<span data-ttu-id="d8a1f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="d8a1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





