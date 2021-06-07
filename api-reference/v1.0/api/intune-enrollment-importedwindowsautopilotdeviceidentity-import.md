---
title: действие импорта
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 750b525ec0cdf7c28213787920c8164f7fcb1ac5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753406"
---
# <a name="import-action"></a><span data-ttu-id="128ab-103">действие импорта</span><span class="sxs-lookup"><span data-stu-id="128ab-103">import action</span></span>

<span data-ttu-id="128ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="128ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="128ab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="128ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="128ab-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="128ab-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="128ab-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="128ab-107">Prerequisites</span></span>
<span data-ttu-id="128ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="128ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="128ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="128ab-110">Permission type</span></span>|<span data-ttu-id="128ab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="128ab-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="128ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="128ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="128ab-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128ab-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="128ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="128ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="128ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="128ab-115">Not supported.</span></span>|
|<span data-ttu-id="128ab-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="128ab-116">Application</span></span>|<span data-ttu-id="128ab-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="128ab-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="128ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="128ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="128ab-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="128ab-119">Request headers</span></span>
|<span data-ttu-id="128ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="128ab-120">Header</span></span>|<span data-ttu-id="128ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="128ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="128ab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="128ab-122">Authorization</span></span>|<span data-ttu-id="128ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="128ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="128ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="128ab-124">Accept</span></span>|<span data-ttu-id="128ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="128ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="128ab-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="128ab-126">Request body</span></span>
<span data-ttu-id="128ab-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="128ab-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="128ab-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="128ab-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="128ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="128ab-129">Property</span></span>|<span data-ttu-id="128ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="128ab-130">Type</span></span>|<span data-ttu-id="128ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="128ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="128ab-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="128ab-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="128ab-133">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="128ab-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="128ab-134">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="128ab-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="128ab-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="128ab-135">Response</span></span>
<span data-ttu-id="128ab-136">В случае успеха это действие возвращает код ответа и импортируемую `200 OK` [коллекциюWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="128ab-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="128ab-137">Пример</span><span class="sxs-lookup"><span data-stu-id="128ab-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="128ab-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="128ab-138">Request</span></span>
<span data-ttu-id="128ab-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="128ab-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 808

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="128ab-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="128ab-140">Response</span></span>
<span data-ttu-id="128ab-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="128ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 773

{
  "value": [
    {
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
  ]
}
```




