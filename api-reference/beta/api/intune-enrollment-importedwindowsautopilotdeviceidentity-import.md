---
title: действие импорта
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f7d106bfb98e0848511ed52fbbb7d0cb7e3ce76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466572"
---
# <a name="import-action"></a><span data-ttu-id="04ab3-103">действие импорта</span><span class="sxs-lookup"><span data-stu-id="04ab3-103">import action</span></span>

<span data-ttu-id="04ab3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04ab3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04ab3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ab3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04ab3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04ab3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04ab3-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="04ab3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04ab3-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04ab3-108">Prerequisites</span></span>
<span data-ttu-id="04ab3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ab3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04ab3-111">Permission type</span></span>|<span data-ttu-id="04ab3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04ab3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04ab3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04ab3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04ab3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ab3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="04ab3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04ab3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04ab3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04ab3-116">Not supported.</span></span>|
|<span data-ttu-id="04ab3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04ab3-117">Application</span></span>|<span data-ttu-id="04ab3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04ab3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04ab3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04ab3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="04ab3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="04ab3-120">Request headers</span></span>
|<span data-ttu-id="04ab3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04ab3-121">Header</span></span>|<span data-ttu-id="04ab3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="04ab3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04ab3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ab3-123">Authorization</span></span>|<span data-ttu-id="04ab3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04ab3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04ab3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04ab3-125">Accept</span></span>|<span data-ttu-id="04ab3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04ab3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04ab3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="04ab3-127">Request body</span></span>
<span data-ttu-id="04ab3-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04ab3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="04ab3-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="04ab3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="04ab3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="04ab3-130">Property</span></span>|<span data-ttu-id="04ab3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="04ab3-131">Type</span></span>|<span data-ttu-id="04ab3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="04ab3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04ab3-133">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="04ab3-133">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="04ab3-134">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="04ab3-134">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="04ab3-135">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04ab3-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="04ab3-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="04ab3-136">Response</span></span>
<span data-ttu-id="04ab3-137">При успешном выполнении это действие возвращает `200 OK` код отклика и коллекцию [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04ab3-137">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04ab3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="04ab3-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="04ab3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="04ab3-139">Request</span></span>
<span data-ttu-id="04ab3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04ab3-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04ab3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="04ab3-141">Response</span></span>
<span data-ttu-id="04ab3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04ab3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





