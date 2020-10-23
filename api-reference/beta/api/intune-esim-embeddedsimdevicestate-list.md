---
title: Список Ембеддедсимдевицестатес
description: Список свойств и связей объектов Ембеддедсимдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12c2e888c50c0582eb15180b3767a2dbe6393461
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693061"
---
# <a name="list-embeddedsimdevicestates"></a><span data-ttu-id="fe2b5-103">Список Ембеддедсимдевицестатес</span><span class="sxs-lookup"><span data-stu-id="fe2b5-103">List embeddedSIMDeviceStates</span></span>

<span data-ttu-id="fe2b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe2b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe2b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe2b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe2b5-107">Список свойств и связей объектов [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="fe2b5-107">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe2b5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe2b5-108">Prerequisites</span></span>
<span data-ttu-id="fe2b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe2b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe2b5-111">Permission type</span></span>|<span data-ttu-id="fe2b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe2b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe2b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe2b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe2b5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe2b5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fe2b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe2b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe2b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-116">Not supported.</span></span>|
|<span data-ttu-id="fe2b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe2b5-117">Application</span></span>|<span data-ttu-id="fe2b5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe2b5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe2b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe2b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="fe2b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe2b5-120">Request headers</span></span>
|<span data-ttu-id="fe2b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe2b5-121">Header</span></span>|<span data-ttu-id="fe2b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe2b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe2b5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe2b5-123">Authorization</span></span>|<span data-ttu-id="fe2b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe2b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe2b5-125">Accept</span></span>|<span data-ttu-id="fe2b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe2b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe2b5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe2b5-127">Request body</span></span>
<span data-ttu-id="fe2b5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe2b5-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe2b5-129">Response</span></span>
<span data-ttu-id="fe2b5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe2b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fe2b5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe2b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe2b5-132">Request</span></span>
<span data-ttu-id="fe2b5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="fe2b5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe2b5-134">Response</span></span>
<span data-ttu-id="fe2b5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe2b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
      "id": "908884a3-84a3-9088-a384-8890a3848890",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
      "deviceName": "Device Name value",
      "userName": "User Name value",
      "state": "failed",
      "stateDetails": "State Details value"
    }
  ]
}
```





