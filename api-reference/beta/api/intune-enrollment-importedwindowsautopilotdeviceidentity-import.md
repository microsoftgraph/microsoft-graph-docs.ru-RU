---
title: действие импорта
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2ad866ad8180a6e65d7dafe2628bcb9e9be2921b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943777"
---
# <a name="import-action"></a><span data-ttu-id="a6517-103">действие импорта</span><span class="sxs-lookup"><span data-stu-id="a6517-103">import action</span></span>

> <span data-ttu-id="a6517-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6517-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6517-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6517-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6517-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="a6517-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6517-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a6517-107">Prerequisites</span></span>
<span data-ttu-id="a6517-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6517-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6517-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6517-110">Permission type</span></span>|<span data-ttu-id="a6517-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6517-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6517-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6517-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6517-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6517-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a6517-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6517-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6517-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6517-115">Not supported.</span></span>|
|<span data-ttu-id="a6517-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6517-116">Application</span></span>|<span data-ttu-id="a6517-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6517-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6517-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6517-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="a6517-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6517-119">Request headers</span></span>
|<span data-ttu-id="a6517-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6517-120">Header</span></span>|<span data-ttu-id="a6517-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a6517-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6517-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6517-122">Authorization</span></span>|<span data-ttu-id="a6517-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6517-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6517-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a6517-124">Accept</span></span>|<span data-ttu-id="a6517-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6517-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6517-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6517-126">Request body</span></span>
<span data-ttu-id="a6517-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6517-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a6517-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="a6517-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a6517-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6517-129">Property</span></span>|<span data-ttu-id="a6517-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a6517-130">Type</span></span>|<span data-ttu-id="a6517-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a6517-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6517-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="a6517-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="a6517-133">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="a6517-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="a6517-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a6517-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a6517-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6517-135">Response</span></span>
<span data-ttu-id="a6517-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6517-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6517-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a6517-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6517-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6517-138">Request</span></span>
<span data-ttu-id="a6517-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6517-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 860

{
  "importedWindowsAutopilotDeviceIdentities": [
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

### <a name="response"></a><span data-ttu-id="a6517-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6517-140">Response</span></span>
<span data-ttu-id="a6517-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6517-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





