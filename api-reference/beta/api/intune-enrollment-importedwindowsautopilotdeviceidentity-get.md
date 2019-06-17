---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c349cbe092d638c113031d6499ff6c0615bfee9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981757"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="cdaff-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cdaff-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="cdaff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdaff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdaff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdaff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdaff-106">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="cdaff-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdaff-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cdaff-107">Prerequisites</span></span>
<span data-ttu-id="cdaff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdaff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdaff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdaff-110">Permission type</span></span>|<span data-ttu-id="cdaff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdaff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdaff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdaff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cdaff-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdaff-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cdaff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdaff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdaff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdaff-115">Not supported.</span></span>|
|<span data-ttu-id="cdaff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdaff-116">Application</span></span>|<span data-ttu-id="cdaff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdaff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdaff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdaff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdaff-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdaff-119">Optional query parameters</span></span>
<span data-ttu-id="cdaff-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdaff-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdaff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdaff-121">Request headers</span></span>
|<span data-ttu-id="cdaff-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdaff-122">Header</span></span>|<span data-ttu-id="cdaff-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cdaff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdaff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdaff-124">Authorization</span></span>|<span data-ttu-id="cdaff-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdaff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdaff-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cdaff-126">Accept</span></span>|<span data-ttu-id="cdaff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cdaff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdaff-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdaff-128">Request body</span></span>
<span data-ttu-id="cdaff-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdaff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdaff-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdaff-130">Response</span></span>
<span data-ttu-id="cdaff-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cdaff-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdaff-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cdaff-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdaff-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdaff-133">Request</span></span>
<span data-ttu-id="cdaff-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdaff-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="cdaff-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdaff-135">Response</span></span>
<span data-ttu-id="cdaff-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdaff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 743

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
    "orderIdentifier": "Order Identifier value",
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
}
```





