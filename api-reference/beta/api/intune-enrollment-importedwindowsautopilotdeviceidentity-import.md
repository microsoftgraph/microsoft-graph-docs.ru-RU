---
title: действие импорта
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4da744d7acd78b31b27238805fb63aa9cb7e3186
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730001"
---
# <a name="import-action"></a><span data-ttu-id="10d60-103">действие импорта</span><span class="sxs-lookup"><span data-stu-id="10d60-103">import action</span></span>

> <span data-ttu-id="10d60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10d60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="10d60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10d60-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="10d60-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10d60-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="10d60-107">Prerequisites</span></span>
<span data-ttu-id="10d60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10d60-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10d60-110">Permission type</span></span>|<span data-ttu-id="10d60-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="10d60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10d60-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10d60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10d60-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10d60-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10d60-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10d60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10d60-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d60-115">Not supported.</span></span>|
|<span data-ttu-id="10d60-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10d60-116">Application</span></span>|<span data-ttu-id="10d60-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10d60-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10d60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="10d60-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10d60-119">Request headers</span></span>
|<span data-ttu-id="10d60-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10d60-120">Header</span></span>|<span data-ttu-id="10d60-121">Значение</span><span class="sxs-lookup"><span data-stu-id="10d60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10d60-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10d60-122">Authorization</span></span>|<span data-ttu-id="10d60-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10d60-124">Accept</span><span class="sxs-lookup"><span data-stu-id="10d60-124">Accept</span></span>|<span data-ttu-id="10d60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10d60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10d60-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10d60-126">Request body</span></span>
<span data-ttu-id="10d60-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10d60-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="10d60-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="10d60-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="10d60-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="10d60-129">Property</span></span>|<span data-ttu-id="10d60-130">Тип</span><span class="sxs-lookup"><span data-stu-id="10d60-130">Type</span></span>|<span data-ttu-id="10d60-131">Описание</span><span class="sxs-lookup"><span data-stu-id="10d60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10d60-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="10d60-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="10d60-133">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="10d60-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="10d60-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="10d60-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="10d60-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="10d60-135">Response</span></span>
<span data-ttu-id="10d60-136">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10d60-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10d60-137">Пример</span><span class="sxs-lookup"><span data-stu-id="10d60-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="10d60-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="10d60-138">Request</span></span>
<span data-ttu-id="10d60-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10d60-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10d60-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d60-140">Response</span></span>
<span data-ttu-id="10d60-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10d60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





