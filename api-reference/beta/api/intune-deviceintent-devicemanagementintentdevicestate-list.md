---
title: Список Девицеманажементинтентдевицестатес
description: Список свойств и связей объектов Девицеманажементинтентдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 810969a55ce8e5c31768264d7e34b75df23f4369
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470954"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="a7f57-103">Список Девицеманажементинтентдевицестатес</span><span class="sxs-lookup"><span data-stu-id="a7f57-103">List deviceManagementIntentDeviceStates</span></span>

<span data-ttu-id="a7f57-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7f57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7f57-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7f57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7f57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7f57-107">Список свойств и связей объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="a7f57-107">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7f57-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7f57-108">Prerequisites</span></span>
<span data-ttu-id="a7f57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7f57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f57-111">Permission type</span></span>|<span data-ttu-id="a7f57-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7f57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7f57-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7f57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7f57-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7f57-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7f57-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7f57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7f57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f57-116">Not supported.</span></span>|
|<span data-ttu-id="a7f57-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7f57-117">Application</span></span>|<span data-ttu-id="a7f57-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7f57-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7f57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7f57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="a7f57-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a7f57-120">Request headers</span></span>
|<span data-ttu-id="a7f57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7f57-121">Header</span></span>|<span data-ttu-id="a7f57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7f57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7f57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7f57-123">Authorization</span></span>|<span data-ttu-id="a7f57-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7f57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7f57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7f57-125">Accept</span></span>|<span data-ttu-id="a7f57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7f57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7f57-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7f57-127">Request body</span></span>
<span data-ttu-id="a7f57-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7f57-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7f57-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7f57-129">Response</span></span>
<span data-ttu-id="a7f57-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7f57-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7f57-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a7f57-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7f57-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7f57-132">Request</span></span>
<span data-ttu-id="a7f57-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7f57-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="a7f57-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f57-134">Response</span></span>
<span data-ttu-id="a7f57-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7f57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
      "id": "8db75881-5881-8db7-8158-b78d8158b78d",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable",
      "deviceId": "Device Id value"
    }
  ]
}
```





