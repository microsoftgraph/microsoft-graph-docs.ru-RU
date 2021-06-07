---
title: Получение importedWindowsAutopilotDeviceIdentity
description: Чтение свойств и связей между объектамиimportedWindowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 55b4f4fd17fa7f8ea84fe1175898da371ee66ea9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753407"
---
# <a name="get-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="1660a-103">Получение importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1660a-103">Get importedWindowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="1660a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1660a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1660a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1660a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1660a-106">Чтение свойств и связей между объектами[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="1660a-106">Read properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1660a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1660a-107">Prerequisites</span></span>
<span data-ttu-id="1660a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1660a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1660a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1660a-110">Permission type</span></span>|<span data-ttu-id="1660a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1660a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1660a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1660a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1660a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1660a-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1660a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1660a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1660a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1660a-115">Not supported.</span></span>|
|<span data-ttu-id="1660a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1660a-116">Application</span></span>|<span data-ttu-id="1660a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1660a-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1660a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1660a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1660a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1660a-119">Optional query parameters</span></span>
<span data-ttu-id="1660a-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1660a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1660a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1660a-121">Request headers</span></span>
|<span data-ttu-id="1660a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1660a-122">Header</span></span>|<span data-ttu-id="1660a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1660a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1660a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1660a-124">Authorization</span></span>|<span data-ttu-id="1660a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1660a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1660a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1660a-126">Accept</span></span>|<span data-ttu-id="1660a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1660a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1660a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1660a-128">Request body</span></span>
<span data-ttu-id="1660a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1660a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1660a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1660a-130">Response</span></span>
<span data-ttu-id="1660a-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1660a-131">If successful, this method returns a `200 OK` response code and [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1660a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1660a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1660a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1660a-133">Request</span></span>
<span data-ttu-id="1660a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1660a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="1660a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1660a-135">Response</span></span>
<span data-ttu-id="1660a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1660a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 729

{
  "value": {
    "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
    "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
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




