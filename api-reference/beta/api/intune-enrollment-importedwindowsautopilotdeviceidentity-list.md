---
title: Список importedWindowsAutopilotDeviceIdentities
description: Список свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d99edced6a20f243441fd755ec1e343fc6e6dc61
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729980"
---
# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="b489d-103">Список importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="b489d-103">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="b489d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b489d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b489d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b489d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b489d-106">Список свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b489d-106">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b489d-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b489d-107">Prerequisites</span></span>
<span data-ttu-id="b489d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b489d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b489d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b489d-110">Permission type</span></span>|<span data-ttu-id="b489d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b489d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b489d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b489d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b489d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b489d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b489d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b489d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b489d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b489d-115">Not supported.</span></span>|
|<span data-ttu-id="b489d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b489d-116">Application</span></span>|<span data-ttu-id="b489d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b489d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b489d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b489d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b489d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b489d-119">Request headers</span></span>
|<span data-ttu-id="b489d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b489d-120">Header</span></span>|<span data-ttu-id="b489d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b489d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b489d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b489d-122">Authorization</span></span>|<span data-ttu-id="b489d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b489d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b489d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b489d-124">Accept</span></span>|<span data-ttu-id="b489d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b489d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b489d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b489d-126">Request body</span></span>
<span data-ttu-id="b489d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b489d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b489d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b489d-128">Response</span></span>
<span data-ttu-id="b489d-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b489d-129">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b489d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b489d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b489d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b489d-131">Request</span></span>
<span data-ttu-id="b489d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b489d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="b489d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b489d-133">Response</span></span>
<span data-ttu-id="b489d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b489d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 825

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "importId": "Import Id value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      },
      "assignedUserPrincipalName": "Assigned User Principal Name value"
    }
  ]
}
```





