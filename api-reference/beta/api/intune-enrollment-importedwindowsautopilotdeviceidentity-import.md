---
title: действие импорта
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df7d1b6b069a66bd2f86a55a442aaa5f359517b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736438"
---
# <a name="import-action"></a><span data-ttu-id="9ff9c-103">действие импорта</span><span class="sxs-lookup"><span data-stu-id="9ff9c-103">import action</span></span>

<span data-ttu-id="9ff9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ff9c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ff9c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff9c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff9c-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff9c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ff9c-108">Prerequisites</span></span>
<span data-ttu-id="9ff9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff9c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ff9c-111">Permission type</span></span>|<span data-ttu-id="9ff9c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ff9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff9c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ff9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff9c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff9c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ff9c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ff9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff9c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-116">Not supported.</span></span>|
|<span data-ttu-id="9ff9c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ff9c-117">Application</span></span>|<span data-ttu-id="9ff9c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff9c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff9c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ff9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="9ff9c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ff9c-120">Request headers</span></span>
|<span data-ttu-id="9ff9c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ff9c-121">Header</span></span>|<span data-ttu-id="9ff9c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ff9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff9c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ff9c-123">Authorization</span></span>|<span data-ttu-id="9ff9c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff9c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ff9c-125">Accept</span></span>|<span data-ttu-id="9ff9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff9c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ff9c-127">Request body</span></span>
<span data-ttu-id="9ff9c-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9ff9c-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9ff9c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ff9c-130">Property</span></span>|<span data-ttu-id="9ff9c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff9c-131">Type</span></span>|<span data-ttu-id="9ff9c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff9c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff9c-133">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="9ff9c-133">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="9ff9c-134">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9c-134">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="9ff9c-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9ff9c-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ff9c-136">Response</span></span>
<span data-ttu-id="9ff9c-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-137">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff9c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9ff9c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff9c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ff9c-139">Request</span></span>
<span data-ttu-id="9ff9c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ff9c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ff9c-141">Response</span></span>
<span data-ttu-id="9ff9c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ff9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





