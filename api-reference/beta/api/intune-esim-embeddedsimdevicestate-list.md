---
title: Список Ембеддедсимдевицестатес
description: Список свойств и связей объектов Ембеддедсимдевицестате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe92ab69b3ef2eb885ff80a4f5b03bf51bcf76a0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983717"
---
# <a name="list-embeddedsimdevicestates"></a><span data-ttu-id="ce084-103">Список Ембеддедсимдевицестатес</span><span class="sxs-lookup"><span data-stu-id="ce084-103">List embeddedSIMDeviceStates</span></span>

> <span data-ttu-id="ce084-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce084-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce084-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce084-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce084-106">Список свойств и связей объектов [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) .</span><span class="sxs-lookup"><span data-stu-id="ce084-106">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce084-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ce084-107">Prerequisites</span></span>
<span data-ttu-id="ce084-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce084-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce084-110">Permission type</span></span>|<span data-ttu-id="ce084-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce084-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce084-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce084-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce084-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce084-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ce084-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce084-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce084-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce084-115">Not supported.</span></span>|
|<span data-ttu-id="ce084-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce084-116">Application</span></span>|<span data-ttu-id="ce084-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce084-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce084-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce084-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="ce084-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce084-119">Request headers</span></span>
|<span data-ttu-id="ce084-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce084-120">Header</span></span>|<span data-ttu-id="ce084-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ce084-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce084-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce084-122">Authorization</span></span>|<span data-ttu-id="ce084-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce084-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce084-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ce084-124">Accept</span></span>|<span data-ttu-id="ce084-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce084-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce084-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ce084-126">Request body</span></span>
<span data-ttu-id="ce084-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce084-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce084-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce084-128">Response</span></span>
<span data-ttu-id="ce084-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [ембеддедсимдевицестате](../resources/intune-esim-embeddedsimdevicestate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce084-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce084-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ce084-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce084-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce084-131">Request</span></span>
<span data-ttu-id="ce084-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce084-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="ce084-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce084-133">Response</span></span>
<span data-ttu-id="ce084-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce084-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





