---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 938b7d0f61c4b2a19437d6e994529320b8c6a128
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466544"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="d011a-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d011a-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="d011a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d011a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d011a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d011a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d011a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d011a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d011a-107">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d011a-107">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d011a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d011a-108">Prerequisites</span></span>
<span data-ttu-id="d011a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d011a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d011a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d011a-111">Permission type</span></span>|<span data-ttu-id="d011a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d011a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d011a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d011a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d011a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d011a-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d011a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d011a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d011a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d011a-116">Not supported.</span></span>|
|<span data-ttu-id="d011a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d011a-117">Application</span></span>|<span data-ttu-id="d011a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d011a-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d011a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d011a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d011a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d011a-120">Optional query parameters</span></span>
<span data-ttu-id="d011a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d011a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d011a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d011a-122">Request headers</span></span>
|<span data-ttu-id="d011a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d011a-123">Header</span></span>|<span data-ttu-id="d011a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d011a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d011a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d011a-125">Authorization</span></span>|<span data-ttu-id="d011a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d011a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d011a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d011a-127">Accept</span></span>|<span data-ttu-id="d011a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d011a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d011a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d011a-129">Request body</span></span>
<span data-ttu-id="d011a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d011a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d011a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d011a-131">Response</span></span>
<span data-ttu-id="d011a-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d011a-132">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d011a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d011a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d011a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d011a-134">Request</span></span>
<span data-ttu-id="d011a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d011a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="d011a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d011a-136">Response</span></span>
<span data-ttu-id="d011a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d011a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "value": {
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
}
```





